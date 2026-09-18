# platform_submit_pack

## Purpose

Turn a **single** metadata pack from `tools/submission_checklist.md` into platform-ready paste sheets.

One source of truth — no second marketing draft.

---

## When To Use

After checklist metadata is filled and continuity / golden-three gates pass.

Before opening any platform upload form.

---

## Inputs

| Input | Source |
|-------|--------|
| Metadata pack | `tools/submission_checklist.md` (Blurb backfill example) |
| Platform notes | `knowledge/submit_*.md` |
| Cover brief | checklist metadata |

---

## Output layout

```text
submit-pack/
  README.md                 # how to paste
  qidian.md
  tomato.md
  jinjiang.md
  feilu.md
  qimao.md
  zongheng.md
```

One file per platform. Same title/synopsis facts; only field mapping and tone notes differ.

---

## Sheet template (every platform file)

```markdown
# {Platform} 投稿包

## 表单粘贴区

| 表单字段 | 粘贴内容 |
|----------|----------|
| 书名 | {title} |
| 一句话简介 | {one_liner} |
| 简介（短） | {short_blurb} |
| 简介（长） | {long_synopsis} |
| 分类 | {category} |
| 标签 | {tags} |
| 作者寄语 | {author note} |

## 封面 brief
{cover brief}

## 平台注意（来自 knowledge）
- {要点1}
- {要点2}

## 提交前检查
- [ ] checklist gates 1–8 已过
- [ ] 本文件内容与 checklist 元数据一致
- [ ] 未新增未验证的卖点
```

---

## Platform field map

| Platform | Primary synopsis length | Notes |
|----------|-------------------------|-------|
| 起点 qidian | 80–150 字 + 标签 | 见 knowledge/submit_qidian.md |
| 番茄 tomato | 偏短、强钩子 | 见 knowledge/submit_tomato.md |
| 晋江 jinjiang | 感情线权重更高 | 见 knowledge/submit_jinjiang.md |
| 飞卢 feilu | 硬门禁，先过 hard gates | 见 knowledge/submit_feilu.md |
| 七猫 qimao | 移动端更短简介 | 见 knowledge/submit_qimao.md |
| 纵横 zongheng | 先过 golden three | 见 knowledge/submit_zongheng.md |

Always **copy** from the checklist table; only compress length if the platform sheet says to.

---

## Generated pack checklist

- [ ] `submit-pack/` created
- [ ] Each sheet’s 书名/简介/标签 equals checklist metadata
- [ ] Platform “注意” bullets filled from knowledge files
- [ ] File names use lowercase platform id
- [ ] Optional export name: `{book-slug}_submitpack_v{skill}_{YYYYMMDD}.zip`
