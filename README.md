# Ikemen GO - BGM Select Module
External Module for [**Ikemen GO Engine**](https://github.com/ikemen-engine/Ikemen-GO) that adds BGM Select to Stage Select Menu.

Tested in Ikemen GO: **v0.98.2**, **v0.99.0** and **2024-08-14 Nightly Build**.

- **Auto** Option works like stage select default song assignment (Uses select.def or stage.def music added).
- **Random** Option will select a random music stored in "**./sound**" directory.
- Custom BGM will show all the sounds that you have stored in the "**./sound**" directory and you can use them for stage selected.

https://github.com/user-attachments/assets/22595272-1685-47e7-ab48-62f848a1dcc6

##  _Installation:_
1- Extract archive content into "**./external/mods**" directory

2- IMPORTANT! **HOW TO FIX bgmSelect.lua:124** error:
GO TO "**./external/script/start.lua**" AND FOR "**local stageListNo = 0**"
remove "**local**" and save the file to that stage select works with this module...

3- New SYSTEM.DEF parameters assignments in [Select Info] Section:
>;BGM Select
>
>bgm.move.snd = 100,0
>
>bgm.pos = 160,164
>
>bgm.active.font = 3,0,0
>
>bgm.active2.font = 3,2  ;Second font color for blinking
>
>bgm.done.font = 3,0
>
>bgm.text = "BGM %i: %s"
>
>bgm.random.text = "BGM: Random"
>
>bgm.auto.text = "BGM: Auto"
