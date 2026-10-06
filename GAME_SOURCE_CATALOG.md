# 新火萤｜游戏源码目录

本页介绍新火萤的游戏工程与目录结构，涵盖客户端、服务端、二次开发版本和归档源码，方便按游戏名称或模块编号查找对应工程。

[返回游戏介绍](README.md) · [服务端与游戏模块](#服务端与游戏模块) · [其他客户端模块](#其他客户端模块) · [归档源码](#归档源码) · [配套工程](#配套工程)

## 工程概览

| 组成 | 目录规模 |
| --- | --- |
| 服务端游戏工程 | 47 个顶层目录，含 14 个二开目录；按 KindID 分为 28 组 |
| 客户端协议模块 | 63 个模块目录，分布在 61 个顶层游戏文件夹中 |
| 两侧游戏编号 | 合计 52 组，其中 24 组另列于客户端模块表 |

上述数量反映源码的组织结构。原版、二开、人数版本及主题分支分别保留目录；KindID 为工程中的游戏编号，同一编号下可以包含多个主题或版本，因此编号组数不等于独立玩法数量。

### 目录阅读说明

- 所有路径均相对于源码项目根目录，便于在本地工程中定位；不是公开下载链接。
- 名称以游戏名称或原始模块名列示，保留英文标识便于检索。
- `二开_` 表示二次开发版本，分号分隔同一编号下的多个目录。
- 表中的“—”表示该栏未列出对应编号的目录；Windows 客户端与压缩包源码另行展示。
- 表格按源码声明的编号组织，展示的是工程位置，不表示各历史分支可直接互换。

## 服务端与游戏模块

以下 28 个编号组列出服务端工程，以及同编号的 Lua 客户端目录。

| 编号 | 游戏或模块名称 | 客户端 Lua 源码目录 | 服务端源码目录 |
| --- | --- | --- | --- |
| 3 | 德州扑克 | `client/client/game/yule/dzshowhand/`；`client/client/game/yule/dzshowhandsixhy/` | `Server/子游戏/德州扑克/`；`Server/子游戏/二开_德州扑克/` |
| 6 | 诈金花 | `client/client/game/yule/zhajinhua/`；`client/client/game/yule/zhajinhuahy/` | `Server/子游戏/二开_诈金花/`；`Server/子游戏/诈金花/` |
| 16 | 五人21点 | — | `Server/子游戏/五人21点/` |
| 49 | 十三水 | — | `Server/子游戏/13水/` |
| 50 | 牛牛（含五人及二开目录） | `client/client/game/yule/oxsixx/`；`client/client/game/yule/oxsixxhy/` | `Server/子游戏/二开_牛牛/`；`Server/子游戏/牛牛/`；`Server/子游戏/五人牛牛/` |
| 104 | 百人牛牛（含抢庄版本） | `client/client/game/yule/oxbattle/`；`client/client/game/yule/oxbattlehy/` | `Server/子游戏/百人牛牛/`；`Server/子游戏/百人牛牛抢庄/`；`Server/子游戏/二开_百人牛牛抢庄/` |
| 122 | 百家乐（含抢庄版本） | `client/client/game/yule/baccaratnew/`；`client/client/game/yule/baccaratnewhy/` | `Server/子游戏/二开_新百家乐抢庄/`；`Server/子游戏/新百JL/`；`Server/子游戏/新百JL抢庄/` |
| 123 | 飞禽走兽 | `client/client/game/yule/animalbattle/`；`client/client/game/yule/animalbattlefqzs/` | `Server/子游戏/飞禽走兽/` |
| 124 | 奔驰宝马（服务端目录：碰碰车） | `client/client/game/yule/animalbattlebcbm/`；`client/client/game/yule/hhsw/` | `Server/子游戏/碰碰车/` |
| 131 | 红黑大战 / shuiguo | `client/client/game/yule/rhbattle/`；`client/client/game/yule/rhbattlehy/`；`client/client/game/yule/shuiguo/` | `Server/子游戏/二开_红黑大战/`；`Server/子游戏/红黑大战/`；`Server/子游戏/红黑大战/百人_红黑大战/` |
| 132 | 龙虎斗 | `client/client/game/yule/dtbattle/`；`client/client/game/yule/dtbattlehy/` | `Server/子游戏/二开_龙H/`；`Server/子游戏/龙虎斗/` |
| 200 | 斗地主 | `client/client/game/qipai/landhy/` | `Server/子游戏/斗地主/`；`Server/子游戏/二开_斗地主/` |
| 238 | 510K | `client/client/game/yule/510k/` | `Server/子游戏/510K/` |
| 302 | 血战麻将 | `client/client/game/yule/sharkbattle/sparrowxz/`；`client/client/game/yule/sparrowxz/` | `Server/子游戏/血战麻将FK/` |
| 392 | 二人麻将 / 红中二人麻将 | `client/client/game/yule/sparrowhztwo/` | `Server/子游戏/二开_二人麻将/`；`Server/子游戏/二人麻将/`；`Server/子游戏/红中麻将_二人/` |
| 407 | 新李逵劈鱼 | `client/client/game/yule/xlkpy/` | `Server/子游戏/新李逵劈鱼/` |
| 408 | 新摇钱树 | `client/client/game/yule/xyaoqianshu/` | `Server/子游戏/新摇钱树/` |
| 409 | 新金蝉捕鱼 | `client/client/game/yule/xjcby/` | `Server/子游戏/新金蝉捕鱼/` |
| 411 | 捕鱼（含二开版本） | `client/client/game/yule/dntg2/`；`client/client/game/yule/eypyhy/`；`client/client/game/yule/qpby/` | `Server/子游戏/捕鱼/`；`Server/子游戏/二开_捕鱼/` |
| 412 | 鳄鱼捕鱼 | — | `Server/子游戏/鳄鱼捕鱼/` |
| 413 | 千炮捕鱼 | — | `Server/子游戏/千炮捕鱼/` |
| 503 | 连环夺宝 | `client/client/game/yule/duobao/` | `Server/子游戏/连环夺宝/` |
| 516 | 财神到 / watermargin | `client/client/game/yule/shz/`；`client/client/game/yule/watermargin/` | `Server/子游戏/财神到/`；`Server/子游戏/二开_财神到/` |
| 517 | 水果拉霸 / jxlw | `client/client/game/yule/fruitslots/`；`client/client/game/yule/jxlw/` | `Server/子游戏/水果拉霸/` |
| 518 | 水浒传 | — | `Server/子游戏/二开_水浒传/`；`Server/子游戏/水浒传/` |
| 601 | 跑得快 / 湖南跑得快 | `client/client/game/yule/runfasthn/` | `Server/子游戏/二开_湖南跑得快/`；`Server/子游戏/二开_跑得快/`；`Server/子游戏/湖南跑得快/`；`Server/子游戏/跑得快/` |
| 655 | 水果机 | `client/client/game/yule/fruitmachine/` | `Server/子游戏/水果机/` |
| 706 | 六人德州扑克 | — | `Server/子游戏/德州扑克六人/` |

## 其他客户端模块

以下 24 个编号组展示其他 Lua 客户端模块，模块名与源码目录保持一致。

| 编号 | 游戏或模块名称 | 客户端 Lua 源码目录 | 服务端源码目录 |
| --- | --- | --- | --- |
| 25 | hkfivecardnew | `client/client/game/yule/hkfivecardnew/` | — |
| 26 | showhand | `client/client/game/yule/showhand/` | — |
| 27 | oxnew | `client/client/game/yule/oxnew/` | — |
| 36 | 通比牛牛 | `client/client/game/yule/oxsixex/` | — |
| 101 | redblack | `client/client/game/yule/redblack/` | — |
| 102 | oxex | `client/client/game/yule/oxex/` | — |
| 105 | redninebattle / zhongfabai / dzpk | `client/client/game/yule/redninebattle/`；`client/client/game/yule/zhongfabai/` | — |
| 106 | 海南牌九 | `client/client/game/yule/hainanpaijiu/` | — |
| 111 | sharkwanimal | `client/client/game/yule/sharkwanimal/` | — |
| 118 | 百人骰宝 | `client/client/game/yule/sicbobattle/` | — |
| 127 | sharkbattle | `client/client/game/yule/sharkbattle/` | — |
| 133 | longfengdou | `client/client/game/yule/longfengdou/` | — |
| 140 | luxurycar | `client/client/game/yule/luxurycar/` | — |
| 386 | sparrowzz | `client/client/game/yule/sparrowzz/` | — |
| 389 | sparrowhz | `client/client/game/yule/sharkbattle/sparrowhz/`；`client/client/game/yule/sparrowhz/` | — |
| 391 | sparrowgdex | `client/client/game/yule/sparrowgdex/` | — |
| 401 | gobang | `client/client/game/yule/gobang/` | — |
| 406 | shuiguolaba | `client/client/game/yule/shuiguolaba/` | — |
| 410 | dntg | `client/client/game/yule/dntg/` | — |
| 507 | fishry | `client/client/game/yule/fishry/` | — |
| 508 | line | `client/client/game/yule/line/` | — |
| 510 | fishlk | `client/client/game/yule/fishlk/` | — |
| 511 | fishyqs | `client/client/game/yule/fishyqs/` | — |
| 707 | luckstart | `client/client/game/yule/luckstart/` | — |

## 归档源码

部分客户端工程以压缩包形式保存在子游戏目录中。下表列出压缩包位置与包内协议文件，方便定位对应模块。

| 编号 | 压缩包路径 | 包内协议文件 |
| --- | --- | --- |
| 49 | `Server/子游戏/13水/thirteenx.zip` | `thirteenx/src/models/cmd_game.lua` |
| 105 | `Server/子游戏/二开_德州扑克/dzpk.zip` | `dzpk/src/models/CMD_Game.lua` |
| 132 | `Server/子游戏/二开_龙H/百人_龙虎斗.zip` | `dtbattle/src/models/CMD_Game.lua` |
| 105 | `Server/子游戏/德州扑克/dzpk.zip` | `dzpk/src/models/CMD_Game.lua` |
| 132 | `Server/子游戏/龙虎斗/百人_龙虎斗.zip` | `dtbattle/src/models/CMD_Game.lua` |

`Server/子游戏/水浒传dy.rar` 另存有 watermargin 客户端，协议编号为 516。部分归档同时保存在原版与二开目录中，按各自路径列出，重复副本不另计为新游戏。

## 配套工程

除 Lua 游戏模块外，项目还保留 Windows 客户端、界面资源与平台工程。例如，五人21点的 Windows/MFC 工程位于 `Server/子游戏/五人21点/客户端组件/GameClient.vcxproj`；十三水的 Lua 工程位于 `Server/子游戏/13水/thirteenx.zip`。

| 工程内容 | 项目内路径 |
| --- | --- |
| 大厅相关代码 | `client/client/client/` |
| Lua 游戏模块 | `client/client/game/` |
| 引擎与平台工程 | `client/frameworks/` |
| 平台及游戏服务 | `Server/` |
| Web 前台与管理后台 | `WebCode/` |
| 数据库相关文件 | `DB/` |
| 界面与资源工程 | `UI/` |
| 子游戏界面工程 | `UI_Game/` |

游戏场景及开发工程图片见 [项目介绍](README.md)。
