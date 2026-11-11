# test1

用于练习本地文件、文件夹上传到 GitHub，以及修改后更新仓库。

- 本机目录：`/home/robot/my_projects`
- GitHub 仓库：https://github.com/shiqistar/test1
- 分支：`main`
- 连接方式：SSH

## 已完成的演示

1. 创建 `examples/hello.txt`，提交并上传。
2. 将示例文件更新到版本 2，再次提交并推送。

Git 会保留这两次提交的历史。文件夹通过里面的文件一起上传；空文件夹不会被 Git 单独记录。

## 日常上传与更新

在终端执行：

```bash
cd /home/robot/my_projects
git status
git add .
git diff --cached
git commit -m "说明本次修改"
git push
```

`git diff --cached` 用于检查即将上传的内容。确认后再执行提交与推送。没有修改时，无需再次提交。

## 同步 GitHub 上的更新

在开始本次修改之前，确保本地修改已提交，然后执行：

```bash
cd /home/robot/my_projects
git pull --ff-only
```

## 在 VS Code 中操作

打开 `/home/robot/my_projects`，进入左侧“源代码管理”，查看修改、暂存、填写提交说明并提交，然后选择推送。
