# 在 Antigravity 中使用 Spec Kit 和 Specify

## 1. 安装 Specify CLI

首先，确保你已经安装了 Specify CLI：

```bash
# 推荐的持久安装方式
uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
```

## 2. 初始化项目（使用 Antigravity 作为 AI 代理）

Antigravity 需要使用 `--ai-skills` 标志来安装必要的技能：

```bash
# 创建新项目并使用 Antigravity
specify init my-project --ai agy --ai-skills

# 或者在当前目录初始化
specify init --here --ai agy --ai-skills
```

## 3. 开始使用 Spec-Driven Development 流程

初始化完成后，你可以在 Antigravity 中使用以下命令开始开发流程：

### 步骤 1：建立项目原则

```bash
/speckit.constitution 创建专注于代码质量、测试标准、用户体验一致性和性能要求的原则
```

### 步骤 2：创建规格说明

```bash
/speckit.specify 描述你想要构建的功能，专注于"做什么"和"为什么"，而不是技术栈
```

### 步骤 3：创建技术实现计划

```bash
/speckit.plan 提供你的技术栈和架构选择
```

### 步骤 4：分解任务

```bash
/speckit.tasks
```

### 步骤 5：执行实现

```bash
/speckit.implement
```

## 4. Antigravity 特定配置

- **目录结构**：Antigravity 使用 `.agent/commands/` 目录来存储命令文件
- **技能安装**：必须使用 `--ai-skills` 标志来安装 Spec Kit 技能
- **命令格式**：使用标准的 `/speckit.*` 命令格式

## 5. 验证安装和工具

你可以使用以下命令检查系统要求和已安装的工具：

```bash
specify check
```

## 6. 示例工作流

1. **初始化项目**：`specify init --here --ai agy --ai-skills`
2. **创建项目原则**：`/speckit.constitution 专注于代码质量和用户体验`
3. **定义需求**：`/speckit.specify 构建一个简单的待办事项应用，支持添加、编辑、删除任务`
4. **技术规划**：`/speckit.plan 使用 HTML、CSS 和 JavaScript，本地存储数据`
5. **分解任务**：`/speckit.tasks`
6. **实现功能**：`/speckit.implement`

通过这种结构化的流程，你可以在 Antigravity 中高效地使用 Spec Kit 和 Specify 进行规范驱动开发。
