# 000 · MVP练手 · 提示词卡

复制本页内容到 Midjourney / Runway / 剪映即可。只让 `1场2镜` 做 i2v，其余用静帧、截图和剪映动画完成。

## 全局锚点

- 风格：夜晚职场写实，低饱和冷光，干净构图。
- 主角：年轻亚洲职场人，疲惫但强撑乐观，白衬衫或卫衣。
- 角色库：`../../docs/characters.md`；场景库：`../../docs/locations.md`。
- 画幅：9:16。
- 预算护栏：单镜出图不超过 8 次；i2v 不超过 3 次。

---

### 1场1镜 · 深夜工位

- 资产：`stills/1场1镜.png` | `clips/1场1镜.mp4`
- i2v：No
- 时长：5s
- role：setup
- character：[`employee_02`]
- location：`midnight_workstation`
- audio：[`amb_office_night`, `keyboard_stop`, `vo_finally_off_work`]

**MJ 提示词**

```text
late night modern Chinese office, one tired young office worker sitting alone at desk, computer screen glow, time 23:48 implied, cinematic low-key lighting --ar 9:16
```

**Runway i2v 控制**

```text
不做 i2v：剪映做 105% 缓慢推近即可，保持画面稳定。
```

**备注**：MVP 不追求动作，先验证深夜疲惫氛围是否成立。

---

### 1场2镜 · 自我安慰

- 资产：`stills/1场2镜.png` | `clips/1场2镜.mp4`
- i2v：Yes
- 时长：5s
- role：tension
- character：[`employee_02`]
- location：`midnight_workstation`
- audio：[`vo_hope_sleep`]

**MJ 提示词**

```text
close-up tired young Asian office worker forcing a small optimistic smile, blue computer light on face, late night office background, realistic cinematic style --ar 9:16
```

**Runway i2v 控制**

```text
Subtle push in, keep face identity, no large body movement, no head turn, no distorted mouth, calm late-night office atmosphere.
```

**备注**：只做轻微表情和推近，不让 AI 做复杂说话嘴型。

---

### 1场3镜 · 早会提醒反杀

- 资产：`stills/1场3镜.png` | `clips/1场3镜.mp4`
- i2v：No
- 时长：5s
- role：punchline
- character：[`employee_02`]
- location：`phone_notification_ui`
- audio：[`calendar_alert`]

**MJ 提示词**

```text
不使用 MJ 生成中文。用真实手机截图或剪映通知样式制作：明早 8:30 全员早会。
```

**Runway i2v 控制**

```text
不做 i2v：剪映做通知下滑动画，清脆提示音后切黑，黑屏保留 1 秒。
```

**备注**：中文必须清晰；通知内容是 punchline，不要交给图像模型生成。
