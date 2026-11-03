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

---

just accidentally launched with the `wizard_unpack` flag or whatever it is. tonight we go in through the main entrance. will i die in today's daily? tbd.

okay, had to dig juuuuust a little bit. `ControllerGoombaAIComponent` gave me a chuckle. oh, hold on, lets grep for `eyes` or maybe the viking word for it.

```
piccolo.us-east-1  ~/dev/schaney/the-eyes-bro-what-are-they @main * grep -ir 'eyes' ./noita/data
grep: ./noita/data/fonts/generated/notosans_zhcn_20.bin: binary file matches
grep: ./noita/data/audio/Desktop/music01.bank: binary file matches
grep: ./noita/data/audio/Desktop/music.bank: binary file matches
grep: ./noita/data/audio/Desktop/music03.bank: binary file matches
grep: ./noita/data/data.wak: binary file matches
./noita/data/translations/common.csv:statusdesc_rainbow_farts,"Open your eyes, I see\nYour eyes are open\nWear no disguise for me\nCome into the open\n","Открывай глаза, вижу я\nТвои глаза распахнуты\nНе скрывай одеждами себя\nВыйди на открытое место ты\n","Abra os olhos, eu vejo\nSeus olhos estão abertos\nNão se disfarce para mim\nVenha para a vastidão\n","Abre los ojos, ya veo\nTienes los ojos abiertos\nNo te camufles ante mí\nVen al descubierto\n","Open your eyes, I see\nYour eyes are open\nWear no disguise for me\nCome into the open\n","Ouvrez les yeux, je vous vois\nVos yeux sont ouverts\nNe vous cachez pas face à moi\nVenez prendre l'air\n",Gli occhi aprirai\nPerché devi vedere\nDa me non ti nasconderai\nDevi farti valere\n,Otwórz szeroko oczy\nTwoje oczy są otwarte\nCzas śmiało kroczyć\nPrzez szlaki przetarte\n,睁开双眼吧，我看到了\n你的双眼睁开了\n不要在我面前掩掩藏藏\n开诚布公吧\n,目を開けば、見える\n君の目は開いている\n外装など無意味なこと\n自由になって\n,눈을 뜨세요\n당신이 눈을 뜬 게 보여요\n내 앞에서는 숨지 마세요\n탁 트인 곳으로 나와요\n,,Transliterate,,,,,,,,,,,
./noita/data/translations/common.csv:biomemodifierdesc_invisibility,You suddenly have trouble focusing your eyes...,Внезапно вам стало трудно сфокусировать взгляд...,"De repente, você não consegue mais focalizar a visão...",De repente tienes problemas para centrar la vista...,"Dir fällt es plötzlich schwer, deinen Blick zu fokussieren …",Vous avez soudain du mal à focaliser votre regard...,Di colpo hai difficoltà a focalizzare lo sguardo...,Masz nagle problem z ostrością widzenia...,你突然无法聚焦视线...,突然あなたの焦点が合わなくなってきました…,갑자기 시야가 흐려집니다...,,,,,,,,,,,,,
```

```
piccolo.us-east-1  ~/dev/schaney/the-eyes-bro-what-are-they @main * grep -ir 'øye' ./noita/data
grep: ./noita/data/audio/Desktop/music08.bank: binary file matches
```

maybe some breadcrumbs here. anyway, i've got a daily to play <3
