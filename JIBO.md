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

联系Jibo技术人员，降低SDk版本（在node-module/jibo中的package.json有依赖），或者升级系统

## 4.连接不到
>**Could not connect to Netposa. Make sure the robot is turned on.

原因可能是：1.未开机 2.刚开机还没连接到 3.系统更新（都无法打开Body Service网页).
## 5.中文character
>**中文字库没有，可以在模拟器中引入webfont， 但是依旧无法在真机显示。

JIBO回复：目前尚不支持UTF-8字符编码（2016-06-07）
## 6.jibo-cli删除上传文件的命令
>**

JIBO回复：可根据大家需求，考虑以后添加新的命令支持。
## 6.1.jibo-cli查看剩余存储空间的命令

df -h
## 7.SKILL创建在sdk为1.2.7以前版本
>**
Update a skill to the newest APIs

If your skill was created with jibo-sdk v1.2.7 or earlier, you may need to update to fuzzy versioning first. See the next section for instructions.

Open your command line interface.
Change directories to your skill's top-level folder.
Run: npm install
Click View > Developer > Reload Window on the Atom toolbar to refresh your skill.
Update an old skill to use fuzzy versioning

If your skill was created with jibo-sdk v1.2.7 or earlier:

Open the skill you want to update.
If you do not see the Project pane, click View > Toggle Tree View.
Click package.json at the bottom of the Project pane to open it.
In the dependencies node, change the jibo version to ^3.0.0 to use fuzzy versioning. You will no longer have to manually update this dependency when updating this skill.
For example, change: "jibo": "2.0.5" to: "jibo": "^3.0.0"
Run: npm install
Click View > Developer > Reload Window on the Atom toolbar to refresh your skill.

## 8.使用jibo.lps.setPreview()时的报错
>**e is not a function.

待解决

## 9.使用Parallel Behavior其中一个为循环,完成另一项即可结束
>**

Behavior Arguments: succeedOnOne.


