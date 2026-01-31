# 神经网络与深度学习

书籍地址：
[神经网络与深度学习](https://nndl.github.io/)
[nndl-book.pdf](./doc/nndl-book.pdf)

## 项目信息：
项目地址：https://github.com/SGL23187/nndl

本项目是用于共同学习《神经网络与深度学习》一书的代码实现与笔记整理。个人笔记文档存在`xxx_diary`文件夹和`xxx_diary\notes`文件夹中。建议日记使用markdown格式编写,note使用jupyter notebook编写。

## git分支说明：
- `main`: 主分支，仅接收合并请求，由项目负责人审核并合并
- `personal/<username>`: 个人分支，用于提交各自的学习笔记和代码实现

## Git 工作流程：

### git基本操作：

**第一步：克隆项目仓库**
```bash
git clone https://github.com/SGL23187/nndl.git
```
- 该命令将远程仓库克隆到本地，创建一个名为 `nndl` 的文件夹，并下载所有文件和历史记录。

```bash
cd nndl
```
- 进入克隆下来的项目目录，以便进行后续操作。

**第二步：创建个人分支**
```bash
git checkout -b personal/<your-username>
```
- 该命令创建一个新的分支，命名为 `personal/<your-username>`，并切换到该分支。个人分支用于提交各自的学习笔记和代码实现。

**第三步：本地开发与提交**
```bash
git add .
```
- 将所有更改的文件添加到暂存区，准备提交。

```bash
git commit -m "描述你的更改"
```
- 提交暂存区的更改到本地仓库，并附上描述信息，说明所做的更改。

**第四步：推送到远程个人分支**
```bash
git push origin personal/<your-username>
```
- 将本地的个人分支推送到远程仓库，使其他人能够看到你的更改。

**第五步：等待项目负责人审核与合并**
- 项目负责人负责所有的代码审查和 `main` 分支合并工作。确保你的代码符合项目标准。
- 避免直接向 `main` 分支提交代码，所有更改应通过个人分支进行。

**保持个人分支更新**
```bash
git fetch origin
```
- 从远程仓库获取最新的更改，但不合并。

```bash
git rebase origin/main
```
- 将你的个人分支更新到最新的 `main` 分支，确保你的更改基于最新的代码。

## uv环境配置
如果没有安装uv环境，可以从tools文件夹下，把uv文件夹复制到你专门装环境的地方
比如我是：`D:\2Environments\uv`
然后保存环境变量：
```powershell
$env:UV_HOME="D:\2Environments\uv"
$env:PATH="$env:UV_HOME\bin;$env:PATH"
```




