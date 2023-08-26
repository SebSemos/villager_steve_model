# Villager Steve Model

This page regroup instruction for my 3 ressources packs available on [planeteminecraft](https://www.planetminecraft.com/member/seb_semos/)


` I'll start with credits!`

[Song of war villagers](https://www.planetminecraft.com/texture-pack/song-of-war-villagers/) has been made following the animation of the same name on youtube. Back then a ressource packs with all the skins and texture had been released to the public. With the rebranding of the animation studio, it is (to my knowledge) no longer available. 

[Alex and Steve villagers](https://www.planetminecraft.com/texture-pack/alex-and-steve-villagers/) also took inspiration from the animated story of the same studio. Although I did worked with vanilla Alex and Steve textures, this is why you have possibility to get the "Derp" skin in this pack.

[Hermitcraft villagers](https://www.planetminecraft.com/texture-pack/hermitcraft-villagers/) is using skins of famous youtubers currently playing on this smp. The skins I used have been taken via [NameMC](https://fr.namemc.com/) You can get the history of skin used by a player on this website.

If you came accross these pack I assume you most likely know where they come from. If not, feel free to check out [Squared Media](https://www.youtube.com/@SquaredMediaAnimations) for the animations and [Hermitcraft](https://hermitcraft.com/) for the SMP.

Now for the mod needed to these pack to work you'll need
- [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures)
- [Entity Model Features](https://modrinth.com/mod/entity-model-features)
- [Cit Resnew](https://modrinth.com/mod/cit-resewn)

Pre 1.20 used [Chime](https://www.curseforge.com/minecraft/mc-mods/chime-fabric) to get custom items, but it is not updated to 1.20 yet, and is not focused in priority by his owner. Files are still in the ressource pack, and should so work if an update is publish

The model has been worked from a port of [Fresh Animation](https://www.curseforge.com/minecraft/texture-packs/fresh-animations) By [Young SoulluoS](https://github.com/YoungSoulluoS/Fresh-Animations_cem_Fork) to make it compatible at the time with CEM fabric. Note: You now can directly use FA in fabric and supposedly forge thanks to EMF

Feel free to use my villager model in your own pack. If you publish it, please give a link here and credit Fresh Animation and Young SoulluoS.
All the base work has been made by them. I just changed the model and altered a few line of code here and there

I'm a fabric user, I don't know if my pack work with forge mods, but it should.
Might also work with optifine has these mods aim to give a fabric/forge equivalent. If it's not, nothing will be done for that matter.


____________________________________________________________________________________________________________________________________________________________
`Merging my packs:`

These 3 packs have been done in a way so you could merge them easily. All the variated textures are labeled so you can copy them all in one folder, and edit the villager.properties file (assets\minecraft\optifine\random\entity\villager)

> skins.1 to skins.7 are the vanilla textures of villagers.
> skins.8 is empty so you can put your own skin
> skins.9 to skins.231 are Hermitcraft skins
> skins.231 to skins.499 are meant to be future hermitcraft skins
> skins.500 to skins.985 are for Song Of Wars skins
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

____________________________________________________________________________________________________________________________________________________________
`Items:`

There are a few item such as swords that change texture when renamed. Most of them are in the SOW pack. First made to be used with Chime mod, they were then rewrite to work with CITresnew
Some weapon were displayed regarding the name of the mob wich hold them. This is a Chie feature and currently doesn't work with CIT. Mod owner said it was a upcoming feature. I will make it work again when so. 
For now you'll have to first rename the item, then give it to the mob.
This is a great feature with the guard villager mod. 

____________________________________________________________________________________________________________________________________________________________

`Optional Mods:`

[Friend and Foes](https://www.curseforge.com/minecraft/mc-mods/friends-and-foes) Beekeeper is supported
[Guard Villagers](https://www.curseforge.com/minecraft/mc-mods/guard-villagers-fabric) Use the Steve model in the mod option. A bunch of skins of the pack will be used for Guard regarding to the biome they're in


____________________________________________________________________________________________________________________________________________________________
`Customize/add your own skins:`

In order to get the Fresh Animation vibe I wanted, I decided to go for a more complex model that gives me options. Biggest problem was to be able to use Alex type AND Steve type skins. (Their arms are not the same size) I wanted to keep 2nd layers of skins, and to have facial animations. Squeeze all that in a 64x64 regular skin.png was impossible. So I decided to work with a 128x128. 

To use you own skin, simply open it with a image editor (I use paint.net) make so the work area is going up to 128x128 make sure everything is transparent. Your skin must be on the top left quarter corner. If you have an Axel type skin. Move the arms (and 2nd layer arms) on the top right quarter corner
The bottom left quarter corner is use for villager jobs, bottom right quarter is unuse
Use these picture as references. 
Do note that villager jobs hat need to be shrinked a little bit to look right. Same for villager faces. This sadly broke a direct compability to villagers ressources pack where you would only had to resize the .png file.

![Image](https://user-images.githubusercontent.com/89230340/259273846-cd3e87ba-0ca1-4b63-843a-4a6898d3b3fd.png)
![Image](https://user-images.githubusercontent.com/89230340/259273880-7776e36f-6d91-4262-976e-7374f78dabfc.png)

Face animations:
Use this template to know where to put texture of eyes and mouth for it to be animated.
You don't want these texture on the main face or it will display them twice
The sleep part will display "closed eyes" when villagers are in a bed. It must be added when using eyes animation because it set so eyes will disapear during sleep.
The noze part will display the vanilla villager noze. So you can have it on your own skin :D 
I have set it up so any face can be supported.

The "realistic" part will display thinner mouth and brows. It does not support all kind of faces. See the next photo to get an idea how it looks.
I've use it for Ardonis and some "mouthless" skins in SOW pack so they have a mouth kinda like in the animation

![Image](https://user-images.githubusercontent.com/89230340/259906090-8de7e722-d940-49b7-b127-8e9260fc4464.png)
![Image](https://user-images.githubusercontent.com/89230340/259906726-cf46b5fb-110f-4b3c-8e42-69721a23d36f.png)
![Image](https://user-images.githubusercontent.com/89230340/259907284-deb0950d-0a4b-466a-bd7a-0dfad4f5f6be.png)

NOTE: Since 1.20, a sleeping villager get another model. I set it up so the animated eyes dissapears. But it mean you have to define a sleep texture or it will look weird.
It also remove the jobs outfit. And vanilla skined one will loose their biome coat. It now look like they are in pijamas :p 

____________________________________________________________________________________________________________________________________________________________
Future ideas

I have a bunch of ideas to come at some point. No ETA, no promises. But to name a few:

Sounds, especially for Hermitcraft pack. I might implement classic "catch phrases" for the villagers. But to do so, I'll have to first get in contact with them to get some recording. (I will not rip audio from videos!)

Implement a second layer on most of SOW background caracters. In the files only the main one have detailled textures. This will take a long time tho :p 

A few differents sleeping villagers models. This one might be added soon, but I need to do a bunch of testing to see if my idea is possible.

More custom items for the hermitcaft pack. I think about all the one the get by renaming stuff. This will likely be added after they release season 9 map.
I might check previous season in between, for like derpcoins and such.

Animated guard villagers the same way villagers are. I am doing some test for that matter. Not sure if I will get it work tho.
