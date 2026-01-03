# 验收模板（T-*）引用方式

> 强制来源：`附件/附件3-验收标准.md`。

## 1. 模板说明
附件3定义了验收模板（如 T-CRUD/T-LIST/T-CREATE/T-UPDATE/T-DELETE/T-AUTH/T-NOTIFY/T-IMPORT/T-EXPORT/T-REPORT/T-SCHEDULE/T-GENERAL）。

## 2. 单条需求文件的验收写法
在每个 `req-Rxx-xxx.md` 中：
1. 必须标注该需求对应的验收模板（以附件3映射表为准）。
2. 必须给出可执行的验收用例（至少覆盖：权限校验、school_id 隔离、审计要求（如适用）、分页限制（列表类））。
3. 可补充该需求的特定边界（例如撤回、延时、审核流等），但不得引入合同范围外的新流程。

## 3. 通用门禁（所有模板默认叠加）
- 租户隔离（school_id）
- 权限校验（RBAC/ABAC）
- 审计/日志（如适用）
- 输入校验（UUID/必填字段/格式）
- 列表分页 `limit<=100`
