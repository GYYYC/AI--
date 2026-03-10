# AI 工具入门与实操教程

> 我也希望国内的AI更厉害，这样我们也不用费这么大劲儿去使用国外的AI。当然现在国内的AI也有很不错的，比如 MinMax 模型、GLM 模型、DeepSeek 也可以的。

---

## 一、准备工作

### 1. 科学上网（梯子）

梯子是必要的。GitHub 或 CSDN 里面都有介绍，想进入 GitHub 但进不去的可以下载 **Steam++**：
- 官方网址：<https://steampp.net/>

### 2. 注册 Google 账号

有了梯子之后，我们要注册 Google 账号。目前最有效的方法就是在**手机版 Gmail** 里面注册，用国内手机号就可以（但手机要有梯子和 Gmail）。

### 3. 推荐的 AI 工具

现在最稳定且低成本可享用的是谷歌旗下的：
- **Gemini**（网页版）
- **Antigravity**（IDE，可操作本地文件）
- **OpenCode**（CLI，可操作本地文件）
- **GitHub Copilot**（CLI，可操作本地文件）

### 4. 低成本操作指南

要保证自己的谷歌会员是 **Pro 版本**：

1. 查看自己的谷歌账号是否有学生认证资格：<https://one.google.com/ai-student?hl=en-US>
2. 如果没有，可以联系我进谷歌的家庭组，也可以在网上自己找家庭组
3. 如果有钱就自己充值，每月 20💲
4. 也可以白嫖 Google AI Studio：<https://aistudio.google.com/>（支持最新版模型，额度应该够日常使用）

### 5. 准备 GitHub 账号

挂上梯子正常注册就行，谷歌或 QQ 邮箱都可以。如果是大学生也可以进行**学生认证**，可以在 B 站搜索"GitHub 学生认证教程"，国内大学也可以认证（如果实在不行可以来问我）。

### ✅ 准备工作总结

现在我们具备的条件：
1. ✅ 科学上网环境
2. ✅ 谷歌 Pro 账号
3. ✅ 学生认证过的 GitHub 账号

---

## 二、日常教学

> **声明**：我希望大家可以把 AI 真正地运用起来，而不是简单地把它当作高级百度。
>
> 记住：**AI 决定人类的下限，但上限由你来决定。** 所以 AI 并不能缩小人与人之间的差距，反而会扩大差距。

---

## 三、Gemini 篇

### 3.1 推荐插件

推荐下载 Gemini 的网页版插件 **Gemini Voyager**：
- 官网：<https://voyager.nagi.fun/>
- 插件功能在官网有详细介绍

### 3.2 临时对话

因 Gemini 有记忆模式，平常用来提问简单问题或与之前主题差异较大时，可以打开**临时对话**进行简单问答。

### 3.3 Gem（智能体）

可以把 Gem 想象成豆包中的智能体，你可以对它进行角色设定（System Instructions）。

**示例用法**：想学某技能 → 在临时对话中让 AI 给你一个精通该技能的老师的 System Instructions（Prompt）。

**全局 Prompt 设置**：
- Gemini 左下角 → 设置与帮助 → 个人使用场景 → 向 Gemini 提供指令 → 点击添加

> 💡 **我对 System Instruction 的理解**：我们平常为了让 AI 回答符合预期，通常会在提问时控制 AI 的回答方式。但每次这样做很麻烦，所以引入了 System Instruction 这个功能。

### 3.4 其他功能

- **文件上传**：对话框中的 ➕ 能添加文件（文字和视频）
- **NotebookLM**：<https://notebooklm.google.com>
  - 适用场景：系统性学习一项技能时，搜索相关文献和网址，提交给 AI 进行深度理解
  - 优势：减少 AI 幻觉（少说假话），右侧 Studio 模块可进行内容可视化
  - 特别适合：老师教学、做 PPT

### 3.5 内置工具

| 工具 | 说明 |
|------|------|
| **Nano Banana** | 制作图片 |
| **Canvas** | 代码可视化（最常用） |
| **Deep Research** | 深度挖掘数据和文献 |
| **制作视频** | 视频生成 |
| **学习辅导** | 辅助学习 |

### 3.6 Canvas（重点推荐）

Canvas 可以将代码直接可视化。比如写一个前端代码，完成后可以**直接展示前端界面**，而不用手动保存为 `.html` 再运行。

