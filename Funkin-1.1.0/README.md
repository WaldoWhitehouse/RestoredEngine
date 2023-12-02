# FNF 1.1.0: Restored Engine

This is an FNF engine that runs off FNF 1.1.0. This engine runs exclusively off the built version. If you want to edit this using source, i'd reccomend downloading 1.1.0 Restored here: https://gamebanana.com/mods/481150.

# New Characters

You can create a new character by making a file with your character's name in "characterOffsets" folder with format: "idleoffsetx, idleoffsety, upoffsetx, upoffsety, rightoffsetx, rightoffsety, leftoffsetx, leftoffsety, downoffsetx, idleoffsety
change in character x, change in character y
change in camera x, change in camera y
is x flipped? (true/false)".

Add your character's assets (must be named excactly what your character is, xml file must use Idle, Up, Down, Left, Right only for the names of animations) into images and add your character's name is characterList.txt (located in assets/data). You can then use the animation editor (press 8 during a song, ijkl to move the camera, shift to go 10x as fast, arrow keys to move offsets, w and s to change which animation is currently playing) to configure the opponents offsets and the chart editor (needs no explanation) to select your character in the second dropdown box that has character selection.

# New Stages (backgrounds)

You can add a new stage by adding a folder labeled with the name of your stage, and inside there should be three png images labeled "front", "back", and "curtains" (which work the same as the regular fnf stage). You should also include a .txt file in stages with this format: "backx, backy, frontx, fronty, curtainsx, curtainsy". Then add an entry for your stage in stageList.txt (located in assets/data) and then select it in the chart editor.

# New Songs / Freeplay menu

To add a new song simply add your chart in the same way you would for the newer versions (I would reccomend you make the chart outside of 1.1.0) and add your songs audio into the music folder with the format: "yoursongname_Inst.ogg" and "yoursongname_Voices.ogg". You can then load the charts in the chart editor and configure the characters and stage from there. Then save your new chart and add your song as an entry in freeplayList.txt (located in assets/data).

# Story Mode

Download the FLA file from the "art" folder labeled "campaign_menu_UI_assets" and open it. Add your week selection graphic to it and export a sparrow V2 spritesheet with the symbols included being: week2 select, WEEK2, WEEK1 select, WEEK1, week 2 CANNOT select, NORMAL, lock, HARD, EASY, arrow right, arrow push right, arrow push left, arrow left, ontop of your week (which should be labeled: "[name of your week] select"). Add a .txt file with your week's name into the weeks folder (located in assets/data), and it should be formatted like this:
"
Songs here can be any amount
character left, character middle, character right
"
Currently the only selectable characters for the story mode menu are: "dad", "bf", "gf", "spooky". Then, simply add your weeks name to the file customWeekList.txt (located in assets/data).