# Life Planning Coach

[![Release](https://img.shields.io/github/v/release/mgn170018-prog/life-planning-coach)](https://github.com/mgn170018-prog/life-planning-coach/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111827)](skill/life-planning-coach/SKILL.md)

一套面向 Codex 的循证型人生规划与执行 Skill。

An evidence-informed life-planning and execution coaching skill for Codex.

它通过单问题动态访谈，帮助用户澄清真实目标、现实约束、关键矛盾和下一阶段行动，并把长期方向转化为可验证、可调整的计划。

> 不是成功学话术，也不模仿名人。关键建议区分研究依据、专家实践与个体化推断，并用真实行动结果继续校正。

## 适合谁

- 想系统梳理人生、职业或创业方向；
- 面临辞职、转型、迁居、学习等重要选择；
- 有很多目标，但难以明确优先级和取舍；
- 希望把长期愿景转成年度目标、90天战役和第一周行动；
- 已有计划，希望通过结果、证据和复盘持续调整。

## 核心原则

> 以学术循证方法为骨架，以企业家案例为补充，以用户的真实行动结果作为最终裁判。

- 每次只问一个问题；
- 不机械完成固定题数；
- 根据复杂度自动升级、降级或结束访谈；
- 区分事实、用户观点、推断、证据和待验证假设；
- 用低成本行动实验检验重要判断；
- 不冒充名人或持牌专业人士；
- 医疗、心理健康、法律、投资、税务等高风险问题必须先核验最新权威资料。

## 为什么值得信任

本项目不要求用户因为“AI说得像专家”而相信结论，而是提供可以检查的推理链：

1. 区分事实、用户观点、外部证据、专家实践、本次推断和待验证假设；
2. 关键建议标明依据类型、适用条件和主要局限；
3. 学者和企业家的方法只在其适用范围内使用；
4. 对重大判断设计低成本、可逆的行动验证；
5. 现实结果与原建议冲突时，优先修正建议；
6. 高风险专业问题必须检索当前有效的官方资料。

常用依据包括目标设定、自我决定、实施意图、心理对照、习惯形成、刻意练习和反馈干预等研究。完整来源、适用范围和限制见[证据地图](skill/life-planning-coach/references/evidence-map.md)。

### 依据标签

| 标签 | 含义 |
|---|---|
| `【官方规范】` | 当前有效的法律法规、监管文件、官方指南或专业标准 |
| `【综合研究】` | 系统综述、元分析或高质量共识 |
| `【原始研究】` | 与问题直接相关的同行评审研究 |
| `【专家实践】` | 企业家、管理者或专业实践者的方法与案例 |
| `【本次推断】` | 根据用户已确认信息作出的暂定个体判断 |
| `【证据不足】` | 可靠依据不足、冲突或无法安全外推 |

## 能做什么

- 完整梳理人生方向；
- 分析职业、创业、学习、财富、家庭与生活目标之间的冲突；
- 诊断一个具体的人生决定；
- 制定长期方向、阶段路线、年度目标和90天战役；
- 建立每周、每月和季度复盘机制；
- 审查并调整已有计划。

## 快速安装

在终端执行：

```bash
git clone https://github.com/mgn170018-prog/life-planning-coach.git
cp -R life-planning-coach/skill/life-planning-coach ~/.codex/skills/
```

重新启动或刷新 Codex 后，使用：

```text
$life-planning-coach
```

也可以直接输入：

```text
使用 $life-planning-coach 帮助我梳理人生方向，并转化为可验证、可调整的行动计划。
```

如果已经克隆过仓库：

```bash
git -C life-planning-coach pull
```

然后先备份本机修改过的同名 Skill，再重新复制最新版。

## 使用示例

```text
使用 $life-planning-coach 帮我判断未来三年应该继续职场发展，还是开始创业。
```

```text
使用 $life-planning-coach 帮我完成一次完整人生规划。每次只问一个问题。
```

```text
使用 $life-planning-coach 复盘我的90天计划，根据真实结果判断继续、调整还是停止。
```

## 工作方式

访谈从最低必要深度开始：

- 快速模式：约10—15个问题；
- 标准模式：约25—35个问题；
- 深度模式：约35—50个问题。

题数只是容量提示。Skill 每完成4—6个问题重新评估复杂度，信息充分时提前结束，关键事实不足时继续追问。

完整规划可以包含：

1. 真实目标；
2. 已确认事实与关键假设；
3. 主要矛盾、取舍和机会成本；
4. 当前核心瓶颈；
5. 长期方向与阶段路线；
6. 未来12个月目标；
7. 90天主战役；
8. 第一周行动；
9. 指标、风险和停止条件；
10. 周、月、季度复盘机制。

## 仓库结构

```text
skill/life-planning-coach/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── evidence-and-boundaries.md
    ├── evidence-map.md
    ├── high-stakes-protocol.md
    ├── interview-framework.md
    └── planning-output.md
```

## 方法边界

本 Skill 不是医疗、心理治疗、法律、税务或投资咨询服务。它可以帮助用户整理问题、查阅公开依据、比较选择和准备专业咨询，但不能替代合格专业人士对个案的评估。

企业家案例仅用于提供实践启发，不作为普遍规律或成功保证。

## 参与改进

- 发现证据错误、链接失效或相反研究：提交 [Evidence correction](https://github.com/mgn170018-prog/life-planning-coach/issues/new?template=evidence-correction.yml)；
- 提交功能建议或行为问题：使用 GitHub Issues；
- 贡献前请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。

尤其欢迎心理学、教育、职业发展、创业、法律、医疗和投资领域的专业人士帮助审查边界与证据。

## Project keywords

Codex skill, life planning, life coach, evidence-based coaching, goal setting, career planning, personal development, decision making, implementation intentions, deliberate practice, AI coaching, 人生规划, 职业规划, 目标管理, 循证教练。

## License

[MIT License](LICENSE)