> **小技巧**：如果对话一段时间后 Gemini 不按提示走，拿着最后版本的代码**另起一个对话框**，把代码和要求重新输入。写代码时最好把对话框右下角切换成 **Pro 或思考模式**。

### 3.7 Deep Research

它不再是"问答机器人"，而是通过模拟导师的教学方法，引导你从"得到答案"转向"理解概念"，适合学生和老师。

---

## 四、OpenCode 篇

### 4.1 下载安装

可以下载 Desktop 版本或 CLI 版本：
- GitHub 仓库：<https://github.com/anomalyco/opencode>（含介绍、安装包、CLI 下载方法）

### 4.2 基础操作

| 操作 | 说明 |
|------|------|
| `Tab` 键 | 切换 Plan / Build 模式 |
| Plan 模式 | 不会更改文件，先用来沟通几轮 |
| Build 模式 | 可修改/创建本地文件 |
| `/models` | 选择模型 |
| `/new` | 新建对话 |
| `/sessions` | 选择历史对话 |
| `Ctrl+P` | 选择诉求 |

### 4.3 模型选择

OpenCode 内置了 **MinMax M2.5** 和 **Kimi 2.5** 两个模型。如果需要顶级模型（Claude、Gemini、GPT），需要用 **Antigravity Tools** 进行 API 反代。

### 4.4 配置 Antigravity Tools 反代

1. 在 GitHub 搜索 Antigravity Tools：<https://github.com/lbjlaq/Antigravity-Manager>
   - 右侧 Releases 中找安装包（不知道下载哪个可以截图问 Gemini）
