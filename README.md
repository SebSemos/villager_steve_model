<ins>Description not up to date!</ins> (WIP)
The 3 ressource packs are not up to fate with Villagers to Players yet neither!
Coming soon!









# Villager Steve Model

This page regroup instructions for 3 of my ressources packs available on [modrinth](https://modrinth.com/user/SebSemos) All of these using my [villagers to player](https://modrinth.com/resourcepack/villagers-to-player) villager model.


` I'll start with credits!`

[Song of war villagers](https://modrinth.com/resourcepack/songs-of-war-villagers) has been made following the animation of the same name on youtube. All the skins/textures and sounds come from the asset available [here](https://archive.blackplasma.xyz/songs-of-war/).

[Alex and Steve villagers](https://www.planetminecraft.com/texture-pack/alex-and-steve-villagers/) also took inspiration from the animated story of the same studio. This is why you have possibility to get the "Derp" skin in this pack. I did worked with vanilla Alex and Steve textures as a base. 

Hermitcraft villagers is using skins of famous youtubers currently playing on this smp. The skins I used have been taken via [NameMC](https://fr.namemc.com/) You can get the history of skin used by a player on this website.
Some custom items have been made by Stridey. He gave me authorization to use them. I don't know who made the rest. If you are the creator and don't want it to be shared in this pack, let me know :)
Custom sounds also come from the ressource pack of world download.

If you came accross these pack I assume you most likely know where they come from. If not, feel free to check out [Squared Media](https://www.youtube.com/@SquaredMediaAnimations) for the animations and [Hermitcraft](https://hermitcraft.com/) for the SMP.

Now for the mod needed to these pack to work you'll need
- [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures)
- [Entity Model Features](https://modrinth.com/mod/entity-model-features)
- Entity Sound Features
- [Chime](https://www.curseforge.com/minecraft/mc-mods/chime-fabric) is prefered to CIT Resnew to get custom items
- [Cit Resnew](https://modrinth.com/mod/cit-resewn)
- [Cit Resnew, Forge](https://www.curseforge.com/minecraft/mc-mods/forge-cit)


The Villager model has been worked from a port of [Fresh Animation](https://www.curseforge.com/minecraft/texture-packs/fresh-animations) By [Young SoulluoS](https://github.com/YoungSoulluoS/Fresh-Animations_cem_Fork) to make it compatible at the time with CEM fabric. Note: You now can directly use FA in fabric and forge thanks to EMF
All the base work has been made by them. I just changed the model and altered a few line of code here and there. Big thanks to them for letting me use it in these packs :)

If you find anything broken, please open an issue :)



____________________________________________________________________________________________________________________________________________________________
`Merging my packs (Textures):`


These 3 packs have been done in a way so you could merge them easily. All the variated textures are labeled to not conflict between packs, you should just have to merge  all the .properties files and make sure they are in the top pack in your game list

#
<ins>Villagers textures (assets\minecraft\textures\entity\villager):</ins>
> skins.1 is the vanilla villager
> 
> skins.2 to skins.499 are Song Of Wars skins
> 
> skins.500 to skins.506 are Guard Villagers skins
> 
> skins.510 to skins.519 are Alex and Steve skins
> 
> skin.600 to skins.1999 are Hermitcraft skins (Each hermit has 50 reserved slots, so 600-649, 650-799...)

Each pack you'll have texture randomly or you can rename an entity to get a specific one. Except for Alex & Steve, all textures have the same chance to be spawned

At the end of the .property file: #entityRenderLayerOverride=transclucent_cull.
This is a property unique to ETF. This mean 2nd layer of texture will render transparent according to their .png file. Without it it will render a solid color.
For example in the hermitcraft pack "Suit Scar" is meant to have a transparent helmet. Also fun fact, vanilla librairian glasses are meant to be transparent too, but they render solid.
But for the moment there is [this issue](https://github.com/Traben-0/Entity_Texture_Features/issues/254). You can remove the # to make it work, but any renamed villager you'll look at will crash your game.


#
<ins>Guard Villagers textures (assets\guardvillagers\textures\entity\guard):</ins>

Guard villagers texture follow the same principle as villagers
Only exepction is that Songs of War pack have specific naturally spwan condition regarding the biome
They havd textures labeled guard_0, guard_1..., the number refering to the biome they spawn in
>0 is plains and have Ardoni skins (Will also be used for other biomes villageless)
>
>1 is deserts and have Karthen & Northwind skins
>
>2 is savanna and have Hydraphel & General skins
>
>3 is swamps and have Conchord skins
>
>4 is jungle and have Cydonia & Etherea skins
>
>5 is taiga and have Felden skins
>
>6 is snow plains and have Crown Peak skins

#
<ins>Straw Statues textures (assets\strawstatues\optifine\random\entity):</ins>

These textures must be the orignal skin (64*64) with no edit on the eyes. The texture suffix is the same as villagers
Rename a statue in the style tab to get the texture



Note that there are some zombies textures in the SOW. 
I recommand to use Fresh animation pack in complement of mine, but put it below my pack in the game list


____________________________________________________________________________________________________________________________________________________________
`Merging my packs (Sounds):`

Under assets\minecraft\esf\entity\villager you will find a liste of .properties and .json files
The .properties uses an unique ETF feature to match sound regarding the texture suffix. It then load a corresponding .json file, wich is written like the vanilla sound.json
The suffix of the .json generally matches the one of the textures. In most of Hermitcraft case, it will match the first one of the 50 allocated.
Sounds are stored in assets\minecraft\sounds\custom\name_of_the_pack
Again, just merge the .propertie file and make sure it is in the top level pack in the game list

Guard villagers have their .properties in assets\guardvillagers\esf\entity\guard but the .json uses the same audio files as the villagers

You will also need to merge the sound.json in assets\minecraft
This one loads musics in game and menu


____________________________________________________________________________________________________________________________________________________________
`Merging my packs (Models):`

Only the guard villagers .propertie files (assets\minecraft\emf\cem) should be merged
Uses the comment on the file to copy and paste what you need.

Note: Forge and Fabric version of the mod don't have the same name for the model
Also, these models might be updated in a near future with some new EMF feature to make things easier


____________________________________________________________________________________________________________________________________________________________
`Capes:`
You can set capes in the texture files. There is 4 slots available. They will randomly appear when the villager/guard spawn.
Capeless mobs are more likely to spawn, then the slot #1 have a higher chance than #2, #3 & #4

____________________________________________________________________________________________________________________________________________________________
`Items and names:`

There are  item that change texture when renamed.
  -You will have weapons from Song Of War. For the most part swords, I did them in every vanilla material. (this is supported by either Chime or CIT)
  -You also will find the custom items used by the hermits in season 8 & 9 (this is supported ONLY by Chime at the moment!!) 
  -Some weapon will be displayed regarding the name of the mob wich hold them. This is a Chime feature and currently doesn't work with CIT.
          -> So if you're using only CIT you'll have to first rename the item, then give it to the mob. (Forge doesn't have a chime port afaik)
      
You can get any texture by renaming a villager or a guard. The full list of possible names can be found in the main branch. You can also check the "Names and custom weapon list" file inside the ressource pack. Guard villagers have their textures in the guard villagers asset subfolder, not the minecraft on.

____________________________________________________________________________________________________________________________________________________________

`Optional Mods:`

[Villager Names](https://modrinth.com/mod/villager-names-serilum) This mod from Serilum gives villagers (and modded one) random names. You can also provide you custom list. There a file in each pack with them names of the pack. You automatically get matching textures. This when used with chime gives automatically adequate weaapons to guard villagers :) 

Place the custom names.txt in .minecraft/config/villagernames/

Note: If only the custom list is activated, it means it ignore texture distribution of the .properties files. 


[Omega Mute](https://modrinth.com/mod/omega-mute) Also by Serilum, this mod let you cull entity sounds. With villager saying proper words
Either use the ingame command: `/omegamute cull 1 entity.villager.ambient`
Or edit in the config file to: `1-minecraft:entity.villager.ambient`
The number 1 represent the second without the game producing a villager sound. You can go higher, but from my testing it works pretty good with just 1


____________________________________________________________________________________________________________________________________________________________
`Customize/add your own skins:`

My pack [villagers to player](https://modrinth.com/resourcepack/villagers-to-player) provide a detailed guide on how to get your own skin on my models.
You'll also find the .pdf in the files on this page.

I recommand you to add your texture using a suffix higher than 2000 as it is the last of the hermitcraft pack. (assuming no new hermit...)


____________________________________________________________________________________________________________________________________________________________
`Future ideas`

I have a bunch of ideas to come at some point. No ETA, no promises. But to name a few:

Implement a second layer on most of SOW background caracters. In the files only the main one have detailled textures. This will take a long time tho :p 

A few differents sleeping villagers models. This one might be added soon, but I need to do a bunch of testing to see if my idea is possible.
