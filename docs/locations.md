# 跨期场景库

本文件维护跨期可复用的 location preset。`episodes/*.md` 只引用 `location.id`，具体风格、光线、道具和 MJ 锚点在这里维护。

## 使用规则

- `id` 使用英文小写、数字和下划线。
- `mj_anchor` 用英文，方便拼入提示词。
- 同一个场景可通过 `variants` 区分正常、午休、定格、夜晚等状态。

## office_floor_5 · 五楼大平层办公区

```yaml
id: office_floor_5
display_name: 五楼大平层办公区
style: chinese internet company, open plan office
lighting: warm noon light, heavy window shadows
palette: low saturation, warm gray, muted yellow
props: [cubicle desks, monitors, office chairs, wall clock]
variants: [normal, lunch_break, freeze]
mj_anchor: "modern Chinese corporate open-plan office, dim warm noon light, heavy window shadows, cubicle desks, cinematic"
used_in: [001]
```

## glass_mailroom · 玻璃快递房

```yaml
id: glass_mailroom
display_name: 玻璃快递房
style: semi-transparent office mailroom beside open-plan office
lighting: cool white ceiling light, glass reflection
palette: cool gray, muted blue, cardboard brown
props: [glass wall, cardboard boxes, parcels, packing tape]
variants: [busy, noisy, reflected]
mj_anchor: "semi-transparent glass mailroom inside modern office, courier silhouette, stacked parcels, cool white light, cinematic reflection"
used_in: [001]
```

## company_group_chat_ui · 公司大群手机界面

```yaml
id: company_group_chat_ui
display_name: 公司大群手机界面
style: clean professional mobile group chat interface
lighting: cool phone screen glow
palette: white interface, green outgoing bubble, dark CEO bubble, gold badge
props: [smartphone, chat bubbles, CEO badge, timestamp]
variants: [send_message, waiting, ceo_reply]
mj_anchor: "clean smartphone group chat UI, readable layout, green message bubble, premium dark CEO bubble with golden badge"
used_in: [001]
```

## midnight_workstation · 深夜空办公室工位

```yaml
id: midnight_workstation
display_name: 深夜空办公室工位
style: late-night office workstation
lighting: blue computer screen glow, dark background
palette: blue gray, black, low saturation
props: [laptop, office desk, chair, smartphone, clock]
variants: [alone, exhausted, closing]
mj_anchor: "late night modern Chinese office workstation, blue computer screen glow, one tired worker, cinematic low-key lighting"
used_in: [000]
```

## phone_notification_ui · 手机日历通知界面

```yaml
id: phone_notification_ui
display_name: 手机日历通知界面
style: minimal smartphone notification UI
lighting: bright phone screen on dark background
palette: white notification card, cool gray background
props: [smartphone, calendar notification, lock screen]
variants: [calendar_alert, black_screen]
mj_anchor: "smartphone lock screen notification UI, clean white notification card, calendar alert, dark background"
used_in: [000]
```
