# StudentMain Manager 2
![](https://img.shields.io/badge/language-C%23-blue) ![](https://img.shields.io/badge/version-2.0.0-brightgreen) ![](https://img.shields.io/github/repo-size/yangshunhuai/StudentMainManager2)

StudentMain Manager 第二代，一个专杀极域电子教室的C#程序，具有基于WinForm的GUI。

## 原理
* 使用NTSD调试工具，取得Debug权限后强制结束极域教室（无论极域教室有没有设置任务管理器防杀）。
* 使用微软官方Sysinternals的工具[PsSuspend](https://docs.microsoft.com/zh-cn/sysinternals/downloads/pssuspend)挂起StudentMain进程，可以使得教师端定格画面但不会显示学生端断开。
* 使用IE的全屏模式，将教师端控制屏幕变成一个窗口，可以在进行自己的操作的同时看老师上课。
* 给Windows自带的`sethc.exe`快捷键打补丁，即使不慎被控屏，只需按下5次Shift键即可轻松逃脱控屏。
* 可以配套使用GitHub用户 @快乐的梦鱼 的[JiYuTrainer](https://github.com/imengyu/JiYuTrainer)，取得更好的控制效果。

## 系统要求
由于Windows XP在它诞生将近20年后，早已退出了历史舞台，本程序不计划支持Windows XP。

对于32位的支持，本程序是可以实现的。

## 使用协议 & 免责声明

若你使用本程序，即认为你已阅读并同意以下条款：

* 本程序仅供学习交流之用途，**禁止将本程序用于任何不道德、不遵守法律的行为**。如果不遵守，产生的后果自负。
* 本程序从你已经了解老师上课的内容的角度出发。如果你希望使用本软件，请务必保证你已经充分了解老师上课的内容。
  如果因为使用本程序而导致对学业成绩的影响，**后果自负**。
* 请遵守本程序的开源协议。

若你不同意以上条款，请**不要使用此程序**。

## 手动构建
本程序是基于Visual Studio 2017开发的，所以只要配置好了Visual Studio 2017和.NET开发环境，是很容易编译的。只需打开sln文件并且在上方点击生成->生成解决方案。

## 开源协议
GPL-v2（见[`/LICENSE`](https://github.com/yangshunhuai/StudentMainManager2/blob/main/LICENSE)）