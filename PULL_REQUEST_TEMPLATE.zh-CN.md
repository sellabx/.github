# Pull Request

## Conventional Commits 合规性

PR 标题必须符合 Conventional Commits：

<type>(<optional-scope>): <summary>

示例：

- feat(api): add tenant-aware throttling
- fix(ci): restore cache fallback behavior

## 1. 变更说明

请说明改了什么，以及为什么改。

## 2. 关联 Issue

请使用关键字关联 issue，例如：

- closes #123
- refs #456

## 3. 测试说明

请描述测试覆盖与结果。

- 单元测试：
- 集成测试：
- 手工验证：

## 4. 变更类型

- [ ] 缺陷修复
- [ ] 新功能
- [ ] 能力增强
- [ ] 文档变更

## 5. 检查清单

- [ ] PR 标题符合 Conventional Commits
- [ ] 已通过 lint 与格式检查
- [ ] 已按需新增或更新单元测试
- [ ] 相关测试已在本地通过
- [ ] 已按需更新文档
- [ ] 未提交密钥或凭据
- [ ] 已评估向后兼容性
- [ ] 高风险变更已说明回滚考虑

## 评审备注

请补充有助于评审判断风险、架构影响与发布安全的信息。
