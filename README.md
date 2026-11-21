# 周公解梦 · Zhougong Dream Interpretation

一个按原典解梦的 Claude 技能（Skill）。它以通行本《周公解梦》和东汉王符《潜夫论·梦列》的**原文**为依据，逐条引用，再加上心理学视角，以及可选的八字联动。

A Claude Skill that interprets dreams from the **original classical texts**: the popular edition of *Zhougong Jiemeng* (The Duke of Zhou's Dream Interpretation) and Wang Fu's *Qianfu Lun · Menglie* ("On Dreams", Eastern Han). It quotes the sources entry by entry, then adds a psychological reading and an optional BaZi (Four Pillars) link.

---

## 特点 ｜ Features

| 中文 | English |
|---|---|
| **引经据典，不编原文**：先查原文条目原样引用；原书没有就明说"未收此条"，不编造 | **Cited, never invented:** quotes matching entries verbatim; if the text has no entry, it says so instead of making one up |
| **十梦分类**：按《梦列》把梦归入直、象、精、想、人、感、时、反、病、性十类 | **Ten kinds of dreams:** classifies each dream using *Menglie*'s ten categories |
| **感受定吉凶**：依《梦列》"梦吉事而己意大喜乐……则真吉"，先问梦里的感受 | **Feeling decides the omen:** following *Menglie*, the dreamer's emotion in the dream comes first |
| **反梦提示**：原文本身判为吉的"凶象"会如实说明，不吓人 | **Reversals explained:** frightening images the text itself reads as auspicious are explained calmly |
| **心理学视角**：每次都附一段现实心事的解读 | **Psychological reading:** every interpretation links the dream to waking concerns |
| **八字联动（可选）**：若有命盘，看做梦当晚的流年、流月、流日与原局的呼应 | **Optional BaZi link:** if a chart is available, relates the night's pillars to the natal chart |
| **中英双语**：用户用什么语言就用什么语言回答，原文始终保留 | **Bilingual:** replies in the user's language and always keeps the original Chinese |

## 内容 ｜ Contents

```
zhougong-jiemeng/
├── SKILL.md                                      # 技能说明（中英对照） · Skill instructions (bilingual)
└── references/
    ├── zhougong-jiemeng-original.md              # 《周公解夢》全文 27 章 · Full text, 27 chapters (~900 entries)
    ├── zhougong-jiemeng-selected-en.md           # 86 条精选中英对照 · 86 selected entries, Chinese–English
    └── menglie-zh-en.md                          # 《夢列》全文中英对照 · Full Menglie, Chinese–English
```

## 安装 ｜ Installation

**Claude Code**：把 `zhougong-jiemeng/` 文件夹复制到 `~/.claude/skills/`。
Copy the `zhougong-jiemeng/` folder into `~/.claude/skills/`.

```bash
git clone https://github.com/kkkkkkkaro-cyber/-Book-of-Dreams.git
cp -r -- -Book-of-Dreams/zhougong-jiemeng ~/.claude/skills/
```

**Claude 应用 ｜ Claude apps**：把 `zhougong-jiemeng/` 文件夹打包成 zip，在技能设置中上传。
Zip the `zhougong-jiemeng/` folder and upload it as a custom skill.

## 用法示例 ｜ Example

> **用户**：我梦到很多人想和我当室友，梦里有点开心。
>
> **Claude**：
> - 一句话结论：偏吉，属《夢列》所说的"想梦"：「人有所思，即夢其到」。
> - 原典：《周公解夢·帝王文武呼召》「一切貴人皆吉祥」；《船車遊行物件》「與人同船主移居」（类推）……
> - 梦里开心，依《夢列》「己意大喜樂……則真吉矣」，偏向贵人相助一面。

> **User:** I dreamed lots of people wanted to be my roommate, and I felt a bit happy.
>
> **Claude:**
> - Verdict: mildly auspicious, a "reflective" dream in *Menglie*'s terms.
> - Classics: 「一切貴人皆吉祥」 "All noble persons are auspicious"; 「與人同船主移居」 "Sharing a boat with others: you will move house" (by analogy)…

## 版本与来源 ｜ Sources & editions

- **《周公解夢》通行本** · *Zhougong Jiemeng*, popular edition. 来源：[维基文库](https://zh.wikisource.org/wiki/周公解夢)。托名周公旦，实为后世（一般认为明清时期）民间编辑的七言条目梦书，**与敦煌唐写本《新集周公解夢書》不是同一本**。
  Via Wikisource. Attributed to the Duke of Zhou but actually a later popular compilation (generally dated Ming–Qing), **not the Tang-dynasty Dunhuang manuscript**.
- **王符《潛夫論·夢列第二十八》** · Wang Fu, *Qianfu Lun*, ch. 28. 来源：[维基文库](https://zh.wikisource.org/wiki/潛夫論/卷七)。已校正两处繁简转换讹字。
  Via Wikisource; two character-conversion errors corrected.
- 英译均为本项目所作。 · All English translations are by this project.

## 许可 ｜ License

- 技能说明、英译与整理：MIT（见 `LICENSE`）。 · Skill instructions, translations and arrangement: MIT (see `LICENSE`).
- 两部古籍原文属公有领域。 · The two classical source texts are in the public domain.

## 免责声明 ｜ Disclaimer

解梦仅供文化参考与自我反思，不是预测，也不能替代医疗或心理专业意见。

Dream interpretation here is for cultural interest and self-reflection only. It is not prediction and is no substitute for medical or mental-health advice.
