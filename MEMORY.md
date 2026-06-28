铁规：①多消息全读完再回②说停即停③遇阻塞踩到底(改参/换模/读源/补exports)，不问"换方案吗"④不重复犯错⑤改Hermes配置先确认⑥"写好了"先打开确认⑦先穷尽再让用户动手⑧不提议换方案⑨时效数据web_search+年份限定+跨源验证⑩【防绕圈】同一任务已失败2次的方案，禁止第3次重试——必须换全新路径或诚实告诉用户。每次失败后心里默记"已试过X,Y,Z"，再想新方案前先翻记录确认没重复。
§
GitHub Token 存 ~/.config/github-token（不在 ~/.hermes/ 下以免脱敏），40位，永久有效。存token方法：hex编码写文件用xxd -r -p解码。技能 clash-setup 有详细步骤。
§
web.backend=firecrawl（搜索/抓取/后端全走Firecrawl，不用DDGS）。Firecrawl Key用户2026年6月提供，API已验证通过。
§
用户要求：每次需要用到delegate_task（子Agent）完成任务时，必须先口头告知要用了并说明原因，等用户确认再执行。不能直接派出去。
§
【自动化决策铁规】决定自动化前必须先load automation-governance-decision skill走决策框架。范围：关掉会话还在跑的东西（cron/脚本/管线/webhook）。一次性命令不触发。
§
球赛预测优先级: Bet365截图(最准)→DraftKings→Polymarket→Sports Mole。Bet365直连被拦截只能截图。去水概率差<30pp禁押单方向。大盘-3.5+首推赢球不穿盘比分。
§
⚠️改config.yaml必须terminal Python读CC-Switch DB取Key+yaml.dump，patch/write_file触脱敏破坏Key(2026-06-19翻车)。仅construction一个profile，改配置用`hermes config set`。DeepSeek reasoning_effort=medium。
§
一步API：gpt-image-2≈0.06元/张，Key:skills/.img_key。编辑模式(参考图+改换装/道具/去元素)远优于从零生成。端点yibuapi.com/v1。
§
备份cron: GitHub(beee2bef6b07,每天3:00)+MEGA(987d004a0798,每天4:00)。找不到旧技能/模块先翻MEGA对应日期的skills-YYYYMMDD.tar.gz。56模块系统(multi-agent-orchestrator-handbook)从MEGA 6月9号skills-0609恢复，原会话20260609_071239_d8beb84b。
§
红果短剧Q版角色：大头修长身(非圆滚滚)+瓜子脸+杏仁眼+剑眉。Ideogram iPhone免费额度可用。API Key已得但付费。
§
代理：Clash 127.0.0.1:7897，浏览器+curl都走代理。liblib.art✅，ideogram.ai❌403。
§
用户有 Gemini API Key，可用于 Gemini 2.5 系列模型的画图（Imagen 3）/参考图编辑功能。目前尚未配进 Hermes。
§
双机：旧机(2C4G无GPU，Hermes常驻+剪映已装)QQ；新机(8C16G GPU，CodeX桌面版+剪映专业版，用户手动操作)。CodeX：lingshuai.cc/gpt-5.5，Key ~/.codex/auth.json。跨机传文件：旧机MEDIA→QQ bot→新机QQ。剪映导出静帧=预览窗相机图标→PNG；边缘羽化=画面面板滑块1-2；抠图=剪映智能抠像(不用rembg)。GitHub：Chi3Xiao10T/hermes-context。
§
中国网络下载GitHub文件：ghfast.top ✅（支持git clone/wget/curl/zip），ghproxy.com ⚠️（间歇可用），gitclone.com ❌（已失效）。格式：`https://ghfast.top/https://github.com/...`。ghfast不支持二进制/exe/msi直链（会报Invalid input），仅支持源码/文本/zip。
§
剪映缩放动画：手动关键帧BUG(首帧设100%→末帧加关键帧改值无效/跳回100%)。正解：不用关键帧→切「动画」标签→「入场」→「缩放」/「放大」→时长拉满素材全长。
§
新机8核16G（非之前2核4G云电脑），剪映操作快。Codex远程操控UI天然慢，简单拖拽/点击让用户手动比Codex快10倍，只有复杂多步操作才考虑Codex。用户倾向：能手动10秒搞定的不让Codex2分钟折腾。