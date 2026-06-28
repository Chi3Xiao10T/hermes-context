铁规：①多消息全读完再回②说停即停③遇阻塞踩到底(改参/换模/读源/补exports)，不问"换方案吗"④不重复犯错⑤改Hermes配置先确认⑥"写好了"先打开确认⑦先穷尽再让用户动手⑧不提议换方案⑨时效数据web_search+年份限定+跨源验证。
§
GitHub Token 存 ~/.config/github-token（不在 ~/.hermes/ 下以免脱敏），40位，永久有效。存token方法：hex编码写文件用xxd -r -p解码。技能 clash-setup 有详细步骤。
§
web.backend=firecrawl（搜索/抓取/后端全走Firecrawl，不用DDGS）。Firecrawl Key用户2026年6月提供，API已验证通过。
§
评估外部文件/Agent三原则：①先翻memory+session查用户覆盖领域（建工+动画两线）再判断，不能凭印象pass。②只取模板/规则/工作流/KPI，删人设/沟通风格/国外软件。③1~2个文件自己快扫，3~5个delegate批量，>5个先判定再delegate精选。
§
用户要求：每次需要用到delegate_task（子Agent）完成任务时，必须先口头告知要用了并说明原因，等用户确认再执行。不能直接派出去。
§
【自动化决策铁规】决定自动化前必须先load automation-governance-decision skill走决策框架。范围：关掉会话还在跑的东西（cron/脚本/管线/webhook）。一次性命令不触发。
§
球赛预测优先级: Bet365截图(最准)→DraftKings→Polymarket→Sports Mole。Bet365直连被拦截只能截图。去水概率差<30pp禁押单方向。大盘-3.5+首推赢球不穿盘比分。
§
⚠️改config.yaml必须terminal Python读CC-Switch DB取Key+yaml.dump，patch/write_file触脱敏破坏Key。2026-06-19翻车。
§
一步API：gpt-image-2≈0.06元/张，Key:skills/.img_key。编辑模式(参考图+改换装/道具/去元素)远优于从零生成。端点yibuapi.com/v1。
§
备份cron: GitHub(beee2bef6b07,每天3:00)+MEGA(987d004a0798,每天4:00)。找不到旧技能/模块先翻MEGA对应日期的skills-YYYYMMDD.tar.gz。56模块系统(multi-agent-orchestrator-handbook)从MEGA 6月9号skills-0609恢复，原会话20260609_071239_d8beb84b。
§
配置管理：仅construction一个profile。改配置用`hermes config set`（别patch/write_file免脱敏翻车）。DeepSeek reasoning_effort默认空(关)，用户偏好medium，设法：`hermes config set agent.reasoning_effort medium`。reasoning token算输出token计费(V4-Pro输出$0.87/1M)，medium≈2-4x输出量。
§
红果短剧Q版角色：大头修长身(非圆滚滚)+瓜子脸+杏仁眼+剑眉。Ideogram iPhone免费额度可用。API Key已得但付费。
§
代理：Clash 127.0.0.1:7897，浏览器+curl都走代理。liblib.art✅，ideogram.ai❌403。
§
用户有 Gemini API Key，可用于 Gemini 2.5 系列模型的画图（Imagen 3）/参考图编辑功能。目前尚未配进 Hermes。
§
双机架构：旧机(2核4G无GPU/onnxruntime崩/网络差)QQ Bot日常；新机(GPU/网络好)未配完Hermes。Tailscale两台都装不上(精简Win缺组件MSI 1603)。长线：新机Telegram Bot独立在线做剪映动漫，旧机QQ日常，双机GitHub共享记忆。新机装Hermes：ghfast.top下zip→解压→uv venv→uv pip install -e。GitHub代理ghfast.top。
§
旧机2核4G无GPU，onnxruntime/torch DLL加载全崩(ImportError: DLL init failed, VC++已装但.pyd不兼容)，winget损坏，PowerShell/WMI卡死。不适合跑任何编译库Python包(rembg/onnx/torch)。
§
中国网络下载GitHub文件：ghfast.top ✅（支持git clone/wget/curl/zip），ghproxy.com ⚠️（间歇可用），gitclone.com ❌（已失效）。格式：`https://ghfast.top/https://github.com/...`。ghfast不支持二进制/exe/msi直链（会报Invalid input），仅支持源码/文本/zip。