# crystar-Cheat-Engine
crystar的ct表
恸哭之星修改器

快七年了，网上一直找不到哭星的修改器（唯一一个在3dm找到的还用不了），而且这个游戏的战斗又枯燥的一批，一怒之下怒了一下，遂作此表。

由于本人对汇编一窍不通，所以仅有一些最基础的功能（想修改速度也无从下手，如果能的话以后再说吧）

注意：修改增加经验值并且升级后不能通过减少经验值达到降级的目的

It’s been nearly seven years, and I’ve never been able to find a working cheat table for Crystar. The only one I found (on 3DM) didn’t work either. And the combat in this game is just unbearably tedious. So I got pissed off — but all I could do was get pissed off — and in the end, I just made this table myself.

Since I know next to nothing about assembly, this table only has the most basic features. (I wanted to mod speed too, but I have no idea how — maybe sometime in the future if I figure it out.)

If your language is English, give this table to an AI and tell it to open it in text mode, then translate the Chinese characters inside into English — keeping in mind that some of the Chinese characters are abbreviations of game-specific terms

Note: After modifying to increase experience points and leveling up, you cannot reduce experience points to achieve a downgrade.

<img width="752" height="390" alt="image" src="https://github.com/user-attachments/assets/0c478fae-986b-488d-8526-297901290dba" />

---

## CRYSTAR_AllMap_Speed.CT

这份表在原表基础上额外提供了两个功能：

- **All Map Reveal**：进入关卡后直接显示完整地图，不再随着角色移动逐步点亮。
- **Global Speed x2**：全局 2 倍速，可通过 `Speed Multiplier` 调整倍率。

### 使用方法

1. 用 Cheat Engine 打开 `CRYSTAR_AllMap_Speed.CT`
2. 附加到 `CRYSTAR.exe`
3. 按需勾选：
   - `All Map Reveal`：建议在进入关卡前开启，或开启后重进一次关卡
   - `Global Speed x2`：开启后立即生效
4. 如需调整速度倍率，先启用 `Global Speed x2`，再修改 `Speed Multiplier` 数值

### 说明

- `All Map Reveal` 作用于地图生成阶段，因此在部分场景需要重进关卡才能看到完整效果。
- `Global Speed x2` 通过修改 `Time.get_deltaTime` 的返回值实现，不会修改游戏文件或存档。
- 建议先备份存档再使用修改器。

### Notes

- `All Map Reveal` affects the map generation stage, so you may need to re-enter a stage after enabling it.
- `Global Speed x2` works by modifying the return value of `Time.get_deltaTime`; it does not modify game files or saves.
- It is recommended to back up your save data before using this table.

