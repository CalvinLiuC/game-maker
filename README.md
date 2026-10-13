# game-maker

一个卡牌构筑 roguelike 原型。核心机制是「翻倍引擎」：打出一张牌后，选择**加仓**（50% 翻倍，失败归零）或**平仓**（锁定结算）。每次加仓都要付手续费。没有怪物，节点是「合约」（在 3 手内凑够指定点数），Boss 是和庄家对赌。

设计文档：[docs/superpowers/specs/2026-10-13-gamble-roguelike-design.md](docs/superpowers/specs/2026-10-13-gamble-roguelike-design.md)

## 原型

`prototype/index.html` 是一个零依赖的单文件浏览器原型，双击即可玩。包含 8 份合约、三选一拿牌、手续费、庄家对赌三种性格，以及结束时的验证数据（贪心率、爆仓次数、最大连翻、手续费总支出）。不含商店和遗物。

## 状态

原型验证阶段。先玩原型确认「翻倍按钮」本身上头，再定正式技术栈。
