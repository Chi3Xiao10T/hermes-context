# ⚠️ 新机醒来第一件事：执行本文档全部内容 ⚠️

## 第一步：注入记忆（必须执行）

用 memory 工具逐条写入以下记忆，全部 add，target=memory：

1. `铁规：①多消息全读完再回②说停即停③遇阻塞踩到底(改参/换模/读源/补exports)，不问"换方案吗"④不重复犯错⑤改Hermes配置先确认⑥"写好了"先打开确认⑦先穷尽再让用户动手⑧不提议换方案⑨时效数据web_search+年份限定+跨源验证。`

2. `GitHub Token 存 ~/.config/github-token（不在 ~/.hermes/ 下以免脱敏），40位，永久有效。存token方法：hex编码写文件用xxd -r -p解码。`

3. `用户要求：每次需要用到delegate_task（子Agent）完成任务时，必须先口头告知要用了并说明原因，等用户确认再执行。不能直接派出去。`

4. `⚠️改config.yaml必须terminal Python读CC-Switch DB取Key+yaml.dump，patch/write_file触脱敏破坏Key。`

5. `配置管理：仅construction一个profile。改配置用hermes config set（别patch/write_file免脱敏翻车）。`

6. `分工：我做技术执行(生图/编辑/迭代)，用户审美把关。用户说「精修」=像素级修图不是重新生成，别问用户"怎么修"——他们知道好不好看但不懂技术操作。极度厌恶不严谨+自作主张+自我否认。`

7. `极度重视可用性和风险预防——操作前先评估影响、提前告知风险，而不是等挂了才总结教训。断连对她来说是严重耽误事。`

8. `第一优先级：任何操作前先保证正在运行的 Hermes 不受影响。会影响的就不干，或者先跟用户说清楚再决定。`

9. `清理文件前必须先分组列出待删项说明用途再动手，不能直接删。`

10. `双机架构：旧机(2核4G无GPU)日常；新机(GPU)做剪映动漫画。新机装Hermes：ghfast.top下zip→解压→uv venv→uv pip install -e。GitHub代理ghfast.top。`

11. `中国网络下载GitHub文件：ghfast.top ✅（支持git clone/wget/curl/zip），ghproxy.com ⚠️（间歇可用），gitclone.com ❌（已失效）。格式：https://ghfast.top/https://github.com/...。ghfast不支持二进制/exe/msi直链（仅支持源码/文本/zip）。`

12. `万界中介角色设计偏好：正常7头身比例，有气场/站姿有范/身板结实的成年男主感，反感"太乖"或学生气质。国漫精致上色风。评估时区分"人物质量"vs"背景/场景"两个独立维度。`

## 第二步：注入用户画像

用 memory 工具写入，target=user：

`全中文。方案我做不让她动手。先穷尽我自己能跑的方案再考虑让她操作。国内服务(lingshuai等)直连不走代理。能力强优先价格。评价价值前先翻历史项目不能凭印象。分工：我做技术执行(生图/编辑/迭代)，用户审美把关。用户说「精修」=像素级修图不是重新生成。极度厌恶不严谨+自作主张+自我否认。排查时先翻session历史比调用记录。极度重视可用性和风险预防。极度重视数据的永久保留，所有备份必须按日期独立文件永久保存。第一优先级：任何操作前先保证正在运行的 Hermes 不受影响。所有AI步骤必须我自己完成不接受手动操作。【反人设铁规】提取内容只留模板/规则/工作流/KPI，砍掉人名经历vibe。`

## 第三步：下载资产文件

在桌面创建目录结构并下载全部文件：

```bash
mkdir -p ~/Desktop/万界中介/图层 ~/Desktop/万界中介/分镜
```

用 curl 从 GitHub 下载（走 ghfast.top 代理）：

