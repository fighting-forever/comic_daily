# 001 · 午休风波 · 提示词卡

复制本页内容到 Midjourney / Runway / 剪映即可。`2场1镜` 和 `2场2镜` 不做 i2v，优先使用手机截图、剪映文字和定格。

## 全局锚点

- 风格：现代职场写实摄影感，低饱和，办公室暗部重。
- 角色：小职员近景作为主角种子图；CEO 优先用群聊昵称、金色角标或头像表达。
- 角色库：`../../docs/characters.md`；场景库：`../../docs/locations.md`。
- 画幅：办公室镜头可 `--ar 16:9` 生成后裁切；群聊镜头用 `--ar 9:16`。
- 成本护栏：单镜出图不超过 8 次；i2v 不超过 3 次。

---

### 1场1镜 · 午休办公区全景

- 资产：`stills/1场1镜.png` | `clips/1场1镜.mp4`
- i2v：Yes
- 时长：4s
- role：setup
- character：[`npc_sleepers`]
- location：`office_floor_5`
- audio：[`office_ac_hum`]

**MJ 提示词**

```text
Inside a large modern Chinese corporate office, dim moody lighting, dozens of real Asian employees sleeping at their cubicle desks at 1:00 PM, heavy window shadows, photorealistic, cinematic composition --ar 16:9
```

**Runway i2v 控制**

```text
Static shot, subtle breathing motion, tiny dust motes floating slowly in the dim light. Keep all faces indistinct, no large body movement.
```

**备注**：大厂控本。全景不要看清脸，减少人脸一致性成本。

---

### 1场2镜 · 玻璃快递房噪音

- 资产：`stills/1场2镜.png` | `clips/1场2镜.mp4`
- i2v：Yes
- 时长：4s
- role：tension
- character：[`courier_01`]
- location：`glass_mailroom`
- audio：[`tape_rip`, `box_hit`, `tape_box`]

**MJ 提示词**

```text
POV shot looking at a semi-transparent glass mailroom nearby, blurry background office, a courier in uniform working inside, high contrast, cinematic photography --ar 16:9
```

**Runway i2v 控制**

```text
Camera slowly tracking forward, sharp focus on the glass room reflection. The courier remains mostly silhouette, no detailed hand action, no tape tearing close-up.
```

**备注**：动作防融化。不画撕胶带的手，靠空间和音效传达噪音。

---

### 1场3镜 · 小职员惊醒

- 资产：`stills/1场3镜.png` | `clips/1场3镜.mp4`
- i2v：Yes
- 时长：5s
- role：tension
- character：[`employee_01`]
- location：`office_floor_5`
- audio：[`vo_clerk_inner`]

**MJ 提示词**

```text
A young Asian male office clerk with glasses abruptly waking up at his desk, extremely frustrated expression, sharp eyes looking to the side, realistic skin texture, desk marks on cheek --ar 16:9
```

**Runway i2v 控制**

```text
Dolly zoom, camera suddenly pulls back, facial muscles tense, background blurs. Keep the same face identity, no mouth distortion, no large head rotation.
```

**备注**：这张图跑通后冻结为 `[主角小职员-ID]`。

---

### 2场1镜 · 群聊吐槽发送

- 资产：`stills/2场1镜.png` | `clips/2场1镜.mp4`
- i2v：No
- 时长：5s
- role：escalation
- character：[`employee_01`]
- location：`company_group_chat_ui`
- audio：[`keyboard_typing`, `message_send`]

**MJ 提示词**

```text
不使用 MJ 生成中文。用真实手机截图或剪映界面：公司大群，绿色气泡显示“大中午的能不能有点自觉，没看到别人都是午睡吗？”
```

**Runway i2v 控制**

```text
不做 i2v：剪映做 2-4 帧气泡弹出，搭配键盘声和发送音。
```

**备注**：100% 零成本。手机截图最清晰，不让 AI 生成中文。

---

### 2场2镜 · 13:02 冷场

- 资产：`stills/2场2镜.png` | `clips/2场2镜.mp4`
- i2v：No
- 时长：4s
- role：pause
- character：[`npc_sleepers`, `courier_01`]
- location：`office_floor_5`
- audio：[`clock_tick`]

**MJ 提示词**

```text
Same office environment as shot 01, all employees and the courier guy completely frozen in place, awkward silence, realistic corporate workspace, heavy shadows --ar 16:9
```

**Runway i2v 控制**

```text
不做 i2v：剪映定格，所有环境音切断，右下角加 13:01 → 13:02 时间戳动画。
```

**备注**：戏剧张力来自静音和时间戳，不来自复杂运动。

---

### 2场3镜 · CEO 群聊反杀

- 资产：`stills/2场3镜.png` | `clips/2场3镜.mp4`
- i2v：Yes
- 时长：8s
- role：punchline
- character：[`ceo_01`]
- location：`company_group_chat_ui`
- audio：[`gavel_hit`]

**MJ 提示词**

```text
Extreme close-up of the same smartphone group chat interface, premium dark chat bubble with shiny golden CEO label badge, devastating reply, dramatic pause --ar 9:16
```

**Runway i2v 控制**

```text
New bubble appears with sharp micro-shake, then fade to black. Keep text area stable and readable; no UI distortion.
```

**备注**：如果 Runway 破坏中文，直接改用手机截图 + 剪映微震 + 切黑。
