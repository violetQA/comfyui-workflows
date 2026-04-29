# AI 协作助手使用日志 / AI Collaboration Assistant Usage Log

## 系统架构 System Architecture

### 运行环境
- OS: WSL2 (Linux 6.6.87.2-microsoft-standard-WSL2)
- Python: 3.12.3
- Node.js: v22.22.2
- OpenClaw: 2026.4.25 (aa36ee6)
- Hermes Agent: v0.11.0 (2026.4.23)

### 核心工具链
- OpenClaw — 主对话助手 (WebChat + WeChat 双渠道)
- Hermes Agent — 定时任务/后台监控
- DashScope Qwen VL — 图片分析
- MiniMax M2.7 — 对话模型
- ComfyUI (aki-v3) — AI 图像生成工作流

## 活跃使用记录 Active Usage

### 心跳定时任务 (Cron Jobs)
- EvoMap 每日探索 — 定时检查 EvoMap Market 资产和 Bounty
- Gateway 健康检查 — 每 30 分钟轮检一次

### 工具使用 Tool Usage
- memory_search — 记忆检索 (每日心跳使用)
- web_search — 网页搜索
- image_generate — 图像生成 (Qwen VL 模型)
- image — 图片分析
- cron — 定时任务调度
- sessions_spawn — 子 Agent 任务委托
- exec — 终端命令执行

### 对话渠道
- WebChat (openclaw-control-ui)
- WeChat (4dac03371825-im-bot)

## 月均 Token 消耗 ≈ 2500万

