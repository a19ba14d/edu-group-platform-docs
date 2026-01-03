# 单条需求文件模板（req-Rxx-xxx.md）

> 适用：每条叶子需求点【Rxx-xxx】对应一个独立文件，文件名必须为 `req-Rxx-xxx.md`。

# 【Rxx-xxx】<功能名称>
<a id="Rxx-xxx"></a>

- **Requirement ID**：【Rxx-xxx】
- **Feature name**：<功能名称>
- **Source**：<模块 > 子模块 > ... > 叶子节点>
- **Applicable Platform/Entry**：<平台/入口路径描述>
- **User Roles & Permission Requirements**：
  - 可执行角色：<角色列表>
  - 权限点（最小粒度）：`req:Rxx-xxx`
  -（可选）通用权限点：`<resource>:<action>`
  - 视角/范围：<集团/学校视角差异或 N/A>
- **User Stories**：
  - 场景 1：作为<角色>，我希望…，以便…
  - 场景 2：…
- **Business Rules & Boundaries**：
  - <分页/软删/幂等/审核流等>
- **Data Scope（school_id）**：
  - <school_id 隔离与可见范围 + 跨校禁止>
- **Audit Log Requirements**：
  - <Required/Recommended/Not required + 触发点 + 字段>
- **Acceptance Criteria（verifiable）**：
  - 验收模板：`T-*`
  - 验收用例：1) … 2) … 3) …

## 相关需求（See also）
- <链接到同流程/同父节点的其它需求>

## 导航
- 返回模块 README：<module README link>
- 返回平台 README：<platform README link>
- 追溯矩阵：`PRD/traceability-matrix.md`
