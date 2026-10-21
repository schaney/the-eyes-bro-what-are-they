this seems like the logical starting place. i did initially google if i could just yank the source, and then somewhere on the noita wiki there's a thing about how to do mods. all i know is that it's lua and completely bespoke. also i guess i'm really after the worldgen stuff? if we can read the world gen code, then maybe could take a known seed with eyes (are they in all seeds? idk, don't care yet either), step through the loading of that seed and watch for eyes to come to life. who knows what we'll see. anyway here's wonderwall:

# goal

try to understand noita worldgen and noita modding. maybe we can do something cool.

## tools'n'things

* https://noita.wiki.gg/wiki/Modding - probably good. so there's a modding api. i might have to use vscode. gross. let's start by unpacking data.wak. we love spreadsheets! `-wizard_unpak` hehe cool.

oh hey, noita has a tools_modding/READ_ME_FIRST.txt. we also love to read. also game recognize game.

let's make a `NOITA_HOME` env var in bashrc. we might need to use that a lot. if you have noita installed and `NOTIA_HOME` set, i can write down clickable links here. that's fun!

oh shit! there's a noita readme. cool! let's make makefile in the root. i want `make link` to make a symlink in here to `NOITA_HOME` for easier exploration in there. gogogo!
