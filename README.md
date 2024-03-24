Description not up to date!
The 3 ressource packs are not up to fate with Villagers to Players yet neither!
Coming soon!









# Villager Steve Model

This page regroup instruction for my 3 ressources packs available on [planeteminecraft](https://www.planetminecraft.com/member/seb_semos/)


` I'll start with credits!`

[Song of war villagers](https://www.planetminecraft.com/texture-pack/song-of-war-villagers/) has been made following the animation of the same name on youtube. Back then a ressource packs with all the skins and texture had been released to the public. With the rebranding of the animation studio, it is (to my knowledge) no longer available. 

[Alex and Steve villagers](https://www.planetminecraft.com/texture-pack/alex-and-steve-villagers/) also took inspiration from the animated story of the same studio. Although I did worked with vanilla Alex and Steve textures, this is why you have possibility to get the "Derp" skin in this pack.

[Hermitcraft villagers](https://www.planetminecraft.com/texture-pack/hermitcraft-villagers/) is using skins of famous youtubers currently playing on this smp. The skins I used have been taken via [NameMC](https://fr.namemc.com/) You can get the history of skin used by a player on this website.
Some custom items have been made by Stridey. He gave me authorization to use them. I don't know who made the rest. If you are the creator and don't want it to be shared in this pack, let me know :)

If you came accross these pack I assume you most likely know where they come from. If not, feel free to check out [Squared Media](https://www.youtube.com/@SquaredMediaAnimations) for the animations and [Hermitcraft](https://hermitcraft.com/) for the SMP.

Now for the mod needed to these pack to work you'll need
- [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures)
- [Entity Model Features](https://modrinth.com/mod/entity-model-features)
- [Chime](https://www.curseforge.com/minecraft/mc-mods/chime-fabric) is prefered to CIT Resnew to get custom items
- [Cit Resnew](https://modrinth.com/mod/cit-resewn)
- [Cit Resnew, Forge](https://www.curseforge.com/minecraft/mc-mods/forge-cit)


The Villager model has been worked from a port of [Fresh Animation](https://www.curseforge.com/minecraft/texture-packs/fresh-animations) By [Young SoulluoS](https://github.com/YoungSoulluoS/Fresh-Animations_cem_Fork) to make it compatible at the time with CEM fabric. Note: You now can directly use FA in fabric and forge thanks to EMF

The Guard Villager model is a modified vindicator from Fresh Animation by Fresh Lx

All the base work has been made by them. I just changed the model and altered a few line of code here and there. Big thanks to them for letting me use it in these packs :)

I'm a fabric user, I have now set a forge version of my packs. Chime stuff need to be deleted, and guard villagers models don't have the same name. I don't play with it, so less likely to find weird stuff in these packs.
Download them from my github
If you find any broken texture, please use EMF/ETF debug feature to tell me the number.

Might also work with optifine has these mods aim to give a fabric/forge equivalent. If it's not, nothing will be done for that matter.


____________________________________________________________________________________________________________________________________________________________
`Merging my packs:`

These 3 packs have been done in a way so you could merge them easily. All the variated textures are labeled so you can copy them all in one folder, and edit the villager.properties file (assets\minecraft\optifine\random\entity\villager)

> skins.1 to skins.7 are the vanilla textures of villagers.
> 
> skins.8 is empty so you can put your own skin
> 
> skins.9 to skins.231 are Hermitcraft skins
> 
> skins.231 to skins.499 are meant to be future hermitcraft skins
> 
> skins.500 to skins.985 are for Song Of Wars skins
> 
> skin.996 to skins.999 are Alex and Steve skins

Note that skins.1 to 7 are in all packs, but distribution of them is not the same in Alex and Steve pack. They are meant to spawn way more in this one, as other two packs give an equal chance to any skin.

Distribution is found in the biome list at the end of the file. 
If you add more than one skin of your own, I recommand to do so after skins.999, but then you will need to raise the numbers for the biome distribution.

At the end of the .property file: #entityRenderLayerOverride=transclucent_cull.
This is a property unique to ETF. This mean 2nd layer of texture will render transparent according to their .png file. Without it it will render a solid color.
For example in the hermitcraft pack "Suit Scar" is meant to have a transparent helmet. Also fun fact, vanilla librairian glasses are meant to be transparent too, but they render solid.
But for the moment there is [this issue](https://github.com/Traben-0/Entity_Texture_Features/issues/194). I prioritize emissive over this feature. But if you are not using Iris, remove the # to make it work

Note that there are some zombies textures in the SOW. 
I recommand to use Fresh animation pack in complement of mine.

Guard Villagers textures should also be mergable. I might have overlooked a few of them, but due to the mess it became because it get 7 categories it will be as it... :p 

____________________________________________________________________________________________________________________________________________________________
`Capes:`
Since version 6.0, models have capes. This is intended to be used in the Hermitcraft pack. I put capes to hermits regarding to the results in Name MC.
There is 4 spaces for capes. One model don't have the cape, it has a slightly lower chance to be selected. The models that display CAPE#1 has a bit higher chance than the 3 other.
CAPE#1 is wich one I usually see the hermit with.
Cape display are completly random. If you want specific cape or none, you'll have to edit the villager.properties
Guard Villagers also have a cape, but it is garantee, and only CAPE#1. There are currently no texture with capes for them in any pack

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

[Friend and Foes](https://www.curseforge.com/minecraft/mc-mods/friends-and-foes) Beekeeper job is supported

[Straw Statue](https://www.curseforge.com/minecraft/mc-mods/straw-statues) 

Renaming a straw statue via the tab Style will give it the corresponding texture. Name list is the same as villagers
Having a player name in the Model Parts tab as the priority to display the "live" texture
Don't forget to set the correct size for amrs if you want to display a slim skin.
To add you own skin you don't need to modify anything of the texture unlike villagers or guards, but texture #8 is not free. If you put something on texture #1 it will display anytime you place the statue (see below)
Currently emessive textures act weridly if you're using Iris. Hopefully will be fixed. Seems fine otherwise

[Guard Villagers](https://www.curseforge.com/minecraft/mc-mods/guard-villagers-fabric) From pack 6.0 use the regular model of guard villagers, as the steve one messes the player armor. 

EMF Must be at least: 1.0 to work. From this version I can change the model to suit the villagers and Fresh Animations.

Guard Villager has originaly texture 6 files corresponding to each vanilla biome than can get villages.
guard_0, guard_1... guard_6

For Song Of War pack:
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
>5 is taiga and have Crown Peak skins
>
>6 is snow plains and have Felden skins

For other packs: Will display the type of villager of the biome + occasionaly a bunch of hermits with "war" skins or Alex, Steve or Derp for their respective pack

Guard Villagers have several models that will change the way they hold weapon, as well as attack animation.
This is primarily intended for SOW pack. They will change depending of the weapon, the name of the weapon or the name of the mob. (Using CIT only might lead to some animation not matching the weapon)
Some weapon as swords have a model when a guard hold two of them. Even tho the animation will make the both of them move, it will not double the damage...
Guard also can spawn as left handed, and have corresponding models. BUT this is not controllable by the player. The guard inventory is the same for left and right handed. (A shift click will send a weapon in the shield slot btw. Take car of that as it could not look good)
Guard Villagers models also have a cape. It only got the CAPE#1, and will always display if on the texture. I choose not to add them to the Hermitcraft pack for now

See next point for textures customisation, but the model for Guard Villagers support the same options as the villager one, except the "biome/profession outfit"
You should keep this place of the .png file transparent. 
There might be a few querks I didn't figured out.
One about armor. When a second layer is used on the helmet of "meterial_layer_1.png" , it appear like it is on another head doing completely different stuff. Also second layers of helmets on "meterial_layer_2.png" seems to not render. The rest of the armor seems to be ok. I'll update a fix if I can find out what's going on.

Note that the textures for Guard Villagers need to be in:
assets\guardvillagers\optifine\random\entity\guard
but the model is in:
assets\minecraft\optifine\cem
Also note you need a dot for the random system suffix : guard_0.x, guard_1.x...

Also note Forge guard villagers don't have the same name file than fabric ones

[Villager Names](https://modrinth.com/mod/villager-names-serilum) This mod from Serilum gives villagers (and modded one) random names. You can also provide you custom list. There a file in each pack with them names of the pack. You automatically get matching textures. This when used with chime gives automatically adequate weaapons to guard villagers :) 
Place the custom names.txt in .minecraft/config/villagernames/

Note: If only the custom list is activated, it means it ignore texture distribution of the .properties files. 

____________________________________________________________________________________________________________________________________________________________
`Customize/add your own skins:`

In order to get the Fresh Animation vibe I wanted, I decided to go for a more complex model that gives me options. Biggest problem was to be able to use Alex type AND Steve type skins. (Their arms are not the same size) I wanted to keep 2nd layers of skins, and to have facial animations. Squeeze all that in a 64x64 regular skin.png was impossible. So I decided to work with a 128x128. 

To use you own skin, simply open it with a image editor (I use paint.net) make so the work area is going up to 128x128 make sure everything is transparent. Your skin must be on the top left quarter corner. If you have an Axel type skin. Move the arms (and 2nd layer arms) 64 pixels to the right

The bottom left quarter corner is use for villager jobs, bottom right quarter is for capes

There is a skin template file in each pack. Use it on a layer in your editing software for easy edit. The skin template legend will tell you what is what

Villager outfit, jobs, level and mob textures need to be resized a bit at places from their vanilla files, other parts of the skin respect vanilla player skin sizes.
Villager biome outfit are now transparent textures and are directly randomized from the random folder. (If you add some, it would be displayed on top of the skin)
This sadly broke a direct compability with other villagers ressources pack.

![Image](https://user-images.githubusercontent.com/89230340/259273846-cd3e87ba-0ca1-4b63-843a-4a6898d3b3fd.png)
![Skin Template Legend](https://github.com/SebSemos/villager_steve_model/assets/89230340/368c7e2e-d304-4db3-a87c-540f1bcba2d2)


Face animations:
Optional, but if you add eyes animations, ou don't want these texture on the main face or it will display them twice
The Eyelid will display "closed eyes". It is used for blinking and during sleeping. Other textures of the eyes are invisible during these two events
The noze part will display the vanilla villager noze. So you can have it on any character
I have set it up so any face can be supported, but the more in the middle the eyes are, the more the result is good. A derp face can go a bit wacky from time to time :p 

The "realistic" part will display thinner mouth and brows. It does not support all kind of faces. See the next photo to get an idea how it looks.
I've use it for Ardonis and some "mouthless" skins in SOW pack so they have a mouth kinda like in the animation

![Image](https://user-images.githubusercontent.com/89230340/259906726-cf46b5fb-110f-4b3c-8e42-69721a23d36f.png)
![Image](https://user-images.githubusercontent.com/89230340/259907284-deb0950d-0a4b-466a-bd7a-0dfad4f5f6be.png)

NOTE: Since 1.20, a sleeping villager get another model. I set it up so the animated eyes dissapears. But it mean you have to define a sleep texture or it will look weird.
It also remove the jobs outfit. And vanilla skined one will loose their biome coat. It now look like they are in pijamas :p 
NOTE #2: Since pack 6.0, job outfits will only render during work time

____________________________________________________________________________________________________________________________________________________________
`Forge vs Fabric`
What's the diffrence:
  - Guard Villagers don't have the same filename.
  - Because Chime is not on forge, item got missing texture is you keep the chime overides in the \assets\minecraft\models folder


____________________________________________________________________________________________________________________________________________________________
`Future ideas`

I have a bunch of ideas to come at some point. No ETA, no promises. But to name a few:

Sounds, especially for Hermitcraft pack. I might implement classic "catch phrases" for the villagers. But to do so, I'll have to first get in contact with them to get some recording. (I will not rip audio from videos!)

Implement a second layer on most of SOW background caracters. In the files only the main one have detailled textures. This will take a long time tho :p 

A few differents sleeping villagers models. This one might be added soon, but I need to do a bunch of testing to see if my idea is possible.