2. 登录 Pro 资格的 Google 账号
3. 导航栏 → API 反代 → 找到 API 密钥
4. 打开或创建 `opencode.json`（路径一般为 `C:\Users\用户\.config\opencode\opencode.json`）
5. 粘贴以下配置：

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "AntigravityTools": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "Antigravity Local",
      "options": {
        "baseURL": "http://127.0.0.1:8045/v1",
        "apiKey": "这个地方粘贴你的API密钥"
      },
      "models": {
        "gemini-3-pro-high": { "name": "Gemini 3 pro High" },
        "gemini-3.1-pro-high": { "name": "Gemini 3.1 Pro High" },
        "gemini-3-flash": { "name": "Gemini 3 Flash" },
        "claude-sonnet-4-6": { "name": "Claude 4.6 Sonnet" },
        "claude-sonnet-4-6-thinking": { "name": "Claude 4.6 Sonnet (Thinking)" },
        "claude-opus-4-6-thinking": { "name": "Claude 4.6 Opus (Thinking)" }
      }
    }
  }
}
```

6. `Ctrl+S` 保存
7. 在 Antigravity Tools 的 API 反代页面顶部点击**启动服务**
8. 在 OpenCode 中输入 `/models` → 找到 **Antigravity Local** → 选择模型

### 4.5 oh-my-opencode 插件（多 Agent 并行）

**简介**：可以想象成一个 CEO——你提出要求后，由 **Sisyphus** 进行问题拆解分配给其他 AI 助手，多个 AI 并行解决各自擅长的问题。

**安装方法**：在 OpenCode 对话框中输入：

```
Install and configure oh-my-opencode by following the instructions here:
https://raw.githubusercontent.com/code-yeongyu/oh-my-opencode/refs/heads/dev/docs/guide/installation.md
```

安装时它会问你有没有 Anthropic（Claude）或 OpenAI（GPT）的会员，都选**否**（我们有 Antigravity Tools 反代）。

安装后会在 OpenCode 文件夹下生成 `oh-my-opencode.json` 配置文件：

```json
{
  "$schema": "https://raw.githubusercontent.com/code-yeongyu/oh-my-opencode/master/assets/oh-my-opencode.schema.json",
  "agents": {
    "sisyphus": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "max" },
    "hephaestus": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "medium" },
    "oracle": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "high" },
    "librarian": { "model": "AntigravityTools/gemini-3-flash" },
    "explore": { "model": "AntigravityTools/claude-sonnet-4-6" },
    "prometheus": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "max" },
    "metis": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "max" },
    "momus": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "medium" },
    "atlas": { "model": "AntigravityTools/gemini-3-flash" }
  },
  "categories": {
    "visual-engineering": { "model": "AntigravityTools/gemini-3.1-pro-high" },
    "ultrabrain": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "xhigh" },
    "deep": { "model": "AntigravityTools/claude-sonnet-4-6", "variant": "medium" },
    "artistry": { "model": "AntigravityTools/gemini-3.1-pro-high", "variant": "high" },
    "quick": { "model": "AntigravityTools/gemini-3-flash" },
    "unspecified-low": { "model": "AntigravityTools/gemini-3-flash" },
    "unspecified-high": { "model": "AntigravityTools/claude-sonnet-4-6" },
    "writing": { "model": "AntigravityTools/gemini-3-flash" }
  }
}
```

`Ctrl+S` 保存即可。

---

## 五、Skills 与 MCP

### 5.1 Skills 配置（以 OpenCode 为例）

不同 CLI 的 Skills 配置方式不同。以 **ui-ux-pro-max**（前端编写 Skill）为例：

1. GitHub 仓库：<https://github.com/nextevelbuilder/ui-ux-pro-max-skill>
2. 安装步骤：
   - 终端（Win+R → cmd）输入：`npm install -g uipro-cli`
   - `cd /path/to/your/project`（例如 `cd C:\Users\28997`）
   - `uipro init --ai opencode`
3. 安装后在 `.opencode/skills/ui-ux-pro-max` 下应该能找到 `SKILL.md`

> **关键要求**：不同 CLI 的配置文件中需要创建 `skills` 文件夹，该文件夹中必须有 `SKILL.md` 才算成功安装技能。
>
> 也可以自己编写 Skills，或者直接将诉求告诉 Gemini 让它帮你生成。

### 5.2 我对 Skills 的理解

Skills 本质上是从 Prompt 演变而来的：

| 阶段 | 说明 |
|------|------|
| **初级** | 写大量标准且准确的长 Prompt，效率极低 |
| **中级** | System Prompt（预设人设面具），死板缺乏灵活性 |
| **高级** | Skills —— 按需加载，用多少拿多少 |

> 💡 **渐进式披露（Progressive Disclosure）**：给 Agent 装了 50 个 Skills 不会一次性全部读完。只有当 AI 判断当前任务需要某项技能时，相关指令才会进入上下文。既节省了 Token，也保住了 AI 的专注力。

### 5.3 我对 MCP 的理解

**MCP（Model Context Protocol）= AI 界的 "USB 接口标准"**

在 MCP 出现之前，让 AI 连接 GitHub、Google Drive 或本地数据库，每个软件都需要编写专属的"翻译代码"。有了 MCP，只要插件符合标准，AI 就可以**直接"盲插"并无缝调用**外部数据。

> 如果说 **Skills** 是赋予 AI 的"认知补丁"（教它怎么想），那么 **MCP** 就是 AI 的"物理接口"（让它能碰到数据）。它们一个优化了大脑效率，一个打通了四肢连接，共同把 AI 从"聊天框"变成了"行动派"。

### 5.4 OpenCode 中的 MCP 配置

**方法一：交互式命令**

```bash
opencode mcp add
```

以 GitHub MCP 为例，你需要先在 GitHub → Settings → Developer Settings 创建 **Personal Access Token**（选第二个，勾选 repo 相关权限）。

命令会引导你填写：
1. MCP 类型：`local`（本地命令）还是 `remote`（远程 URL）
2. 名称：如 `github`
3. 命令：如 `npx -y @modelcontextprotocol/server-github`
4. 环境变量：输入 token 等密钥

**方法二（推荐）：手动编辑 opencode.json**

把 `opencode.json` 文件交给 AI，让它帮你配置所需的 MCP，格式不会出错。

验证是否配置成功：
- 在 OpenCode 输入 `/mcp` 查看
- 或终端输入 `opencode mcp ls`

### 5.5 OpenCode 中的 Agent

在终端输入 `opencode agent create`，或把定义和需求连同 `opencode.json` 交给 AI 让它配置。`Tab` 键可切换 Agent。

---

## 六、GitHub Copilot（副驾驶）篇

> 前提：建议完成 GitHub 学生认证。没有的可以在 B 站搜索教程。

### 6.1 安装

- CLI 安装：<https://github.com/features/copilot/cli>
- 完整文档：<https://docs.github.com/en/copilot/how-tos/copilot-cli/cli-best-practices>

### 6.2 MCP 配置

**方法一（推荐）：交互式命令**

启动 Copilot 后输入：

```
/mcp add
```

用 `Tab` 在字段间切换填写 MCP 服务器信息，`Ctrl+S` 保存（`mcp-config.json` 会自动生成）。

**方法二：手动创建配置文件**

创建 `C:\Users\用户\.copilot\mcp-config.json`：

```json
{
  "mcpServers": {
    "my-server": {
      "command": "npx",
      "args": ["-y", "@some/mcp-server"],
      "env": {
        "API_KEY": "your-key"
      }
    }
  }
}
```

### 6.3 Skill 配置

#### 创建步骤

1. **创建目录**：
   - 个人 Skill（跨项目通用）：`~/.copilot/skills/<skill-名称>/`
   - 项目 Skill（仅当前仓库）：`.github/skills/<skill-名称>/`

2. **创建 `SKILL.md` 文件**（可以让 AI 帮你生成内容）：

```markdown
---
name: my-skill-name
description: 描述这个 skill 做什么，以及 Copilot 什么时候应该使用它。
---

