这个包包含：
1. install_daxiang_router_agents.sh
2. preview/ 下的各 Agent 工作区文件预览

脚本会做这些事：
- 备份 /Users/fangnaoke/.openclaw/openclaw.json
- 备份 6 个相关 Agent 的工作区和 agentDir
- 将所有 daxiang 入站消息统一绑定到 ceo
- 把 ceo / daxiang-group-chat / guest / private-bot / to-up / to-team 写成可用配置
- 删除旧的 work / to_team_bot / daxiang-agent 路由冲突
- 设置 maxSpawnDepth = 2
- 为 ceo 和 daxiang-group-chat 设置 allowAgents
- 将相关工作区的 AGENTS.md / TOOLS.md / 其他 bootstrap 文件写入
- 最后运行 openclaw config validate

运行：
  bash install_daxiang_router_agents.sh