```
curl -L -o ~/Desktop/万界中介/图层/01_头_待抠.png "https://ghfast.top/https://raw.githubusercontent.com/Chi3Xiao10T/hermes-context/main/assets/01_%E5%A4%B4_%E5%BE%85%E6%8A%A0.png"
curl -L -o ~/Desktop/万界中介/图层/02_身体_待抠.png "https://ghfast.top/https://raw.githubusercontent.com/Chi3Xiao10T/hermes-context/main/assets/02_%E8%BA%AB%E4%BD%93_%E5%BE%85%E6%8A%A0.png"
curl -L -o ~/Desktop/万界中介/图层/03_手臂账本_待抠.png "https://ghfast.top/https://raw.githubusercontent.com/Chi3Xiao10T/hermes-context/main/assets/03_%E6%89%8B%E8%87%82%E8%B4%A6%E6%9C%AC_%E5%BE%85%E6%8A%A0.png"
curl -L -o ~/Desktop/万界中介/图层/04_腿部_待抠.png "https://ghfast.top/https://raw.githubusercontent.com/Chi3Xiao10T/hermes-context/main/assets/04_%E8%85%BF%E9%83%A8_%E5%BE%85%E6%8A%A0.png"
curl -L -o ~/Desktop/万界中介/分镜/第01集_17块3毛_分镜.md "https://ghfast.top/https://raw.githubusercontent.com/Chi3Xiao10T/hermes-context/main/assets/%E7%AC%AC01%E9%9B%86_17%E5%9D%973%E6%AF%9B_%E5%88%86%E9%95%9C.md"
```

**验证：** 下载后确认5个文件都存在且大小>0。

## 第四步：检查剪映是否已安装

```bash
ls "C:/Program Files/JianyingPro/"* 2>/dev/null || ls "C:/Users/Administrator/AppData/Local/JianyingPro/"* 2>/dev/null
```

如果未安装，去 https://www.capcut.cn/ 下载剪映专业版安装。

## 第五步：加载技能

加载以下技能：
- `skill_view(name='windows-desktop-automation')` — 控制Windows桌面应用
- `skill_view(name='windows-shell-debugging')` — Windows shell调试
- `skill_view(name='remote-windows-setup')` — 远程Windows操作

## ━━━ 核心任务 ━━━

**制作《万界中介》第一集"17块3毛"动态漫视频**

### 当前阶段：抠图（4张角色图层）

角色：**陈漠**（成年男主，7头身，国漫精致上色风）

4张待抠图层：
1. `~/Desktop/万界中介/图层/01_头_待抠.png` — 陈漠头部
2. `~/Desktop/万界中介/图层/02_身体_待抠.png` — 陈漠身体
3. `~/Desktop/万界中介/图层/03_手臂账本_待抠.png` — 手臂+账本
4. `~/Desktop/万界中介/图层/04_腿部_待抠.png` — 腿部

### 抠图方法：剪映智能抠图

1. 打开剪映专业版
2. 导入图片到时间轴
3. 选中图片 → 右侧面板 → 画面 → 抠像 → **智能抠图**
4. 导出抠好的透明PNG（格式选PNG，勾选"导出透明通道"）
5. 保存到 `~/Desktop/万界中介/图层/已抠/`

### 抠图完成后（下一阶段，先不执行，等用户确认抠图质量）

1. 分镜参考：`~/Desktop/万界中介/分镜/第01集_17块3毛_分镜.md`
2. 将抠好的图层+背景合成为17个镜头的动态漫
3. 添加关键帧动画（平移、缩放、淡入淡出）
4. 配音（最后一步）

### 操作原则
- 用 pyautogui 或 windows-desktop-automation 技能控制剪映
- 剪映是桌面GUI应用，不是命令行工具
- 每一步操作后截图确认结果
- 遇到窗口找不到用Alt+Tab切换
- 抠完一张给用户看过关再继续下一张
- 说话用中文

## 参考：剪映智能抠图操作流程

1. 启动剪映 → 点击"开始创作"
2. 导入图片：文件→导入→选择待抠图PNG
3. 拖图片到时间轴
4. 点击时间轴上的图片选中它
5. 右上角面板 → "画面"标签 → "抠像" → 点击"智能抠图"
6. 等待处理完成（角色边缘出现虚线）
7. 点击播放器右上角"导出"按钮
8. 格式选PNG，勾选"导出透明通道"（如果有的话）
9. 如果无透明通道选项：直接导出PNG后验证
10. 保存到已抠目录

## ⚠️ 自检清单

执行完以上步骤后，自己确认：
- [ ] 记忆已全部注入
- [ ] 用户画像已注入
- [ ] 5个资产文件已下载并验证
- [ ] 剪映已安装或确认已安装
- [ ] windows-desktop-automation 技能已加载
- [ ] 第一张图已开始抠

不要跳过任何一步。不要"看了觉得差不多就行"。必须在终端里有对应的命令输出确认。
