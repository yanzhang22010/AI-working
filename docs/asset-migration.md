# AI 资产迁移清单

来源：内容中心 UED AI 资产指引及内容中心 UED Skills 库。保留许可已经由资产所有方确认。

## 已建立的个人库结构

| 范围 | 原始资产 | 个人库位置 | 状态 |
| --- | --- | --- | --- |
| 体验流程 | `ux-requirements` | `skills/ux-requirements` | 待导入原件 |
| 需求检查 | `spec-review` | `skills/spec-review` | 待导入原件 |
| 需求澄清 | `spec-clarify` | `skills/spec-clarify` | 待导入原件 |
| 设计策略 | `design-strategy` | `skills/design-strategy` | 待导入原件 |
| 概念原型 | `concept-prototype-v5` | `skills/concept-prototype-v5` | 待导入原件 |
| UX 评审 | `design-review` | `skills/design-review` | 待导入原件 |
| 国际化 UI 评审 | `global-ui-review` | `skills/global-ui-review` | 待导入原件 |
| UX 文案 | `ux-copywriting-analyzer` | `skills/ux-copywriting-analyzer` | 待导入原件 |
| 竞品分析 | `competitive-analysis` | `skills/competitive-analysis` | 待导入原件 |
| 交付前检查 | `l-precheck` | `skills/l-precheck` | 待导入原件 |
| Figma 动效 | `figma-motion-video` | `skills/figma-motion-video` | 待导入原件 |
| UI 生成 | `ui-generation-workflow` | `skills/ui-generation-workflow` | 待导入原件 |
| 业务流程 | Trip.Planner LUI Pipeline | `skills/trip-planner-lui-pipeline` | 待导入原件 |
| 知识资产 | AI Showcase / 飞书 / AgentArk | `knowledge/` | 待按主题导入 |

## 导入规则

每次从原始仓库导入一个 Skill 时，保留其 `SKILL.md`、被引用的模板、脚本和参考文件；同时在该目录增加 `SOURCE.md`，写明原始链接、版本或提交、导入日期及需要替换的外部依赖。

## 本地运行边界

- 不保存公司账号、访问 Token、MCP 配置或 SSH 私钥。
- 业务知识库、组件库和设计稿按个人许可范围导入。
- 如某个 Skill 依赖内部设计系统或知识库，应在 `SOURCE.md` 说明其个人替代方案。
