# LynxOPC — The OPC Ledger

> 一人公司(One-Person Company)政策与社区信息聚合站。
> 数据全部来自政府公开政策文件、园区官方公告、新闻报道,不经手第三方数据站。
> 风格沿用主站 [lxlynx.com](https://lxlynx.com) 的"编辑式账本"美学。

## 定位

帮创业者快速查清楚:哪个城市/园区对一人公司免房租、有什么补贴、入驻门槛是什么。
**不做全城市对标,先做深杭州,尤其余杭区。**

## 数据来源原则

- ✅ 政府官网公开政策文件
- ✅ 园区/孵化器官方公告
- ✅ 公开新闻报道(标注来源链接)
- ❌ 不抓取第三方聚合站的整理结果
- ❌ 不 AI 编造政策;缺失官链时明示"参考来源"

## 技术栈

- 纯原生单文件 HTML/CSS/JS,无框架(同 lxlynx.com)
- 数据层:`data/opc.json` 结构化政策 + 社区
- 开放出口:JSON API + RSS + llms.txt
- 双语:中/英切换(localStorage 持久化)

## 目录

```
LynxOPC/
├── index.html          # 首页(杭州概览 + 社区卡片)
├── compare.html        # 城市对比工具
├── data/
│   └── opc.json        # 结构化政策/社区数据
├── cities/
│   └── hangzhou.html   # 杭州详情(余杭区为主)
├── assets/
│   ├── css/            # 样式(账本风格)
│   └── js/             # 双语切换 + 渲染
├── rss.xml             # 数据更新订阅
├── llms.txt            # LLM 可读站点摘要
└── README.md
```

## 开发计划

- [x] 项目骨架
- [ ] 首页 index.html(账本风格 + 杭州种子数据)
- [ ] data/opc.json 结构化数据
- [ ] 杭州城市详情页
- [ ] 对比工具
- [ ] 开放数据出口
