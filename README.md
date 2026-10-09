# myskills

个人 Agent Skills 仓库。每个一级子目录都是一个独立技能，目录内的 `SKILL.md` 是技能的入口文件。

把本仓库地址交给支持 Agent Skills 的 AI，并说明要安装的技能名称即可。例如：

> 请从 `https://github.com/johntommasi/myskills` 安装 `geography-worksheet-maker` skill。

也可以使用 Skills CLI 按目录名安装：

```bash
npx skills add johntommasi/myskills --skill <技能目录名>
```

如果 AI 使用的工具不支持 Skills CLI，请让它将指定技能目录完整复制到该工具的技能目录，并保留 `SKILL.md` 及其所有附属文件。

## 技能目录

| 安装名 | 用途 |
| --- | --- |
| `geography-worksheet-maker` | 根据本地规范、教材和固定 DOCX 模板制作高中地理教学材料；支持学案、限时练、教案及教学记录表。 |
| `find-skills` | 当需要扩展能力时，帮助 AI 在开放技能生态中查找、比较并安装合适的技能。 |
| `grill-me` | 用系统化追问检验方案、决策或想法，厘清前提、约束、分支和成功标准。其内部触发名为 `grilling`。 |
| `six-seat-council` | 通过战略、风险、逻辑、认知偏差、执行和伦理六个视角讨论议题，识别分歧并形成可行动建议；最终决定由用户作出。 |

## 给 AI 的安装说明

1. 读取目标技能目录中的 `SKILL.md`，确认适用场景和所需资源。
2. 复制或安装整个目标目录，而不是只复制 `SKILL.md`；部分技能包含 `agents/`、`references/` 等辅助文件。
3. 安装后重新开启一次 AI 会话，使技能被重新发现。

## 维护约定

- 一个一级目录对应一个独立技能，目录名称即推荐安装名。
- 每个技能必须包含带 YAML 元数据的 `SKILL.md`。
- 添加、更新技能后，请更新本 README 的技能目录表并提交变更。
