# 审计日志（Audit Logging）规范

> 强制来源：`附件/01-三橙智星开发团队技术协议与开发规范.md`（审计字段要求）。

## 1. 必须记录的场景
- 集团人员进入学校视角（`X-View-Scope: {school_uuid}`）执行 VIEW/CREATE/UPDATE/DELETE。
- Web 管理端关键管理操作（通常为 CREATE/UPDATE/DELETE/IMPORT/EXPORT/APPROVE）。

## 2. 字段要求（最小集合）
- `operator_id`：操作人 ID
- `operator_name`：操作人姓名
- `target_school_id`：被操作学校 ID
- `action`：VIEW/CREATE/UPDATE/DELETE
- `resource_type`：资源类型
- `resource_id`：资源 ID（如有）
- `trace_id`：链路追踪标识
- `timestamp`：操作时间

## 3. 与单条需求文件的关系
每个 `req-Rxx-xxx.md` 必须明确：
- 是否需要审计（Required/Recommended/Not required）；
- 触发点（查看/新增/修改/删除/导入/导出/审批/驳回/撤回等）；
- 资源类型与关键字段。