## 指南

这里写给 Copilot 的具体指令、示例和规则...
```

3. **可选**：在同一目录下添加脚本或资源文件

#### 管理命令

| 命令 | 作用 |
|------|------|
| `/skills list` | 列出所有可用 Skills |
| `/skills` | 开启/关闭特定 Skill |
| `/skills info` | 查看 Skill 详情和路径 |
| `/skills reload` | 重新加载（无需重启 CLI） |
| `/skills remove <目录名>` | 删除 Skill |

#### 使用 Skill

- **显式调用**：在提示词中用 `/skill名称`
- **自动调用**：直接描述任务，Copilot 根据 description 自动判断

### 6.4 常用命令

```bash
copilot -h                  # 命令行帮助
copilot help TOPIC          # 主题帮助（config/commands/permissions 等）
/help                       # CLI 内帮助
/usage                      # 查看使用统计
/feedback                   # 提交反馈/报 Bug
```

### 6.5 推荐工作流

```
探索 → /plan → 审查计划 → 实现 → 验证测试 → 提交
```

善用 `/plan`（规划复杂任务）、`/delegate`（异步委托）、`/fleet`（并行加速），`Shift+Tab` 切换模式。

> **Tips**：CLI 可以读取本地文件，直接给文件地址就会自动找到并操作。
>
> Copilot 的 token 消耗按**回答次数**计费，不论为了回答消耗了多少 token，只按次数算。内置模型可通过 `/model` 选择。

---

## 七、Antigravity 篇

> 详细文档：<https://antigravity.google/docs/get-started>（不明白的截图发给 AI 讨论）

### 7.1 Skills

Antigravity 中没有显式命令去调用 Skills（OpenCode、Copilot 可以用 `/skill`），但只要在 `C:\Users\用户\.gemini\antigravity\skills\` 下有规范的 Skill，Antigravity 就会通过**渐进式披露**自动使用。

也可以显式提及，例如："使用 ui-ux-pro-max 来..."

| 类型 | 路径 | 说明 |
|------|------|------|
| 全局 Skill | `~/.gemini/antigravity/skills/<skill>/` | 所有对话/项目可用 |
| 项目 Skill | `<项目>/.agent/skills/<skill>/` | 仅当前项目可用 |

### 7.2 MCP 配置

**方法一：内置 MCP Store（推荐）**

1. 点击编辑器侧边栏顶部的 `...` 下拉菜单
2. 打开 **MCP Servers** 面板
3. 浏览并点击 Install 安装
4. 按提示完成账号授权

> ⚠️ GitHub MCP 需要在 **Docker** 运行的前提下才能连接。

**方法二：手动编辑配置文件**

`...` 下拉 → Manage MCP Servers → View raw config，或直接编辑 `C:\Users\用户\.gemini\antigravity\mcp_config.json`（不会配置就问 AI）。

### 7.3 Workspace（工作区）

| 概念 | 说明 |
|------|------|
| 工作区 | Agent Manager 支持同时管理多个工作区，每个对应一个文件夹 |
| 打开新工作区 | 点击左侧边栏按钮，选择文件夹作为根目录 |
| 切换工作区 | 通过左侧边栏切换（最上面偏右有 Open Agent Manager） |

> 💡 **核心概念**：工作区 = 文件夹。一个工作区可以有多个对话，多个工作区可以同时运行。可以对同一项目开两个窗口同时处理。

### 7.4 Rules（规则）

手动定义的约束条件，引导 Agent 遵循特定行为、风格和技术栈偏好。本质是 Markdown 文件，限制 12,000 字符。

| 类型 | 路径 |
|------|------|
| 全局 | `~/.gemini/GEMINI.md` |
| 工作区 | `.agent/rules/`（工作区或 Git 根目录） |

**创建方式**：`...` 下拉 → Customizations → Rules → `+ Global` 或 `+ Workspace`

**激活方式**：

| 方式 | 说明 |
|------|------|
| Manual | 在输入框中 `@提及` 手动激活（推荐） |
| Always On | 永远生效（推荐） |
| Model Decision | AI 根据自然语言描述自行判断是否应用 |
| Glob | 匹配文件模式时自动应用（如 `*.js`、`src/**/*.ts`） |

### 7.5 Workflows（工作流）

定义一系列步骤，引导 Agent 完成重复性任务（如部署、处理 PR 评论）。也是 Markdown 文件，限制 12,000 字符。

- 与 Rules 存放位置相同，分全局和工作区两级
- **创建**：`...` 下拉 → Customizations → Workflows
- **执行**：在输入框中使用 `/workflow-name`

**高级特性**：
- 嵌套调用：`/workflow-1` → 调用 `/workflow-2` → 调用 `/workflow-3`
- AI 自动生成：手动操作完一系列步骤后，让 Agent 根据对话历史生成 Workflow

> 💡 **建议**：Rules 和 Workflows 都和 AI 商量着写，只要你的 Prompt 足够清晰。不够清晰也没关系，和 AI 对话几轮迭代之后就好了。**不要和 AI 比脑子，你有的只有你的判断力。**

### 7.6 Agent 模式与设置

#### 对话级别模式

| 模式 | 适用场景 |
|------|----------|
| **Planning** | 深度研究、复杂任务、协作工作 |
| **Fast** | 简单任务（改变量名、跑几条命令等） |

#### 全局设置（Settings → Agent 标签页）

**Artifact Review Policy（产物审查策略）**

| 选项 | 说明 |
|------|------|
| Request Review | Agent 规划完成后等你审查 |
| Always Proceed | 规划完直接执行，无需审查 |

**Terminal Command Auto Execution（终端命令自动执行）**

| 选项 | 说明 |
|------|------|
| Request Review | 需要审查 |
| Always Proceed | 自动执行 |

- **Allow List / Deny List** 可在设置中自定义
- 示例：`Request Review` + Allow List 加入 `git status` → 其他命令要审查，`git status` 直接执行
- 示例：`Always Proceed` + Deny List 加入 `rm -rf` → 其他自动执行，`rm -rf` 需审查

**匹配规则**：

| Shell 类型 | 匹配方式 | 示例 |
|-----------|---------|------|
| Unix Shell | 前缀匹配 | 配置 `git` → 匹配 `git commit` ✅，不匹配 `npm run git` ❌ |
| PowerShell | 任意连续子序列匹配 | 配置 `push origin` → 匹配 `git push origin main` ✅ |

**Agent Non-Workspace File Access（工作区外文件访问）**

默认只能访问当前工作区和 `~/.antigravity/`。开启后可读写工作区以外的文件，**谨慎使用**。

### 7.7 Command（代码编辑快捷键）

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+I` | 选中代码后用自然语言指令修改（生成/修改代码） |
| `Ctrl+L` | 选中代码/文字后与智能体对话（询问/讨论） |

**使用流程**：
1. 光标放在目标位置
2. 按快捷键 → 弹出输入框
3. 用自然语言输入需求
4. AI 直接在当前位置生成内容
5. 审查后决定是否接受

### 7.8 Source Control（版本控制）

位于 Antigravity 最左侧一栏（Logo 像 Y），有两个选项：
- **Initialize Repository**：初始化本地仓库
- **Publish to GitHub**：发布到 GitHub

**为什么要用 Source Control**：
- 项目需要多次迭代，每次 commit 都有记录
- 可以随时查看上次的更改
- 每次提交时写 `COMMIT_EDITMSG`（第一行写更改原因或目的）
- 修改好后点击 ✓ 提交

> ⚠️ 连接 GitHub MCP 需要 Docker 运行 + GitHub Token 权限足够。
>
> 💡 每次更新项目都建议 commit，这样以后找之前的版本都有记录。
