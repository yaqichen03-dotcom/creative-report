# 数码家电行业直播链路跑量素材双周报

📊 Digital & Home Appliance · Live-streaming Bi-weekly Report

## 在线预览

部署到 GitHub Pages 后访问：
https://yaqichen03-dotcom.github.io/creative-report/

## 项目组成

- **index.html** - 前端页面（纯静态，可直接托管到 GitHub Pages）
- **data/top50_analysis.json** - Top 跑量素材分析数据
- **data/industry_insights.json** - 行业共性特征提炼
- **server.py** - 本地后端（管理员用，不部署到线上）
- **analyze.py** - 命令行批量分析脚本

## 数据更新流程

1. **管理员本地运行分析**：
   ```bash
   python3 server.py
   ```

2. **打开本地网页上传CSV**：`http://localhost:8765/index.html`

3. **分析完成后推送更新**：
   ```bash
   git add data/top50_analysis.json data/industry_insights.json
   git commit -m "更新双周报数据"
   git push
   ```

4. **GitHub Pages 自动部署**，通常 1-2 分钟后线上生效。

## 功能亮点

- ✅ Top 素材逐个拆解：黄金三秒 / 素材结构 / 核心卖点 / 吸睛开头 prompt
- ✅ 多维度筛选：商品类目 / 素材类型 / 转化人群
- ✅ 行业共性特征自动提炼
- ✅ 行业大盘 Benchmark 对比（白牌 vs 品牌赛道）
- ✅ 视频直接在卡片内预览（显示第1秒画面）
- ✅ 一键复制 AI 视频生成 prompt + 跳转妙思平台

## 技术栈

- 前端：HTML5 + CSS3 + 原生 JavaScript
- 后端：Python 3 + HTTP Server（本地）
- AI：Google Gemini 2.5 Flash（视频理解）
- 托管：GitHub Pages（纯静态）
