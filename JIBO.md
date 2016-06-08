# JIBO 问题汇总
## 1.NLU组件Windows环境下载失败 
>**Reproduce: Download jibo-nlu-js-v0.12.0-win32-ia32.zip
>**Error: Timeout

Disable 并卸载jibo-sdk ，重新用atom安装，刷新页面
## 2.模拟器NLU接口无定义
>**模拟器上： Request URL: http://127.0.0.1: 11231/nlu_interface

>**真机上： Request URL: file:///opt/jibo/jibo-nlu/undefined/nlu_interface

待解决...
## 3.平台版本低
>**Error：Platform version check failed! Skill allows version >=0.12.0 but your current version is 0.11.1.

联系Jibo技术人员，降低SDk版本，或者升级系统

## 4.连接不到
>**Could not connect to Netposa. Make sure the robot is turned on.

原因可能是：1.未开机 2.刚开机还没连接到 3.系统更新（都无法打开Body Service网页).
## 5.中文character
>**中文字库没有，可以在模拟器中引入webfont， 但是依旧无法在真机显示。

JIBO回复：目前尚不支持UTF-8字符编码（2016-06-07）
## 6.jibo-cli删除上传文件的命令
>**

JIBO回复：可根据大家需求，考虑以后添加新的命令支持。



