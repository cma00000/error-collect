# JIBO 问题汇总
## 1.NLU组件Windows环境下载失败 
  >**Reproduce: Download jibo-nlu-js-v0.12.0-win32-ia32.zip
  >**Error: Timeout

Disable 并卸载jibo-sdk ，重新用atom安装，刷新页面
## 2.模拟器NLU接口无定义
>模拟器上： Request URL: file:///opt/jibo/jibo-nlu/undefined/nlu_interface

>真机上： Request URL: http://127.0.0.1: 11231/nlu_interface


