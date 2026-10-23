oh hey, noita has a tools_modding/READ_ME_FIRST.txt. we also love to read. game recognize game.

let's make a `NOITA_HOME` env var in bashrc. we might need to use that a lot. if you have noita installed and `NOTIA_HOME` set, i can write down clickable links here. that's fun!

oh shit! there's a noita readme. cool! let's make makefile in the root. i want `make link` to make a symlink in here to `NOITA_HOME` for easier exploration in there. gogogo!


we get the following nugget:

```
Some arcane secret spells
---

Type %appdata%\..\LocalLow\Nolla_Games_Noita\ to your explorer of files and 
more secrets will be revealed to you.
```

i've included the original trailing space, which i find distasteful.

windows is gross, but surely we can find this. is this just the save dir? that's probably in...
something like this `~/.local/share/Steam/steamapps/compatdata/<APPID>/pfx/drive_c/users/steamuser/AppData/`

app id, should get that and export it in `~/.bashrc` as well. whoa, cool number: `881100`.

okay, let's move this commentary into a field notes.md folder and yap there, this document should be nice and clean. well, that document now. doesn't matter. what's next?

`noita_dev.exe` is interesting


from `$NOITA_HOME/_release_notes.txt`
```
MODDING: Lua API documentation - added generate_lua_documentation.lua which will some day implement API doc generation


Congrats, you are the Master of Scrolling!
```

i am the master of scrolling.

let's go read https://noita.wiki.gg/wiki/World_generation

* `Wang tiles` and `Pixel scenes` lol

so tiles are rectangles that we make a herringbone pattern with. and pixel scenes are images where pixels represent materials.

let's look in `$NOTIA_HOME/data`

---

okay i couldn't help myself. i'm looking in `$NOTIA_SAVE_DIR/save00/stats`.  wtf is `_stats.salakieli`?

okay, this seems useful: https://noita.wiki.gg/wiki/Technical:_File_Formats

---

my wife thinks this is a good and cool idea, so it's obviously a good and cool idea.

there are many directions to take, but i think we must understand the gods. fortunately, they are just very smart and cool humans that exist in the world. let's use that.

i've got a lot of ideas, but first we continue to get a lay of the land. also i have some things to build. hmmm.
