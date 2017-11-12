# PHP_WEBSHELL_FUCKER
Judge a php webshell by php engine &amp; hook

## 需求
为解决服务端难以判断文件是否为webshell、存在漏报、误报等情况

## 思路
通过修改PHP源码，制作一个类似于PHP版的RootKit，通过脚本的行为来进行判断

目前的主要行为有：
* 对不安全函数的使用（中）
* 对断言、eval的使用（高）
* 对用户输入与上述之间的关系做判断
* 对上下文的检测
* 对与用户输入相关的变量的检测

### PHP版本
php7.1.11 (sha256 7646d7de701fc969e3305eeeb2eddda3d46af6a88ee20ef4a47270c447228573)
