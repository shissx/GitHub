
# Gihub 学习日记


# 2024-06-25
## NAS
NAS apps，新建仓库，已经放了这么久了！

# 2026-03-07
## 网页汉化
油猴网站
https://www.tampermonkey.net/index.php?browser=chrome&locale=zh

汉化脚本
https://github.com/maboloshi/github-chinese

直接安装
https://www.tampermonkey.net/script_installation.php#url=https://github.com/maboloshi/github-chinese/raw/gh-pages/main.user.js


## 分支提交
网页修改README.md，新开分支（Branch），然后写描述后提交（Commit）
挺好，先理解为复制备份了一份，并且写了个简单的复制说明

## GitHub Desktop
下载安装GitHub Desktop并汉化

### 帮助
https://docs.github.com/zh/desktop

### 官方版
https://desktop.github.com/
https://github.com/desktop/desktop
GitHubDesktopSetup-x64.exe

默认不支持中文，汉化插件
https://github.com/cngege/GitHubDesktop2Chinese
GitHubDesktop2Chinese.exe


### 社区版
https://github.com/zetaloop/desktop

一个开源的基于 Electron 的 Git 客户端，支持多平台，相比插件汉化的更彻底一些，支持自动更新
Win客户端下载地址
https://github.com/zetaloop/desktop/releases/tag/release-3.5.4
GitHubDesktop-Windows-x64.exe

### 本地提交
登录GitHub Desktop，拉取仓库（Repository）到本地（Clone仓库，pull最新），修改代码，显示差异（类似文本历史版本的对比）
填写描述，提交到main（上传到仓库并合并，Commit，push分支），提示上传成功

网页查看确认完成，微调Markdown语法错误，提交修改

Desktop本地拉取有1个变动，本地不存在，执行拉取origin，成功后刷新仓库，显示无本地改动
编辑本次的网页和本地操作记录，重新填写描述后，上传仓库

# 2026-03-08

## 安装Git
用于GitHub Desktop的补充和自动化操作
https://git-scm.com/install/windows
Git-2.53.0-64-bit.exe
### `常用命令`
### 暂存提交
```
# 1. 查看当前状态（确认修改的文件）
git status
# 应该显示：modified: README.md

# 2. 查看具体修改内容
git diff
# 显示您添加的"常用命令"部分

# 3. 添加文件到暂存区
git add README.md

# 4. 查看已暂存的修改（确认要提交的内容）
git diff --staged
# 应该显示同样的修改内容

# 5. 提交修改
git commit -m "日常更新"

# 6. 推送到远程仓库
git push
```

### 直接提交
```
# 1. 查看当前状态
git status
# 应该显示：modified: README.md

# 2. 查看具体修改内容
git diff
# 确认修改内容

# 3. 直接提交所有已跟踪文件的修改（跳过暂存区）
git commit -a -m "日常更新"
# 或者
git commit -am "日常更新"

# 4. 推送到远程仓库
git push
```

### 直接提交示例
```
git status
git diff
git commit -am "日常更新"
git push
```

### 最简提交示例
```
git commit -am "日常更新"
git push
或
git commit -am "日常更新" && git push
或
git commit -am "日常更新"; git push
或，简单不加引号
git commit -am 日常更新
git push
```

### 撤回提交
```
# 撤回最近一次提交，但保留修改（文件回到工作区）
git reset --soft HEAD~1
# 撤回最近2次提交，保留修改
git reset --soft HEAD~2
```
### 强制推送
```
# 强制推送（覆盖远程）
git push --force

# 或者更安全的强制推送
git push --force-with-lease
```

## 安装VsCode
安装中文插件
可以在GitHub Desktop中链接打开代码文件夹
安装Markdown预览
可以在VsCode中预览Markdown
Markdown All in One
Ctrl+K，V
