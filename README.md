# 2026-04-22-codex

这是一个用于双电脑同步的 Git 项目仓库。

## 这个仓库是做什么的

你可以在电脑 A 和电脑 B 上都使用这个仓库，通过 GitHub 同步项目文件。

推荐使用方式：

1. 两台电脑都安装 Git。
2. 两台电脑都把这个仓库克隆到本地。
3. 开始工作前先拉取最新内容。
4. 修改完成后提交并推送到 GitHub。

## 仓库地址

GitHub:

`https://github.com/xm64400795-collab/2026-04-22-codex.git`

## 第二台电脑如何接入

先打开 PowerShell，然后执行：

```powershell
cd D:\work
git clone https://github.com/xm64400795-collab/2026-04-22-codex.git
```

执行完成后，你会得到本地项目目录：

```text
D:\work\2026-04-22-codex
```

以后就在这个目录里工作。

## 每次开始工作前

进入项目目录：

```powershell
cd D:\work\2026-04-22-codex
```

拉取最新代码：

```powershell
git pull
```

## 每次修改完成后

先查看状态：

```powershell
git status
```

加入本次修改：

```powershell
git add .
```

提交修改：

```powershell
git commit -m "写一句这次改了什么"
```

推送到 GitHub：

```powershell
git push
```

## 最常用的四个命令

```powershell
git pull
git add .
git commit -m "本次修改说明"
git push
```

你可以把它理解成：

- `git pull`：先拿到最新版本
- `git add .`：把这次改动加入提交范围
- `git commit -m "..."`：保存一次修改记录
- `git push`：上传到 GitHub

## 使用规则

- 同一时间尽量只在一台电脑上改同一个文件。
- 开工前先执行 `git pull`。
- 改完后记得执行 `git push`。
- 不要把密码、密钥、隐私配置直接提交到仓库。

## 建议放进仓库的内容

- 源代码
- 文档
- 脚本
- 图片素材
- 配置模板

## 不建议提交的内容

- `node_modules/`
- `.venv/`
- `.env`
- 日志文件
- 构建缓存

这些内容已经在 [`.gitignore`](C:\Users\Administrator\Documents\Codex\2026-04-22-codex\.gitignore) 里做了基础排除。
