this seems like the logical starting place. i did initially google if i could just yank the source, and then somewhere on the noita wiki there's a thing about how to do mods. all i know is that it's lua and completely bespoke. also i guess i'm really after the worldgen stuff? if we can read the world gen code, then maybe could take a known seed with eyes (are they in all seeds? idk, don't care yet either), step through the loading of that seed and watch for eyes to come to life. who knows what we'll see. anyway here's wonderwall:

# goal

try to understand noita worldgen and noita modding. maybe we can do something cool.

## tools'n'things

* https://noita.wiki.gg/wiki/Modding - probably good. so there's a modding api. i might have to use vscode. gross. let's start by unpacking data.wak. we love spreadsheets! `-wizard_unpak` hehe cool.

## understanding noita

* https://nothings.org/gamedev/herringbone/

herringbone wang tiles. interesting. if you're getting into noita you may have heard of [formations](https://noita.wiki.gg/wiki/Formation) which are just special tiles that can contain rewards.

#### so, what is a tile?

the noita world is composed of tiles, basically a set puzzle pieces that you can randomly select. instead of laying these out on a grid, we have variable-sized tiles that get packed together. cool. fix this later, we don't understand quite yet.

#### pixel scene
