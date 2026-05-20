这是一个通过调用 NVIDIA Air API 给指定拓扑续期的项目

第一步：获取 NVIDIA Air API Token
登录 air.cgi.com 后，在个人设置里生成 API Token。

第二步：创建 GitHub Actions Workflow

第三步：配置 GitHub Secrets
在仓库的 Settings → Secrets and variables → Actions 里添加：

需要配置的 4 个 Secrets
进入仓库 Settings → Secrets and variables → Actions → New repository secret，依次添加：

AIR_API_TOKEN:NVIDIA Air 控制台 → 右上角头像 → API Tokens

AIR_TOPOLOGY_ID:Air 拓扑页面 URL 里的 UUID

TG_BOT_TOKEN:Telegram Bot Token（找 @BotFather 创建）

TG_CHAT_ID:你的 Telegram Chat ID（找 @userinfobot 获取）


配置完后可以去 Actions 标签页手动触发一次（workflow_dispatch）测试，看 TG 是否收到通知，确认没问题后定时任务就会自动跑了。
