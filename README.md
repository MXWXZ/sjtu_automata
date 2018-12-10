# AutoElect
![Version](https://img.shields.io/badge/Version-0.1.0-blue.svg)![Language](https://img.shields.io/badge/Language-Python3-red.svg)![License](https://img.shields.io/badge/License-GPL--3.0-yellow.svg)

**注意！此版本为BETA版，未经过严格测试，可能存在BUG，如有问题请提交[issue](https://github.com/MXWXZ/AutoElect/issues)**

上海交通大学抢课脚本\
协议分析：<https://github.com/MXWXZ/AutoElect/blob/master/Protocol%20analysis.md>

## 使用脚本你可以做到
:heavy_check_mark: 无人值守自动抢课\
:heavy_check_mark: 并发抢课提升成功率\
~~:heavy_check_mark: 卡时间准时抢课（暂不开放）~~

## 使用脚本你不能做到
:x: 违反选课规则选课\
:x: 提高您的网速\
:x: 保证一定可以抢到课

## 系统环境测试程度
最佳支持：Ubuntu 18.04 LTS with Python 3.6.7

Linux > Windows >> ~~macOS=0（没钱无测试）~~

## 安装
    
    pip3 install colorama requests Pillow click
    git clone https://github.com/MXWXZ/AutoElect.git
    cd AutoElect

### [可选]验证码自动识别
可以不装，但是需要图形界面支持或者可以打开`captcha.jpeg`验证码图片：

    pip3 install pytesseract

然后安装`tesseract`，不同系统方法不同：\
Ubuntu 18.04：

    sudo apt install tesseract-ocr libtesseract-dev

其他版本/发行版/Windows等自行看文档：https://github.com/tesseract-ocr/tesseract/wiki
    
## 简单使用说明
**注意：教务网限制同一时间只允许有一个session登陆，即如果您正在使用本程序，请不要在网页或其他地方再次登陆教务网，否则将导致登陆失效，选课失败（喜欢折腾的可以参考高级用法规避）。**

## 参数说明
使用：`python3 autoelect.py [-OPTIONS]`

|参数|长参数形式|说明|
|:--:|:--:|:--:|

## 高级用法

## 一些说明
1. 为了尽量减少第三方库的使用，本脚本并未集成且也不会集成验证码识别的功能

## 二次开发
1. 安全考虑，任何二次开发不允许自行询问或保存Jaccount用户名/密码，需要登陆请调用`Login`函数