获取 TG Bot Token 和 Chat ID

Telegram 搜索 @BotFather → /newbot → 按提示创建 → 复制 Token
Telegram 搜索 @userinfobot → 发送任意消息 → 复制 Id 字段（即 Chat ID）
Secret 名称获取方式AIR_API_TOKENNVIDIA Air 控制台 → 右上角头像 → API TokensAIR_TOPOLOGY_IDAir 拓扑页面 URL 里的 UUIDTG_BOT_TOKENTelegram 找 @BotFather → /newbotTG_CHAT_IDTelegram 找 @userinfobot 发消息获取
配置完后可以去 Actions 标签页手动触发一次（workflow_dispatch）测试，看 TG 是否收到通知，确认没问题后定时任务就会自动跑了。
