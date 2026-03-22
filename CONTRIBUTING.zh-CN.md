# 参与贡献指南

感谢你为 sellabx 做出贡献。
我们致力于构建面向多行业业务关键场景的可扩展工具与基础设施。

## 贡献流程

### 1. Fork

将仓库 Fork 到你自己的 GitHub 账号。

### 2. 创建分支

从 main 创建语义清晰的分支。

- `feat/<short-description>`
- `fix/<short-description>`
- `chore/<short-description>`
- `docs/<short-description>`
- `refactor/<short-description>`

### 3. 开发变更

- 保持改动聚焦且最小化。
- 遵循现有架构与命名模式。
- 行为变化时同步更新文档。

### 4. 使用 Conventional Commits 提交

提交信息必须遵循以下格式：

```text
<type>(<optional-scope>): <short summary>
```

支持的 type：

- feat
- fix
- docs
- refactor
- test
- chore
- ci
- perf

示例：

- feat(api): add tenant-aware rate limiting
- fix(worker): prevent duplicate retry scheduling
- ci(github): cache dependency installation

若包含破坏性变更，请使用 ! 并在提交正文说明：

- feat(auth)!: replace legacy token contract

### 5. 本地校验

发起 PR 前请完成：

1. 运行 lint 检查。
2. 运行单元测试。
3. 运行与改动相关的集成测试。
4. 确认未提交密钥、凭据或敏感信息。

### 6. 发起 Pull Request

向 main 发起 PR，并完整填写 PR 模板。

- PR 标题需符合 Conventional Commits。
- 关联相关 issue，例如 closes #123。
- 对涉及上线风险的改动，附测试证据与发布说明。

### 7. 评审与合并

- 清晰、及时地回应评审意见。
- 保持分支与 main 同步。
- 在通过审批与必要检查后由维护者合并。

## 编码标准

- 编写清晰、可维护、可用于生产环境的代码。
- 优先可读性，避免过度技巧化实现。
- 为关键路径补充确定性测试。
- 请求评审前确保 lint 通过。
- 避免在同一 PR 中混入无关重构。
- 对关键运维路径补充日志与指标埋点。

## Issue 分流流程

所有新 issue 由维护者按以下流程分流：

1. Validate：确认是否具备足够上下文与复现信息。
2. Classify：分类为 bug、feature、question 或 docs。
3. Prioritize：评估业务影响与紧急程度。
4. Route：分配负责人或进入待办队列。
5. Track：更新标签与状态，并同步下一步计划。

优先级建议：

- High：生产故障、数据风险、安全问题、关键稳定性回归
- Medium：有替代方案但影响明显的功能问题
- Low：轻微缺陷、非阻塞增强、文档优化

## 安全问题上报

安全漏洞请勿公开提交 issue。
请按 SECURITY.md 中流程私下上报。

## 社区与行为规范

参与社区即表示你同意遵守 CODE_OF_CONDUCT.md。
