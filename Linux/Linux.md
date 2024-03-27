# Linux 系统相关指令

## 1.查看信息类

- uname -m 查看架构

- uname -a 查看操作系统等所有信息

- which（which is）查找文件

- cat 是一个显示的命令

## 2.文件权限问题

**linux 运行.sh 出现 Permission denied 解决办法**

给 sh 文件权限

    chmod +x your_script.sh

暂停进程是 Ctrl+z；终止进程是 Ctrl+c

## 3.screen 方法

### 安装 screen

### screen 相关命令

screen -r name&#x20;

唤醒 screen 终端

    screen -r -d 2467

恢复 screen 界面

- **新建 screen**

  screen -S your_screen_name

- **进入 screen**

  screen -r your_screen_name

  Ctrl+D # 在当前 screen 下，输入 Ctrl+D，删除该 screen&#x20;

  Ctrl+A，Ctrl+D # 在当前 screen 下，输入先后 Ctrl+A，Ctrl+D，退出该 screen

- **显示 screen list**

  ​​​​​​screen -ls

- **连接状态为【Attached】的 screen**

  screen -D -r your_screen_name # 解释：-D -r 先踢掉前一用户，再登陆

- **判断当前是否在 screen 中断下,Ubuntu 系统,可以这样:**

  sudo vim /etc/screenrc

- **删除指定 screen, your_screen_name 为待删除的 screen name**

  ​​​​​​screen -S your_screen_name -X quit

## 4.暂停进程与恢复

使用 ctrl+z 可以暂停进程，然后 fg+序号恢复进程

## 5.压缩与解压缩

### 5.1zip 与 unizp

打包目录的是要加-r（递归打包）-q 是静默操作（也就是不会向控制台输出信息

### 5.2

## 6.文件类

### 6.1 文件的复制

命令是 cp

**语法：**

cp \[options] source destination

#### **a. 复制文件**

cp foo.txt bar.txt

该命令将把  `foo.txt`  文件的内容复制到名为  `bar.txt`  的文件中。

**示例：**

假设您有一个名为  `foo.txt`  的文件，内容如下：

Hello, World!

如果运行  `cp foo.txt bar.txt`  命令，就会创建一个名为  `bar.txt`  的新文件，其内容与  `foo.txt`  完全相同：

Hello, World!

如果  `bar.txt`  已经存在，其内容将被  `foo.txt`  的内容覆盖。如果 bar.txt 不存在，则会被创建。

#### **b. 复制目录（及其内容）**

cp -R foo-folder bar-folder

`-R`  选项代表 “递归”，用于复制目录及其内容，包括子目录。

下面是  `cp -R foo-folder bar-folder`  命令的作用：

- `cp`: 调用复制命令。

- `-R`: 告诉命令进行递归操作，复制所有目录和子目录。

- `foo-folder`: 要复制的源目录。

- `bar-folder`: 要复制源目录的目标目录。

  

### 6.2文件查看

- 可以使用 touch 等创建，cat 可以查看

- 可以使用 vim，nano，gedit 进行查看与编辑。
