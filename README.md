# 🎯 Trading Journal — 交易日志

> 基于 CycleStudies 白皮书框架构建的个人交易系统与日志记录

## 仓库说明

这是我的交易成长记录，包含：

- **交易系统**：我的完整交易逻辑和规则（持续迭代中）
- **每日日志**：每天的交易记录、行情判断、开单逻辑
- **每周复盘**：一周的统计数据和反思总结

## 文件导航

| 文件 | 说明 |
|------|------|
| [trading_system.md](./trading_system.md) | 我的交易系统（核心文档） |
| [journals/](./journals/) | 每日交易日志 |
| [templates/](./templates/) | 模板文件 |

## 当前阶段

- [ ] 阶段一：补齐工具认知（通道颜色、EMA眼睛、爆量）
- [ ] 阶段二：小仓位实盘做多，严格执行检查清单
- [ ] 阶段三：加入做空
- [ ] 阶段四：统计优化

## 核心纪律

1. 叠BUFF ≥ 3个才开单
2. 盈亏比 ≥ 1.5:1 才开单
3. 每单风险 ≤ 总资金的 1-2%
4. 每单必填交易记录
5. 大级别定方向，小级别找入场

## 两部分记录结构（交易线 + 研究线）
把本仓库当作“长期可迁移”的 Markdown 知识库来用，你的两个需求会分别放在两条线里：

1. 交易线：`trade-logs/YYYY-MM-DD/`
2. 研究线：`research/YYYY-MM-DD-<slug>/`

### 统一日期规则
所有条目都会在文件夹名/标题中以 `YYYY-MM-DD` 开头，保证你每天新增记录时都能快速找到、也方便后续迁移到别的软件。

### 交易线（每天开单截图 + 思考）
- 每天一个目录：`trade-logs/YYYY-MM-DD/`
- 每天的主文档：`trade-logs/YYYY-MM-DD/index.md`
- 截图直接放到同目录下（`*.png / *.jpg / *.webp`），在 `index.md` 里用相对路径引用
- 模板：`templates/daily-trade-log_template.md`

建议你每天创建 `trade-logs/YYYY-MM-DD/`，然后把 `templates/daily-trade-log_template.md` 复制成 `index.md`，并在文档顶部先填写当日日期。

### 研究线（好文章 / 好截图收藏）
- 每条收藏一份条目：`research/YYYY-MM-DD-<slug>/index.md`
- 条目截图放到同目录下
- 模板：`templates/research_entry_template.md`

建议你每次发现好文章/好截图，先用当日日期命名一个 `<slug>`（例如 `cyclestudies-ema`、`2026-03-31-abc`），然后把模板复制成对应 `index.md`，并把当日日期写在标题里。

### 迁移到其他软件也能用
因为所有内容是普通 Markdown + 本地图片文件，使用相对路径链接截图，所以你之后不管换成 Typora / Obsidian / 其他工具，只要能识别 Markdown 文件和相对图片路径即可直接查看。
