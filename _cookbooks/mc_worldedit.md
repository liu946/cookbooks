---
layout: cookbook
title:  "MC-WorldEdit"
categories: 游戏
style: compact
---

选区
---
- `//pos1` `//pos2` 选择你的当前位置(所站的方块上方一个方块)
- `//expand <数量> [反方向数量] [方向]` 扩展选区。
- `//expand vert` 扩大选区到基岩和天空

> `//contract` 为缩小

功能性
---
- `//count torch` 计数
- `//distr [-d]` 分布。-d参数对不同附加值单独统计。

基本操作
---
- `//set <target>`
- `//replace [source] <target>` 将source替换为target，source默认为所有非空气方块。
- `//stack <次数> [方向]` 向某方向（默认看向的方向）重复选区多次。
- `//move <距离> [方向] [填充方块]` 向一个方向（默认me，朝向）移动。


高级操作
---
- `//smooth` [迭代次数]
- `//regen` 根据种子重新生成选区
- `//naturalize` 草方块，3x泥土，n x原石方块的构造对选区内方块进行替换。
- `//flora`

剪贴板
---
- `//copy`
- `//paste [-aso]` 相对位置粘贴。-o会粘贴到原始选区位置。
- `//rotate <角度>`
- `//flip [-p] [方向]`
- `//<schematic|schem> <save|load> [<格式>] <文件名>`
- `//<schematic|schem> <''list''> [-dn]`

生成
---
> 这些指令都是以你站的方块为准的。不需要选区。

- `//cyl <方块> <半径> [高度]` 创建实心圆柱，空心使用`hcyl`指令。半径可以替换为`<东西半径>,<南北半径>`用以生成椭圆。
- `//sphere [-r] <方块> <半径>` 生成球。空心使用`hsphere`指令。`-r`参数，会生成升高的球。你会踩在他内部的底上。
- `//sphere <方块> <半径>,<半径>,<半径> [-r]` 椭球
- `//pyramid <方块> <大小>` 金字塔
- `//forestgen 10 tree 0.5` 在10x10范围生成0.5%密度的森林
- `//pumpkins 5` 在5x5范围生成南瓜丛