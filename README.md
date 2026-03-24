# AI PM Career Kit

一个公开可分发的 AI 产品经理求职与方法论模板包。

这个仓库只保留可公开分享的内容：

- `resume/ai-pm-resume-template.md`
- `interview/ai-pm-interview-master-template.md`
- `.cursor/skills/ai-product-0to1-playbook/SKILL.md`

## 这个仓库适合谁

- 正在准备 `AI 产品经理` / `AI Native 产品经理` 求职的人
- 想把简历和面试表达做得更产品化的人
- 想把 “AI 产品从 0 到 1” 流程沉淀成可复用 skill 的人

## 不包含什么

- 不包含 `Saytype` 相关内容
- 不包含私有项目资料、私有链接、内部文档
- 不包含个人手机号、邮箱等隐私信息

## 30 秒开始

把下面这整段直接发给 `Claude Code`，不要拆开：

```text
你现在是我的“安装助手 + 产品教练”。

请用最少操作帮我把这个公开仓库接入到我的 Cursor，并在接入完成后继续像产品教练一样带我从想法走到网站上线。

仓库地址：
https://github.com/MagicalAci/ai-pm-career-kit-public

工作原则：
1. 先自己检查当前环境，不要一开始就丢给我一堆命令
2. 优先用最省步骤的方案自动完成
3. 这是公开仓库，所以如果我没有 GitHub 账号，不要先让我注册；能直接拉取就直接拉取
4. 只有在必须人工操作时，才告诉我下一步，而且一次只给我一个动作
5. 每次回复开头先告诉我：
   - 当前阶段
   - 当前进度
   - 你现在在做什么
   - 如果需要我配合，我只需要做哪一件事

请按下面顺序执行：
A. 检查这台机器是否有 git、curl、unzip、Cursor CLI
B. 如果本地已经有这个仓库，直接更新；如果没有：
   - 有 git 就 clone 到一个合理位置，优先 `~/Downloads/ai-pm-career-kit-public`
   - 没有 git 就直接下载仓库 zip 并解压
C. 检查 `~/.cursor/skills/ai-product-0to1-playbook` 是否已存在；如果没有，就从仓库里复制过去
D. 如果能直接用 `cursor` 命令打开仓库，就帮我打开；如果不能，就告诉我最短的手动打开方式
E. 打开后，读取仓库里的 `START-HERE-build-your-website.md`，然后进入“产品教练模式”，带我继续推进做网站

额外规则：
- 不要因为没有 GitHub 账号就停住，这个仓库是公开的
- 如果你判断我后面确实需要 GitHub 账号，例如我要 fork 或同步到我自己的仓库，再引导我创建，并把步骤压到最少
- 如果某个命令失败，自动切换到备选方案，不要把问题直接抛回给我
- 完成环境准备后，不要停，直接进入第一步产品教练流程

现在先开始环境检查，并只推进第一步。
```

如果对方已经把仓库接进 Cursor 了，后面就让她直接看：

`START-HERE-build-your-website.md`

## 如何使用

### 1. 简历

打开 `resume/ai-pm-resume-template.md`，把方括号占位内容替换成你自己的经历。

### 2. 面试自述稿

打开 `interview/ai-pm-interview-master-template.md`，先改成自己的真实经历，再练成口语化版本。

### 3. Skill

这个仓库已经内置了一个 Cursor 项目 skill：

`/.cursor/skills/ai-product-0to1-playbook/SKILL.md`

你有两种用法：

1. 直接在 Cursor 里打开这个仓库，当作项目 skill 使用
2. 把 `ai-product-0to1-playbook` 目录复制到 `~/.cursor/skills/`，当作个人 skill 使用

### 4. 教练式网站搭建

如果你的目标不是“学习方法论”，而是“真的把一个网站搭出来”，请从这里开始：

`START-HERE-build-your-website.md`

它会告诉你：

- 第一步该给 Cursor 发送什么启动指令
- Cursor 每一轮应该怎么告诉你当前进度
- 每个阶段你需要做什么、给什么信息、拿回什么结果
- 怎么从一个模糊想法走到一个真的上线网站

## 建议的使用顺序

1. 先改简历模板
2. 再改面试总稿模板
3. 如果目标是做网站，直接进入 `START-HERE-build-your-website.md`
4. 最后用 skill 去推进自己的项目材料、产品案例或 0-1 产品方案

## 说明

这个仓库是公开安全版模板包，适合直接分发、复用和二次修改。
