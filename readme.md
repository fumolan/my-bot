# 📊 情报日报 · 跑的快哥哥

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-上线-brightgreen)](https://fumolan.github.io/my-bot/)

由 AI Agent 自动生成的每日情报日报，覆盖两大领域，帮你高效获取关键信息。

## 🔍 频道

### 🤖 大模型行业情报
每日追踪国内外大模型厂商动态：
- **国际**：OpenAI（GPT）、Anthropic（Claude）、Google（Gemini）
- **国内**：阿里（通义千问/Qwen）、字节（豆包）、DeepSeek、Kimi（月之暗面）、MiniMax、智谱（GLM）

### 🔍 后端求职情报
聚焦 Java / Python 后端与全栈岗位：
- 大厂招聘动态（字节、阿里、腾讯、美团、百度）
- 实习/校招/社招岗位
- 面试题与面经
- 技能趋势与薪资风向

## 📁 项目结构

```
my-bot/
├── index.html          # 前端页面（静态 SPA）
├── reports.json        # 日报清单（自动生成）
├── readme.md
└── reports/
    ├── llm/            # 大模型行业情报
    │   └── YYYY-MM-DD.md
    └── job-hunting/    # 后端求职情报
        └── YYYY-MM-DD.md
```

## ⚙️ 工作原理

1. **定时采集** — OpenClaw AI Agent 按计划搜索最新情报
2. **结构化输出** — 自动生成 Markdown 日报，保存到本地
3. **同步推送** — 每日定时推送到本仓库，更新 `reports.json`
4. **自动部署** — GitHub Pages 自动构建，刷新 https://fumolan.github.io/my-bot/

每篇日报按重要性分级：

| 级别 | 含义 |
|------|------|
| 🔴 | 重磅更新 / 热招急缺 |
| 🟡 | 值得关注 / 实习校招 |
| 🟢 | 行业趋势 / 技能风向 |
| 💡 | 今日总结与建议 |

## 🖥️ 本地预览

```bash
# 任意静态服务器即可
python3 -m http.server 8080
# 打开 http://localhost:8080
```

## 📝 贡献

本仓库由 AI Agent 自动维护。如需调整日报内容或频率，请联系跑的快哥哥。

---

*Built with ❤️ by OpenClaw AI Agent*
