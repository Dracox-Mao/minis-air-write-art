# air-writing-style 离线包

Air（主人）的中文奇幻小说写作风格技能。**零依赖**：纯 Markdown，不需要 Python、Node 或任何网络。

## 安装

把 `skills/air-writing-style/` 整个目录复制到：

```
/var/minis/skills/air-writing-style/
```

复制完在 Minis 里重新打开会话即可生效；`SKILL.md` 的 `name` 与目录名一致，无需改配置。

Android 上用 shell 安装（minis 沙箱）：

```sh
cp -r skills/air-writing-style /var/minis/skills/
```

## 迁移到别的电脑

如果你在用 DSH（DeepSeek Harness）之类支持 `SKILL.md` 约定的宿主，直接把 `skills/air-writing-style/` 当成一个普通 skill 目录导入即可。
SKILL.md 里提到的 `/var/minis/shared/writing-style-corpus/` 路径只在 Minis 上存在，语料副本已放进本包 `corpus/`，需要时自行改路径或拷到对应位置。

## 目录

```
air-writing-style/
├── SKILL.md                        主文件：画像 + 十条铁律 + 落笔流程
├── references/
│   ├── style-analysis.md           全量统计（字频、段长、对话比、标点、外语使用）
│   ├── signature-phrases.md        句式模板、场景套路、人物速查、外语香料
│   └── chapter-recipes.md          四种章型分镜表（日常/战斗/设定/反派）
└── corpus/
    ├── sygklisi.txt                《行于隙旅》正文 3.7 万字纯文本
    ├── magic_nova.txt              《杜纳米斯特辑》纯文本
    └── README.md                   语料说明与再生成方法
```

## 出处

语料：`Sygklisi.docx`（111 KB / 1,776 段）、`Magic_Nova.docx`（17.9 KB / 154 段），合计汉字 37,677 字。
统计日期：2026-10-31。
