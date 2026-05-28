# comic_daily

面向「小白转行短剧个人工作室」的内容到短视频工作台。仓库名保留 `comic_daily`，实际主线是：用 Markdown 管理剧本和分镜，用 HTML 做导演预览页，用 `production/` 管理静帧、视频、音频和导出物。

Markdown 是单一可信源；条漫是静帧副产品，短视频是主要目标。

## 阅读顺序

1. [docs/可行性方案.md](docs/可行性方案.md)：先判断个人工作室怎么低成本跑通。
2. [docs/制作指南.md](docs/制作指南.md)：再按 MJ → Runway → 剪映执行。
3. [docs/characters.md](docs/characters.md)：复用跨期角色 ID 和 MJ 锚点。
4. [docs/locations.md](docs/locations.md)：复用跨期场景 ID、光线和道具 preset。
5. [TEMPLATE.md](TEMPLATE.md)：新开一篇时复制填写。
6. [docs/storyboard-template.html](docs/storyboard-template.html)：需要导演预览页时复制到对应 `production/`。

## 双入口

| 入口 | 适合阶段 | 脚本 | 目标 |
|------|----------|------|------|
| MVP 练手 | 第 1 周 | [episodes/000-MVP练手.md](episodes/000-MVP练手.md) | 3 镜、15 秒、1 个 i2v 镜头，先跑通闭环 |
| 挑战关 | 熟悉流程后 | [episodes/001-午休风波.md](episodes/001-午休风波.md) | 6 镜、约 30 秒、办公室反转短剧 |

## 连载目录

| 期号 | 标题 | 难度 | 脚本 | 导演预览页 | 一句话梗概 |
|------|------|------|------|------------|------------|
| 第 0 期 | MVP练手 | ★MVP | [episodes/000-MVP练手.md](episodes/000-MVP练手.md) | 可选 | 打工人刚说「明天一定早睡」，手机提醒明早早会。 |
| 第 1 期 | 午休风波 | ★★★挑战 | [episodes/001-午休风波.md](episodes/001-午休风波.md) | [production/001-午休风波/storyboard.html](production/001-午休风波/storyboard.html) | 小职员午休被快递噪音激怒大群喊话，CEO 一句「我怎么不知道有午休」反杀。 |

## 新开一篇

1. 复制 [TEMPLATE.md](TEMPLATE.md) 到 `episodes/{三位序号}-{短标题}.md`，先定难度：★MVP / ★★入门 / ★★★挑战。
2. 在 `production/{三位序号}-{短标题}/` 创建 `stills/`、`clips/`、`audio/`、`export/`，需要预览页时复制 `docs/storyboard-template.html` 为 `storyboard.html`。
3. 按 [docs/制作指南.md](docs/制作指南.md) 跑静帧、i2v、音频、剪映，最后把产出清单和 README 目录补齐。

## 目录说明

| 路径 | 说明 |
|------|------|
| [TEMPLATE.md](TEMPLATE.md) | 新篇脚本模板，包含难度、分镜单表、i2v 控制、声音设计和避坑风险。 |
| [docs/](docs/) | 可行性方案、制作指南、HTML 分镜模板。 |
| [docs/characters.md](docs/characters.md) | 跨期角色库，维护 `character.id` 与角色外观锚点。 |
| [docs/locations.md](docs/locations.md) | 跨期场景库，维护 `location.id`、光线、道具和场景锚点。 |
| [episodes/](episodes/) | 各期 Markdown 脚本，是单一可信源。 |
| [production/](production/) | 各期素材目录，统一 `stills/clips/audio/export`。 |
