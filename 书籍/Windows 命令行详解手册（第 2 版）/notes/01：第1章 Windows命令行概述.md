---
title: 第1章 Windows命令行概述
hidden: true
---

# 第1章 Windows命令行概述

- [x] 1.1 [命令行基础](#命令行基础)
  - 1.1.1 [理解Windows命令shell](#理解Windows命令shell)
  - 1.1.2 理解MS-DOS命令shell
  - 1.1.3 理解Windows PowerShell
  - 1.1.4 配置命令行属性
  - 1.1.5 [使用命令历史](#使用命令历史)
- [x] 1.2 使用补充的组件
  - 1.2.1 在Windows Vista中使用微软远程服务器管理工具
  - 1.2.2 注册远程服务器管理工具包
  - 1.2.3 配置与选择远程服务器管理工具
  - 1.2.4 删除远程服务器管理工具
  - 1.2.5 删除远程服务器管理工具软件包

## 命令行基础

### 理解Windows命令shell

**`cmd` 内部命令简明参考：**

| 命令           | 描述                                                         |
| -------------- | ------------------------------------------------------------ |
| `assoc`        | 显示或修改当前的文件扩展关联                                 |
| `break`        | 设置调试中断                                                 |
| `call`         | 在一个脚本内调用程序或其他脚本                               |
| `cd(chdir)`    | 显示当前目录名或改变当前目录位置                             |
| `cls`          | 清理命令窗口并擦除屏幕缓冲区                                 |
| `color`        | 设置命令shell窗口的文本与背景色                              |
| `copy`         | 将文件从一个位置复制到另外的位置，或者将多个文件连接在一-起  |
| `date`         | 显示或设置系统日期                                           |
| `del(erase)`   | 删除指定的文件、多个文件或目录                               |
| `dir`          | 显示当前目录或指定目录中的子目录与文件列表                   |
| `dpath`        | 允许程序打开指定目录中的数据文件(就像在当前目录中一样)       |
| `echo`         | 显示命令行的文本字符串，设置命令回显状态(on\|off)            |
| `endlocal`     | 变量局部化结束                                               |
| `exit`         | 退出命令shell                                                |
| `for`          | 对一组文件中的每一文件运行指定的命令                         |
| `ftype`        | 显示当前的文件类型或修改文件类型(文件扩展关联中使用)         |
| `goto`         | 将命令解释器直接跳转到批处理脚本中某个标记行                 |
| `if`           | 命令的条件执行                                               |
| `md(mkdir)`    | 在当前目录或指定目录下创建子目录                             |
| `mklink`       | 为文件或目录创建符号链接或硬链接                             |
| `move`         | 将一个或多个文件从当前目录或指定源目录移动到指定的目标目录，也可以用于对目录进行重命名 |
| `path`         | 显示或设置操作系统用于搜索可执行文件与脚本的命令路径         |
| `pause`        | 中断批处理文件的处理过程(挂起)，等待键盘输入                 |
| `popd`         | 弹出由PUSHD保存的目录，使其成为当前目录                      |
| `prompt`       | 为命令提示符设置文本                                         |
| `pushd`        | 保存当前目录位置，之后跳转到指定的目录(可选)                 |
| `rd(rmdir)`    | 移除目录(也可以移除其子目录)                                 |
| `rem`          | 在批处理脚本或Config.sys中设置标记                           |
| `ren(renamne)` | 对一个或多个文件进行重命名                                   |
| `set`          | 显示当前的环境变量，或者为当前命令shell设置临时变量          |
| `setlocal`     | 在批处理脚本中标记变量局部化的开始                           |
| `shift`        | 改变批处理脚本中可替换变量的位置                             |
| `start`        | 启动一个单独的窗口，以便运行指定的程序或命令                 |
| `time`         | 显示或设置系统时间                                           |
| `title`        | 设置命令shell窗口的标题                                      |
| `type`         | 显示文本文件的内容                                           |
| `verify`       | 在将文件写入磁盘后，指令操作系统对其进行验证                 |
| `vol`          | 显示磁盘卷标与序列号                                         |

### 使用命令历史

- 上下箭头

- F7 选择历史
- F8 前缀匹配
