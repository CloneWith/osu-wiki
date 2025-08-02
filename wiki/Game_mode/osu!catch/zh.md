# osu!catch

osu!catch，也被称作 *Catch the Beat* 或 *CTB*，这个游戏模式需要玩家控制一个人物形象/托盘，按节奏*接住*下落的水果。

## 选歌页面

要切换到 osu!catch 游戏模式，可同时按下 `Ctrl` + `3`。

在 osu!(stable) 中可以点击 `Mode` 按钮并选择 `osu!catch`；在 osu!(lazer) 中也可以点击屏幕顶部的 ![osu!catch 的图标](/wiki/shared/mode/catch.png) 按钮来选择。

要下载更多 osu!catch 谱面，可以前往 osu! 网站的[谱面列表](https://osu.ppy.sh/beatmapsets)；使用 osu!(lazer) 时，也可以按下 `Ctrl` + `B` 或者点击`谱面列表`按钮来访问谱面列表。

![osu!(lazer) 谱面列表按钮](/wiki/shared/lazer_beatmap_listing.png)

## 玩家控制

在 osu!catch 中，玩家应随着音乐节奏控制屏幕底部的**小人**/托盘（Catcher，也被称作“Platter”）接住下落的水果。

控制小人移动的默认按键如下：

- 用左 <kbd>←</kbd>、右 <kbd>→</kbd> 箭头键或 <kbd>Z</kbd>、<kbd>X</kbd> 键移动小人。
- 按住 <kbd>Shift</kbd> 键或鼠标左键 <kbd>🖯</kbd> 可以激活*加速（Dash）*状态，标志是小人发出*白色光晕*，移动时留下残影。
  加速状态下小人的移速是正常速度的**两倍**，需使用加速接住的水果可以被称为*跳*。

正常游玩时，游戏内鼠标光标的位置并不重要。除非在启用 [Relax](/wiki/Gameplay/Game_modifier/Relax) [模组](/wiki/Gameplay/Game_modifier)时，小人会直接随光标移动。

## 打击物件

osu!catch 主要有三种可交互的[打击物件](/wiki/gameplay/Hit_object)：

- 大果 (Fruits)
- 水果串 (Juice streams)
- 香蕉雨 (Banana showers)

### 大果

![CTB 游戏内包含大果的截图](/wiki/shared/Catch_fruits.jpg "osu!catch 的大果")

**大果 (Fruits)** 是 osu!catch 中最基础的物件类型。玩家只需将小人移到大果下方，这样它就会掉落到盘子上，而不是错过它。

接到的大果会给出 `GREAT` 判定，每个大果给 300 分并增加 1 连击数。

### 水果串

**水果串 (Juice stream)** 一般首尾各有一个大果。在两端之间还会有由小果与中果组成的路径，其中中果即为[滑条点](/wiki/Gameplay/Hit_object/Slider/Slider_tick)。水果串与[滑条](/wiki/Gameplay/Hit_object/Slider)相似，也是可以折返的。

每个小果给出 10 分，不会影响连击；每个中果给出 30 分，接到时将增加 1 连击数。与小果不同的是，漏掉中果会导致断连。

### 香蕉雨

![CTB 游戏内包含香蕉雨的截图](/wiki/shared/Catch_bananas.jpg "香蕉雨期间")

在处于**香蕉雨 (Banana shower)** 中时，大香蕉会倾泻而下，由大到小。若未接到香蕉不会影响连击，但每接住一个会得到 1100 分，同时也会恢复一部分血量。每个香蕉的得分固定，与模组乘数和连击无关。

值得注意的是，[Auto](/wiki/Gameplay/Game_modifier/Auto) 模组更离谱，会接到*所有*的香蕉而不错过任何一个，这在正常游玩中是不可能做到的。

## 红果

![红果，以及正在进行红果跳的小人](/wiki/shared/Catch_hyperfruits.jpg "osu!catch 的红果")

**红果（Hyperfruits）** 也被称为 *Hyper*，是一种特殊的水果，当到下一个水果的距离太大，无法正常加速接住时会出现。

接到红果会将小人的跳（加速）升级为*红跳/大跳（Hyperdash）*，使小人足够快，以接到下一个水果。

进行红跳时，小人会发出红光，在接到红果的地方留下临时的*红色残影*。在接到或漏掉下一个水果前，红跳状态将会持续。

通常可以通过水果外围有明显的红色来认出红果。

## 难度参数

osu!catch 有三种难度参数，每种参数都对游玩过程有不同影响：

- [圆圈大小](/wiki/Beatmap/Circle_size)（Circle size）
- [掉血速度](/wiki/Beatmap/HP_drain_rate)（HP drain）
- [缩圈速度](/wiki/Beatmap/Approach_rate)（Approach rate）
- [判定严度](/wiki/Beatmap/Overall_difficulty)（Overall difficulty，仅限 ScoreV1）

这四种参数常被简写为 CS、HP、AR 与 OD。

在 osu!(lazer) 中，用户可以使用 [Difficulty Adjust](/wiki/Gameplay/Game_modifier/Difficulty_Adjust) 模组，酌情调整这些参数。

## 玩法

*主条目：[玩法#osu!catch](/wiki/Gameplay/Play_style#osu!catch)*

## 得分

[osu!catch 中的分数](/wiki/Gameplay/Score/ScoreV1/osu!catch)是游玩过程中多个部分的加权总和。其取决于以下因素：

- [判定](/wiki/Gameplay/Judgement)只为每个接到的打击物件提供固定分值，与打击准确度无关。
- [连击数](/wiki/Gameplay/Combo_(score_multiplier))是一个乘数：连击数较高时，完成一个打击物件会得到更高的分数，反之亦然。在 osu!catch 中，连击可能会因为漏掉大果或中果而[断掉](/wiki/Gameplay/Judgement/Combobreak)，同时[血量](/wiki/Gameplay/Health)也会减少。
- [准确度](/wiki/Gameplay/Accuracy#osu!catch)显示一共接住了多少物件，本身不会影响得分。漏掉小果时会降低准确率，但不会导致断连。

完成谱面后，会为分数[评级](/wiki/Gameplay/Grade#osu!catch) — 评价通常以单个字母为形式，是对准确度的简短评估。金色或银色的 SS 表示 100% 准确度，其他的评价（从 S 到 D）也取决于准确度。

## 自定义皮肤

*主条目：[osu!catch 自定义皮肤](/wiki/Skinning/osu!catch)*

## 作图

### osu! 转谱机制

- 原物件的水平位置决定大果（打击圈）或水果串（滑条）的下落位置。
- 和往常一样，谱面基于 [Timing 组](/wiki/Beatmapping/Timing/zh.md)与 [Combo 组](/wiki/Beatmapping/Combo)的设置。
- 水果串水平移动的速度与滑条的位置和[滑条速度](/wiki/Gameplay/Hit_object/Slider/Slider_velocity)有关。
- 转盘会变成香蕉雨。

**注意：** 红果是自动生成的。

## 冷知识

### 游玩

- [Auto](/wiki/Gameplay/Game_modifier/Auto) 模组*总是*会接住所有香蕉，玩家名称显示为 *“osu!salad”*。
- 在 osu!(stable) 中，当启用`打击偏差`指示计时，总会使用`色块模式`。
- 在[休息时段](/wiki/Beatmap/Break)期间是可以移动小人的。
- 小人失误（Miss）时的动画与 [osu!taiko](/wiki/Game_mode/osu!taiko) 中 pippidon 的失误动画很像。
- 最初的默认接水果小人是 *Ryuuta Ippongi* 的 Q 版形象（来自 [应援团系列](https://zh.wikipedia.org/wiki/Osu!_Tatakae!_Ouendan)）。2014 年后，他被现在的默认小人形象兼吉祥物 [*Yuzu*](/wiki/Mascots#yuzu) 替代。

### 历史

![特殊模式中的 osu!catch logo](/wiki/shared/Ctb_logo.jpg "一张特殊的 osu!catch 横幅")

- 在 2012 年 4 月 10 日之前，osu!catch 谱面无法上架，也无法被纳入排行谱面中。然而现在不会了，谱师可以制作包含 osu!catch 谱面的谱组并将其上架！只要合乎[上架标准](/wiki/Ranking_criteria/osu!catch)即可。
- 第一张至少含有一个 osu!catch 谱面的上架谱组是 [Yousei Teikoku - Dare so Ka no Gekka (TV Size)](https://osu.ppy.sh/beatmapsets/13676)，谱师是 ::{ flag=CN }:: [NatsumeRin](https://osu.ppy.sh/users/151679)，其中 [osu!catch 谱面](https://osu.ppy.sh/b/51945)的合作谱师是 ::{ flag=CN }:: [Uran](https://osu.ppy.sh/users/133302)。
- 第一张上架的 osu!catch 专谱是 [Rita - Hajimari no Toki](https://osu.ppy.sh/beatmapsets/91485)，谱师是 ::{ flag=ES }:: [Deif](https://osu.ppy.sh/users/318565)。
