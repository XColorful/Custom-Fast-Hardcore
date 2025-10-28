# 自定义超限速大逃杀

消除垃圾时间，来一场“快速硬核生存竞技”

- 初始化游戏：`/cbr game init`
- 切换地图中心：`/cbr game offset [x] 0 [z]`
- 加入队伍：`/cbr team join [teamId]`
- 开始游戏：`/cbr game start`

## 核心特色

- 极致轻量：整合包模组不到30个，使用Chunky预生成8000x8000地图仅需2小时
- 搜物资+原版发育：在随处可见的村庄搜集物资，或者快速下矿
- 一切都很快：初始物资+神速稿+密集村庄消除了大部分“垃圾时间”，游戏总时长为25分钟
- 安全开局：黄金螺旋分布的出生点位+开局30秒内全体无敌，告别“落地成盒”

### 核心优势

- 区域机制：客户端原生支持圆形、球形等非原版边界形状范围判定及渲染
- 快节奏：25分钟，初始加速，极低配置，碎片时间兼容
- 框架拓展性：整合包含高度自定义的配置文件，可通过额外添加模组快速转化为枪械/魔法等其他PVP形式
- 向后兼容：可以使用正多边形渲染、延长缩圈时间、减少建筑密度及取消物资刷新还原为UHC

## 游戏流程

游戏区域为半径500的圆内，缩圈共5阶段，每个阶段均为5分钟：
- 初始阶段：玩家出生点分布在半径400的圆内，边界半径从500缩小至400
- 第2/3/4阶段：阶段开始时生成轰炸区+物资区，区域中心受全体存活玩家的中心点吸引
- 第5阶段：安全区从圆变为球体，并逐渐缩小球半径，将地底玩家收回地表

### 详细说明

- 初始物资（9格）：效率X耐久Ⅲ木斧、效率X耐久Ⅲ铁镐、樱花木板x64、玄武岩x64、末影珍珠、工作台、熔炉、火把x16、营火x3
- 轰炸区在30s内半径不断扩大，每秒生成10个TNT随机轰炸，随后60s内随机生成物资掉落物
- 刷新的物资均为低耐久，而挖矿自造的为满耐久
- 所有容器都执行物资刷新，涵盖下界及末地物品
- 第5阶段的球体以全体存活玩家中心为起点，不断缩小并移动至(0,64,0)


## 整合包内容
按名称排序

### 大逃杀机制

- CBR addon by XiaoColorful
- Custom BattleRoyale by XiaoColorful

### 世界生成

- Better Villages by jtl_elisa, jtl_tom
- Biomes O' Plenty by Forstride, TheAdubbz
- ChoiceTheorem's Overhauled Village by ChoiceTheorem
- Chunky by pop4959
- Formations Overworld by SuperMartjin642
- GlitchCore by TheAdubbz
- MVS - Moog's Voyager Structures by finndog_123, olver___\_, havococcultist, TFA120
- Repurposed Structures by telopathicgrunt
- Towns and Towers by Biban_Auriu, Kubek

### 玩法扩展

- JourneyMap by techbrew, Mysticdrew, meme_sapiens
- PlayerRevive by CreativeMD

### 辅助模组

- Controlling by Jaredlll08
- Mouse Tweaks by YaLTeR
- Pick Up Notifier by Fuzs

### 优化模组

- Embeddium by FiniteReality
- ModernFix by embeddedt
- Sodium by JellySquid
