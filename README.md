# TME音乐广告运营 — 周报工作流平台

🎵 **TME Ad Ops Weekly Intelligence Dashboard**

面向TME音乐产品广告流量运营团队的周报型工作流可视化平台。

## 📋 功能模块

| 模块 | 说明 | 更新频率 |
|------|------|----------|
| 🔍 竞品产品动态 | Spotify/网易云/Apple Music/汽水音乐产品追踪 | 每周 |
| 📊 财报解读 | TME及竞品关键财务指标与增长趋势 | 每季度 |
| 📰 行业动态 | 音乐行业资讯、版权动态、热歌趋势 | 每周 |
| 👥 用户指标对比 | MAU/ARPU/付费率/会员占比多维对比 | 每周 |
| 🎯 广告策略建议 | 综合数据输出投放策略建议 | 每周 |
| 📋 周报总览 | 关键变化、重点关注、下周计划 | 每周 |

## 🚀 部署

本项目通过 GitHub Pages 部署，访问地址：
`https://<your-username>.github.io/tme-ad-workflow/`

## 🔄 自动更新

通过 GitHub Actions 每周一上午9:00 (UTC+8) 自动运行 `scripts/update_report.py`，抓取公开数据更新周报。

也支持手动触发：GitHub仓库 → Actions → Weekly Report Update → Run workflow

## 📁 项目结构

```
tme-ad-workflow/
├── index.html                    # Dashboard主页面
├── data/
│   └── weekly-report.json        # 周报数据（自动更新）
├── scripts/
│   └── update_report.py          # 数据更新脚本
├── .github/
│   └── workflows/
│       └── weekly-update.yml     # GitHub Actions配置
├── requirements.txt              # Python依赖
└── README.md
```

## ⚠️ 声明

本平台不含任何内部业务数据，所有信息均为AI基于公开数据生成的分析与建议，仅供参考。
