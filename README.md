# 枫灵快播

枫灵快播（FengTVStream）是一款~~通过在 `OTT 终端` 上播放 `串流内容`、提供与`传统电视`相似体验，~~帮助用户直观地判断各直播源的`延迟情况`以`调整网络设置`的软件。

## 注意

[国家广播电视总局科技司关于对《有线电视业务技术要求》等三项广播电视和网络视听行业标准报批稿进行公示的通知](http://www.nrta.gov.cn/art/2023/10/25/art_113_65927.html)

软件仅供学习使用，**切勿用于非法用途**。

### 工作原理

软件通过自带的 `live.m3u`，建立列表并进入播放，监听 `活动按键事件` 执行对应操作（换源、展示播放源列表等）

##### 特点

- 启动快速：开屏即是直播页面。
- 操作简便：与传统电视的换源、数字切换播放源操作方式基本相同，上手轻松，学习成本低。
- 兼容性强：考虑到 `Android 版本` 的兼容及开发成本，软件使用 `iApp` 开发，其带来的是最低可至 `Android 4.0.3` 的极强兼容性，几乎可在`所有 Android 电视`上运行。
- 设计人性：软件设计风格简洁，无任何多余功能，无内建更新，且初次时候`无需任何配置`即可直接开播。软件具有记忆上次频道的功能，每次启动时会回至上次频道。
- 播放源多：160+ 可用。后期可能会开放允许自定义播放源列表。

### 运行截图

![播放页面]()

![播放源一览]()

![数字换源]()

### 基本操作

#### 单次换源

按遥控器 `↑` / `↓` 键进行换源，`↑` 键调至下一个源，`↓` 键调至上一个源

#### 音量调整

按遥控器 `←` / `→` 键进行音量调整，`←` 键调小音量，`→` 键调大音量

**（Tips：部分电视遥控器上已有音量调节键，在此情况下按 `←` / `→` 键仍为调节音量）**

#### 播放源一览

在 `正常播放` 状态下，按遥控器 `OK` / `确认` 键唤出播放源列表。

此时按遥控器 `↑` / `↓` 键可移动选择光标选中播放源，再按 `确认` 键将调至选中的播放源，或再按 `返回` 键关闭播放源菜单。

#### 数字换源

软件内置的数字换源系统最高支持 `三位数` 播放源，超过将无法使用该方式换源。

仅带有 `数字键盘` 的电视遥控器才可使用该功能。

数字不支持 `回退清除`，但输满三位数后，再输入会 `清除` 之前的三位数。

系统将在按下最后一个数字的 `1800 ms` 后执行换源操作。若输入的播放源序号不存在，输入的数字消失后无动作。
