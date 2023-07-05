# mc-mt-syntax

为MT管理器编写的适用于Minecraft Addon编写的语法文件

目前只编写了适用于mcfunction文件的语法。之后可能会继续添加。比如json（如果可能分辨出来，否则也只能添加关键词高亮）

目前特色，五彩斑斓

注意，如果在使用的时候发现打开对应类型文件是空白的，或者写着写着写着就卡住或者崩溃了，请反馈给我，最好附带原文件或你当时正在写的命令，这样我才可以更快的找出问题所在（我在编写的时候发现了这个问题，后来修好了，但是难保以后不会出现，所以加上这个提醒）

## mcfunction支持

|命令       |高亮|纠错（简单）               |
|--------------------|-------|--------------------------------------------------|
|scoreboard|y   |只有operation中的操作符号  |
|function   |y   |     none            |
|execute    |y   |     if score 中的操作符         |
|titleraw    |y   |原始JSON文本               |
|tellraw     |y   |原始JSON文本               |
|xp        |y    |在使用负数时必须添加L/l标志才会高亮|
|say      |y     |      none |
|me      | y      | none      |
|title     |    y      |    none    |
|tell     |    y      | none      |
|gamemode |     y      | 只会对特定游戏模式高亮|
|gamerule |     y     |   none   |
|replaceitem|    y     | 可判断槽位是否正确|
|camera    |    y     | 可判断easeType是否正确|
|fill   |  y    | 可判断替换模式是否存在|
|setblock | y | 可判断替换模式是否存在 |
|effect | y | none |
|give | y | none |
|clear | y | none  |

支持大部分可在mcfunction中直接使用的命令的高亮（只能高亮命令本体）

对于/execute，如果你只想使用旧版，请在文件中将旧版的高亮匹配放出来，并将新版的匹配删除，然后安装即可

由于这只是一个语法高亮，所以难以实现真正的纠错

并且，基于高亮原理，无法为一些复杂参数（目标选择器参数、方块状态等）添加额外的颜色

## 链接

[MT管理器](https://www.coolapk.com/apk/bin.mt.plus)
[苦力怕论坛](https://klpbbs.com/thread-66574-1-1.html "适用于mt管理器的mcfunction语法高亮描述文件")

## 展示

（没更新，以后可能会更新）

![展示图1](./img/1.jpg)
![展示图2](./img/2.jpg)
![展示图3](./img/3.jpg)
![展示图4](./img/4.jpg)
![展示图5](./img/5.jpg)
![展示图6](./img/6.jpg)
![展示图7](./img/7.jpg)

