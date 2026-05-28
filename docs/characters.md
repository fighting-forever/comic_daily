# 跨期角色库

本文件是跨期角色 Bible。`episodes/*.md` 只引用 `character.id`，具体外观、道具和 MJ 锚点在这里维护。

## 使用规则

- `id` 使用英文小写、数字和下划线，避免工具解析中文。
- `mj_anchor` 用英文，方便直接拼入 Midjourney / Runway prompt。
- 只追求「同一类人稳定」，不追求影视级角色连续性。

## employee_01 · 小职员

```yaml
id: employee_01
display_name: 小职员
archetype: tired office clerk
gender: male
age: 25-30
hair: short black hair, slightly messy
cloth: wrinkled office shirt, optional gray hoodie
props: [office badge, smartphone, desk marks on cheek]
emotion_base: tired, restrained, easily annoyed
mj_anchor: "young Asian male office clerk with glasses, slightly messy short black hair, wrinkled office shirt, tired and annoyed expression, realistic cinematic"
used_in: [001]
```

## ceo_01 · CEO

```yaml
id: ceo_01
display_name: CEO
archetype: high-status executive presence
gender: unspecified
age: 35-50
hair: not visible
cloth: not visible
props: [gold CEO badge, premium dark chat bubble, authority label]
emotion_base: calm, detached, authoritative
mj_anchor: "premium dark company chat bubble with shiny golden CEO label badge, authoritative executive presence, clean mobile UI"
used_in: [001]
```

## courier_01 · 快递小哥

```yaml
id: courier_01
display_name: 快递小哥
archetype: busy delivery worker
gender: male
age: 20-35
hair: mostly hidden or blurred
cloth: blue courier uniform
props: [cardboard boxes, parcels, packing tape, glass mailroom]
emotion_base: focused, unaware, non-malicious
mj_anchor: "Asian courier worker in blue uniform, busy inside semi-transparent glass mailroom, stacked parcels, mostly silhouette, cinematic"
used_in: [001]
```

## npc_sleepers · 午睡同事群体

```yaml
id: npc_sleepers
display_name: 午睡同事们
archetype: sleeping office crowd
gender: mixed
age: 22-40
hair: indistinct
cloth: casual office wear
props: [cubicle desks, office chairs, monitors, jackets used as blankets]
emotion_base: sleeping, unaware, static
mj_anchor: "dozens of Asian office employees sleeping at cubicle desks, faces indistinct, quiet lunch break atmosphere, modern office"
used_in: [001]
```

## employee_02 · 深夜打工人

```yaml
id: employee_02
display_name: 深夜打工人
archetype: late-night office worker
gender: unspecified
age: 25-35
hair: neat or slightly messy dark hair
cloth: white shirt or hoodie
props: [laptop, smartphone, office desk, calendar notification]
emotion_base: exhausted, self-comforting, fragile optimism
mj_anchor: "tired young Asian office worker late at night, blue computer light on face, forcing a small optimistic smile, realistic cinematic"
used_in: [000]
```
