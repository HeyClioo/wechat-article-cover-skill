# 公众号封面生成与评选

把文章交给 Codex，拿回 **10 张公众号封面**和一份面向目标读者的**完整排名**。

这个 Skill 会读取文章，提炼核心观点与点击钩子，生成 10 个真正不同的手绘封面方案，再根据缩略图表现、内容一致性和读者吸引力逐一评选。

```text
文章 → 10 张封面 → 逐张检查 → 完整排名 → 推荐首选
```

## 核心能力

- 一次生成 10 张独立封面，不用反复追加指令
- 候选之间改变标题、视觉隐喻、构图和配色，而不只是微调颜色
- 按目标客户或读者视角给出第 1–10 名及具体原因
- 自动检查明显错字、裁切、比例和主题偏离
- 选定方案后，可继续针对单张封面精修

## 快速开始

### 安装

下载 [`wechat-article-cover.skill`](dist/wechat-article-cover.skill) 安装；也可以手动复制：

```bash
git clone https://github.com/HeyClioo/wechat-article-cover-skill.git
mkdir -p "$HOME/.codex/skills/wechat-article-cover"
cp wechat-article-cover-skill/SKILL.md "$HOME/.codex/skills/wechat-article-cover/SKILL.md"
```

安装后重启 Codex，使 Skill 生效。

### 使用

提供文章正文或本地文件路径：

```text
使用 wechat-article-cover，根据这篇文章生成 10 张公众号封面，
并按目标读者吸引力给出完整排名和原因：

/你的路径/文章.md
```

默认一次完成生成、检查、保存和评选。

## 默认设计规范

| 项目 | 规范 |
| --- | --- |
| 画幅 | 2.35:1 公众号横幅 |
| 风格 | 高对比手绘插画，避免写实元素 |
| 构图 | 主视觉居中或偏左，右侧保留标题区 |
| 文字 | 中文为主，标题不超过 8 个字，可加一行副标题 |
| 视觉 | 1–2 个简洁角色或图标，留白充足，小尺寸醒目 |
| 钩子 | 悬念、数字、痛点或夸张反差 |

详细执行规则见 [SKILL.md](SKILL.md)。

## 评选依据

排名会综合判断：目标读者相关性、缩略图点击力、一秒理解能力、标题钩子、图文一致性和专业可信度。

这些结论是内容与视觉策略判断，不等同于已经验证的真实点击率；正式发布后仍建议结合数据测试。

## 致谢

封面提示词框架参考了宝玉分享的公众号封面生成提示词，在此致谢。本项目在此基础上补充了多方案生成、逐张检查、目标读者评选与 Codex Skill 封装。

<details>
<summary>搜索关键词</summary>

公众号封面、微信公众号封面、微信文章封面、公众号头图、文章配图、AI 生成封面、AI 生图、手绘插画封面、2.35:1 封面、爆款封面、标题钩子、10 个封面候选、目标读者分析、封面排名、Codex Skill、WeChat article cover、cover image generator、AI image generation。

</details>

## 许可证

[MIT](LICENSE)
