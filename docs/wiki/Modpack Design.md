# 自定义超限速大逃杀设计

**消除垃圾时间，来一场“快速硬核生存竞技”**

自定义超限速大逃杀（CFHC）整合包旨在利用模组服的技术优势，系统化地修复传统UHC的效率问题和PUBG的门槛问题，致力于打造**“快速硬核竞技”**。

### 核心技术基础：模组服框架的高自由度

CFHC的所有核心机制均运行在Forge/NeoForge模组服框架上。这种框架提供了超越API驱动的插件服的**高定制化能力**。

|技术领域|模组服+CFHC实现|插件服限制|设计优势|
|:--|:--|:--|:--|
|几何形状与渲染|客户端原生**圆形/球形**区域渲染、黄金螺旋出生点|只能实现原版正方形边界|竞技专业度：告别简陋的方块边界，保障出生点的绝对公平|
|性能与视觉|Sodium/Embeddium优化 + Biomes O' Plenty地形|无法干预客户端 FPS 或渲染|低门槛的基础设施：以**极低的配置门槛**，提供高质量的视觉基础|
|精细机制|装备耐久度NBT标签精确控制、轰炸区/空投等**复杂动态事件**|难以实现复杂的NBT调整，事件和物资刷新单调|深度策略性：利用精细的数值控制，在“物资低耐久 vs 满耐久”之间创造资源博弈|

### 玩法理念：融合、优化与节奏重塑

CFHC保留UHC的深度，并注入PUBG的速度，**预期在 25 分钟**内即可为玩家提供持续的高强度对抗。

|玩家体验目标|CFHC机制设计|解决的传统模式痛点|
|:--|:--|:--|
|消除垃圾时间|初始物资 + 神速稿直接跳过15-20分钟低效采集|解决UHC发育期过长导致的玩家流失问题|
|公平与容错|黄金螺旋出生 + 30秒无敌 + 5秒倒地免伤|消除PUBG式的“落地成盒”现象，提升新手的留存率和团队容错性|
|终局控制|阶段5球体毒圈 → 向(0,64,0)移动|彻底终结了Minecraft竞技模式中“挖地道”的沉闷战术，保障最终 PVP 的观赏性|
|动态对抗|动态调整毒圈中心（受玩家聚集吸引）+ 周期性轰炸/空投|避免地图僵化，强制玩家持续跑图和交火，提升了比赛的紧张感|

### 设计目标

CFHC的设计旨在实现两大核心目标：**时间效率**和**框架扩展性**。

1. 时间效率的设计目标：将UHC的核心乐趣浓缩进25分钟的对局。这种高效的竞技时长能够兼容更多玩家的游戏时间，避免了传统UHC单局时间过长，导致玩家“输掉一把就输掉一整天”的挫败感。
2. 框架扩展性：模式基于CBR核心模组提供竞技规则，得益于模组服提供的高定制化能力及CBR现成的高度自定义的配置文件，该平台能够方便衍生出**枪械、魔法、大战场**等多种PVP玩法。
3. 模组服优势：Forge/Neoforge框架具备添加Sodium/Embeddium等性能优化模组的能力（尽可能降低硬件门槛），同时Biomes O' Plenty可提供超越原版的地貌基础（视觉升级）。

# English

**Eliminate Downtime for a "Fast-Paced Hardcore Survival Arena"**

The Custom Fast Hardcore (CFHC) modpack aims to utilize the technical advantages of modded servers to systematically address the efficiency issues of traditional UHC and the barrier to entry of PUBG, striving to create **"Fast-Paced Hardcore Competition."**

### Technical Core: The High Flexibility of Modded Server Frameworks

All core mechanisms of CFHC run on Forge/NeoForge modded server frameworks. This framework offers **high customization capability** that surpasses API-driven plugins.

|Technical Domain|Modpack + CFHC Implementation|Plugin Server Limitations|Design Advantage|
|---|---|---|---|
|Geometry and Rendering|Client-side native **Circular/Spherical** zone rendering, Golden Spiral spawn points.|Limited to original square boundaries.|Competitive Professionalism: Eliminates crude block boundaries and ensures absolute fairness of spawn points.|
|Performance and Visuals|Sodium/Embeddium optimization + Biomes O' Plenty terrain.|Cannot interfere with client FPS or rendering.|Low-Barrier Foundation: Provides a high-quality visual foundation with **extremely low hardware requirements.**|
|Granular Mechanics|Item durability NBT tag precise control, **complex dynamic events** like bombing zones/supply drops.|Difficulty in implementing complex NBT adjustments; events and loot refresh are simplistic.|Strategic Depth: Utilizes precise numerical control to create resource interplay between "low durability loot vs. full durability crafting."|

### Gameplay Philosophy: Fusion, Optimization, and Tempo Restructuring

CFHC retains the depth of UHC while injecting the speed of PUBG, **expected to provide** players with sustained high-intensity confrontation **within 25 minutes.**

|Player Experience Goal|CFHC Mechanism Design|Solved Traditional Mode Pain Point|
|---|---|---|
|Eliminate Downtime|Starting gear + "Godspeed Pickaxe" directly skips 15-20 minutes of inefficient gathering.|Solves the problem of player attrition caused by excessively long UHC development phases.|
|Fairness and Forgiveness|Golden Spiral spawn + 30 seconds of invincibility + 5 seconds of knockdown invulnerability.|Eliminates the PUBG-style "spawn-killing" phenomenon, improving novice retention and team forgiveness.|
|Endgame Control|Phase 5 spherical boundary → moving towards **(0,64,0)**.|Completely ends the dull tactic of "digging tunnels" in Minecraft competitive modes, ensuring the spectacle of the final PVP.|
|Dynamic Confrontation|Dynamic adjustment of zone center (attracted by player congregation) + periodic bombing/supply drops.|Avoids map stagnation, forcing players to constantly move and engage in combat, enhancing match tension.|

### Design Objectives

The design of CFHC aims to achieve two core objectives: **Time Efficiency** and **Framework Extensibility**.

1. Time Efficiency Design Goal: To concentrate the core fun of UHC into a 25-minute match. This efficient match length accommodates the gaming time of more players, avoiding the frustration of traditional UHC where a single loss can feel like "losing the whole day."
2. Framework Extensibility: The mode relies on the CBR core mod to provide competitive rules. Thanks to the high customization capabilities of the modded server and the readily available highly customizable configuration files of CBR, this platform can easily be leveraged to derive various PVP playstyles such as **gunplay, magic, and large battlegrounds.**
3. Modded Server Advantage: The Forge/NeoForge framework possesses the capability to integrate performance optimization mods like Sodium/Embeddium (to minimize hardware requirements), while Biomes O' Plenty offers a foundation of terrain that surpasses the vanilla game (visual upgrade).