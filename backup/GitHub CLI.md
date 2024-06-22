# GitHub CLI

## 先决条件

### 安装CLI
根据自身操作系统架构选择对应的CLI版本

### 进行身份验证
`gh auth login`

### 选择协议
根据提示选择Git协议为HTTPS或SSH（推荐选择HTTPS）

## 常用命令

### 1.查看状态
`git status`

### 2.克隆存储库
`git repo clone OWNER/REPO` 将其存储库克隆到本地计算机中

### 3.创建存储库
`git repo create` 根据提示创建自己的存储库

### 4.处理问题
`git issue list --repo OWNER/REPO` 列出当前为指定存储库打开的最近创建的问题
若在本地Git存储库运行`issue`命令则可以省略--repo OWNER/REPO的命令

### 5.处理拉取请求
`git pr list --repo OWNER/REPO` 列出当前为指定存储库打开的最近创建的拉取请求
若在本地Git存储库运行`pr`命令则可以省略--repo OWNER/REPO的命令

### 6.处理codespace
输入`gh codespace create`来根据提示创建新的codespace
输入`gh codespace list`来显示现有的codespace
可以用cs代替codespace

### 7.获得帮助
输入`gh`显示顶级的GitHub CLI命令
对于具体的用法帮助，需要在后面增加--help
