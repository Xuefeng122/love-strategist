# 恋爱小助手 · Love Strategist

一个融合系统化分析与直白街头智慧的 AI 恋爱决策 Skill。

## 是什么

不是只会说"勇敢去追"或"赶紧分手"的话术机。它先接住你的情绪，再拆事实、算利弊，最后给能执行的下一步。

两种风格自由切换：

| 模式 | 触发词 | 风格 |
|---|---|---|
| 系统化分析 | 默认 | 结构化、列事实推测未知、给 2-3 个方案 |
| 祖师爷模式 | "童锦程"/"祖师爷怎么看" | 直白口语、短句、先给结论 |

## 能帮你做什么

- 这句消息怎么回？先给一条能直接发的成品，再补后续分支
- 他到底喜不喜欢我？用行为判断，不猜心
- 想追、想复合、想退出？给具体行动方案和停止条件
- 聊天截图太多？锁定说话人，区分事实和脑补
- 多人之间犹豫？分别分析再比较

## 安装

把下面这句话发给你的 AI 助手：

```
请将公开仓库 https://github.com/Xuefeng122/love-strategist 下载并安装为本地 Skill。
```

安装到用户级目录后，Skill 目录应包含 `SKILL.md`、`agents/openai.yaml`、`references/` 与 `scripts/`。

## 使用

装完直接问就行：

```
帮我分析一下这段关系
他对我忽冷忽热，到底什么意思？
童锦程怎么看这件事？
这句话怎么回？
```

第一次用它会问你 MBTI、综合评分、关系背景这些，不知道的可以留空，直接讲故事也行。

## 知识库

内置 20 份跨学科知识文档，按需加载：

- 亲密关系心理学、依恋理论、MBTI
- 沟通冲突与修复、在线约会与数字关系
- PUA 操控与伦理替代、经典社交体系
- 婚姻家庭、金钱家务育儿
- 中国法律安全与危机转介

实用材料层另含 25 份沟通、话术与场景指南，与知识库分开按需读取。

## 长期记忆（可选）

内置本机长期记忆脚本 `scripts/memory_store.py`，用于跨会话复用精简的关系档案：

- **默认关闭**，需用户明确同意后运行 `enable --confirm` 才启用
- 数据只写在本机数据目录（如 `AppData/Local/love-strategist/`），不同步到任何外部服务
- 支持查看、撤销、暂停、忘记对象与彻底删除

## 仓库结构

```
love-strategist/
├── SKILL.md                     # 核心行为规则与输出结构
├── README.md
├── LICENSE                      # MIT（含上游来源说明）
├── agents/openai.yaml           # Agent 平台接口定义
├── references/
│   ├── knowledge/               # 20 篇跨学科知识文档
│   └── practical/               # 25 篇实战指南与风格材料
└── scripts/
    ├── memory_store.py          # 可选本地长期记忆
    └── validate_skill.py        # 仓库结构与行为边界自检
```

## 校验

提交前可运行：

```bash
python3 scripts/validate_skill.py           # 完整校验（含 README、LICENSE）
python3 scripts/validate_skill.py --runtime # 仅校验运行时必需内容
```

## 来源与致谢

本项目由两个开源 Skill 合并而来，合并、改写与维护由 [Xuefeng122](https://github.com/Xuefeng122) 完成：

1. **[goutoujunshi](https://github.com/shengjidaguai-china/goutoujunshi)** — 狗头军师，提供系统化分析框架、知识库和实战指南
2. **[tong-jincheng-skill](https://github.com/hotcoffeeshake/tong-jincheng-skill)** — 童锦程视角，提供直白街头智慧和表达风格

两个上游项目均以 MIT License 发布，其版权声明已在 `LICENSE` 中保留。向原作者致敬。

## 许可证

MIT License — 详见 [LICENSE](LICENSE)。
