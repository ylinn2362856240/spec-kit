# 在 Trae 中测试和使用 Spec Kit 和 Specify

## 1. 安装 Specify CLI

首先，你需要安装 Specify CLI 工具：

```bash
# 推荐的持久安装方式
uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
```

## 2. 初始化项目（使用 Trae 作为 AI 代理）

在 Trae 中，你可以使用以下命令初始化项目：

```bash
# 在当前目录初始化项目，使用 Trae 作为 AI 代理
specify init --here --ai trae

# 或者创建新项目
specify init my-project --ai trae
```

## 3. 开始使用 Spec-Driven Development 流程

初始化完成后，你可以在 Trae 中使用以下命令开始开发流程：

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

## 4. 验证安装和工具

你可以使用以下命令检查系统要求和已安装的工具：

```bash
specify check
```

## 5. Trae 相关配置

Trae 作为基于 IDE 的代理，会在项目中创建 `.trae/rules/` 目录来存储命令文件。

## 6. 开发流程说明

Spec-Driven Development 是一个结构化的过程，强调：

- 意图驱动的开发，先定义"做什么"再定义"怎么做"
- 使用护栏和组织原则创建丰富的规范
- 多步骤细化而不是一次性代码生成
- 依靠先进的 AI 模型能力进行规范解释

## 7. 可用的命令

在 Trae 中，你可以使用以下核心命令：

| 命令                    | 描述                                   |
| ----------------------- | -------------------------------------- |
| `/speckit.constitution` | 创建或更新项目治理原则和开发指南       |
| `/speckit.specify`      | 定义你想要构建的内容（需求和用户故事） |
| `/speckit.plan`         | 使用你选择的技术栈创建技术实现计划     |
| `/speckit.tasks`        | 生成可操作的任务列表用于实现           |
| `/speckit.implement`    | 执行所有任务，根据计划构建功能         |

## 8. 示例工作流

1. **初始化项目**：`specify init --here --ai trae`
2. **创建项目原则**：`/speckit.constitution 专注于代码质量和用户体验`
3. **定义需求**：`/speckit.specify 构建一个简单的待办事项应用，支持添加、编辑、删除任务`
4. **技术规划**：`/speckit.plan 使用 HTML、CSS 和 JavaScript，本地存储数据`
5. **分解任务**：`/speckit.tasks`
6. **实现功能**：`/speckit.implement`

通过这种结构化的流程，你可以在 Trae 中高效地使用 Spec Kit 和 Specify 进行规范驱动开发。
