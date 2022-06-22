# Plugin Interactive Feature List  
As stated above, the features of **CakeSMP** allow you to have a standalone SMP plugin with minimal needs to other plugins to round out the whole experience for you and your friends. Below you will find a detailed list of all the features and how to use them within the plugin for seamless integration.  

## NEW FEATURE:  
You can now **_smelt Diamond, Iron, and Gold Armor / Weapons / Tools_** back into their individual ingot-based counterparts! Simply throw the item inot a **_Blast Furnace_** and it will smelt it back down into what made it. The amount of resources ( ingot / diamonds ) you receive is RANDOM and based off the amount it took to create them with a +-2 fluctuation.

**Example:**
- A Diamond Pick Axe will give you either 0 or 3 diamonds back
- An Iron Chestplate will give you either 6 or 8 iron ingots back  
####

####
## Bank
The **CakeSMP Bank** gives you an economy that is easily managed and wired throughout the ENTIRE plugin and changes dynamically so you have nothing to worry about with setup and use. Pay other players, watch your money grow from working, withdrawl/deposit actual paper money, sell items to the **Recycling Center** for income, sell claims... the list goes on.

```md
Withdrawl / Deposit is a W.I.P. and allows player to *withdrawl* a 
specific amount of money that is converted into `PAPER` with a specific 
title to denote the value. A *deposit* can also be made **WHILE HOLDING 
THE PAPER MONEY**, and will deposit the sum back into your account.
```

| Command | Args | Description |
| --- | --- | --- |
| /bank | ALL | Main initiator of the Bank plugin. This MUST come before every Bank associated argument. |
| --  | balance | Check your current Bank balance |
| --  | pay [player] [amount] | Pay the specified player a specific amount. *( **O.P** -- use this to pay yourself from the server! )* |
| --  | withdrawl [amount] | Withdrawl the specific amount into paper money |
| --  | deposit | Deposit the amount of the paper money in your hand BACK into your account |
| --  | exchange | Exchange **DIAMONDS / EMERALDS IN HAND** for money in your bank account |

####
## Cerberus
Cerberus is the **Land Claim & Security** feature of **CakeSMP** and allows players to enact privacy on **ONE LOCATION**! Players are ONLY allowed to have one land claim at a time... this isn't the 1%-ers...

> NOTE:
> _Land Claims is currently disabled! The Home Security feature is ACTIVE!_

Cerberus is used by equipping a **Wooden Hoe**, then right-clicking 2 blocks on opposite corners from eachother. These locations will be stored and that area will then belong to the player. Should the player want to move and find a new location, they will need to be standing in the **CURRENT** claim and use the `/sellclaim` command. They will recieve compensation, and the claim will no longer be tied to them, allowing them to move on to greater horizons.

**_NEW FEATURE:_**  
**Cerberus Home Security** is the newest feature to **CakeSMP** and it allows players to claim doors attached to structures _( normally a house )_ as their own and keep other players out! Players are allowed a **default of 3 homes to claim**, and an O.P. can give additional houses if the need arises.

The Player / O.P. need to be **_RIGHT IN FRONT OF THE DOOR AND LOOKING AT IT_** to use any of the commands below! The distance is registered at **1 block** so get all up in that door's business!

| Command | Args | Permissions | Description |
| ------- | ---- | ----------- | ----------- |
| /claimhome | N/A | Everyone | Allows a player to claim a door attached to a structure. Default 3 allowed per player |
| /abandonhome | N/A | Everyone | Allows a player to abandon a specific home |
| /setowner | [player] | O.P. | Allows O.P. to override max houses and give player another home |
| /removeowner | [player] | O.P. | Allows O.P. to remove a home from a player at any time |

####
## Magicka  
**Magicka** is a wicked fun little feature that was added after development had started, and it introduces the ability to use XP *( Minecraft XP )* as **Magicka** and cast certain spells that will either assist you, or catch you lacking!

| Command | Description |
| --- | --- |
| /shift | Phase-Shift between 5-7 steps forward, and at the highest block at that position. |
| /pool | Generate a pool in the direction the player is looking... think MLG jump |
| /combust | Create an explosion roughly 10-15 blocks in front of you. Good for Nether mining or blowing up groups of mobs |
| /leech | Trade Health for Magicka |
| /regen | Trade Magicka for Health |
| /float | Begin levitating for roughly 10 seconds. Good for getting out of holes, but make sure you have a ceiling |

####
## Fast Travel
Saving specific locations and traveling between them is a MUST have in any SMP server, and with the **CakeSMP Fast Travel** it has never been easier and more safe!

| Command | Args | Description |
| --- | --- | --- |
| /setmarker | [name] | Save the current location as a Map Marker with the given name to use when fast Traveling |
| /mapmarkers | N/A | View all of ther players saved Map Markers |
| /removemarker | [name] | Remove the specific Map Marker from the players Fast Travel list |
| /fasttravel | [name] | Fast Travel to the saved Map Marker location |

####
## Job Corps
Every player is going to need money to purchase items and build their own little empire with their friends and compadres.

The **Job Corps** has an Hourly Pay function built into it, as well as the custom ranking system so your players can grow and improve as they work and grind!

| Command | Args | Description |
| --- | --- | --- |
| /joblistings | N/A | View all of the currently available jobs on the server |
| /myjob | N/A | View the job the player is currently applied to |
| /applyto | [job] | Apply to the given job |
| /quitjob | [job] | Quit from the given job |

####
## Pockets
The feeling you get when you are spelunking and a Creeper sneaks up and vaporizes you and ALL of the items you were carrying are pretty much gone... that feeling no longer exists with Pockets! Using a simple command, you're players can access their Pockets, a ***27 slot inventory*** that saves everything you put into it... even when they die!

| Command | Args | Description |
| --- | --- | --- |
| /pockets | N/A | Allows player to open their Pockets for safe-keeping |

####
## Recycling Center
Recycling Center

We have all been in that place where we have WAAY too much in our inventory, and we can't pick the ore / item we originally needed in the first place. The **Recycling Center** now handles that problem for you by buying all of your extra items for a reduced price.

| Command | Args | Description |
| --- | --- | --- |
| /recyclingcenter | N/A | Sell the items ***IN MAIN HAND*** to the Recycling Center for money |

####
## RTPer
A MUCH needed asset in any SMP server is quick, efficient, safe ways to travel quickly about the MASSIVE world your players get to enjoy. The **RTPer** is exactly that tool! With a single command, your players can be randomly teleported ANYWHERE within the server world **CakeSMP** is running on! With safety checks to ensure a clean landing spot, your players can now go and grind when they need to, anywhere in the world.

| Command | Args | Description |
| --- | --- | --- |
| /rtp | N/A | Teleports a player to a random locaiton within the server world they are in |

####
## Rubbish
Lava Pit trashcans are a 1.12 thing... and the fact that its not something actually *IN* Minecraft at this point is beyond me. But hey, thats what plugins are for! **Rubbish** is a new, safe alternative Trashcan system that will ensure simple and efficient trash handling for your players.

**Rubbish** uses any sign / wall-sign that IS NOT Warped or Crimson and a specific setup of the text that goes on the sign. Please be sure to follow the directions below to get your Trashcans up and running smoothly!

#####

> NOTE:
> 
> *Due to issues with players taking enough rope to hang themselves with, the setting of Trashcans is only allowed by an O.P. This will keep your trashcan count to a minimum, and will maintain some aspect of realism so you don't find 15 trashcan signs out in the wilderness randomly*

#####

**Rubbish Setup:**

- Place a sign / wall-sign *( NOT Crimson / Warped )*
  
- On the **first line**, write the following: `[Set Rubbish]` and hit `Done`
  
- Right-Click to open the Rubbish bin and say bye-bye to the garbage!
  

####
## ServShop
The **ServShop** is a HUGE asset to have on the server, as it allows you to give players the ability to purchase items that are generally *REALLY* difficult to get, or are a pain to find, from a safe and secure location, and for the prices that you set and decide!

**ServShop** uses the `products.yml` configuration file ***( See Above Configuration Section )*** to set the items that are available to the player, and it is recommended that you take a ***careful*** glance at the file and how the products are setup as you may choose to add new products as you receive feedback!

| Command | Args | Description |
| --- | --- | --- |
| /shop | N/A | Open the server shop to view / purchase items that are stored in the `products.yml` configuration |

####
## SetSpawn (O.P. Only)
**SetSpawn** does exactly what you would think; sets the world spawn point to where you are standing when you give the command. Easy-Peasy.

| Command | Args | Description |
| --- | --- | --- |
| /setsmpspawn | N/A | Sets the world spawn point to the location the player is standing when the command is given |

####
## CakeKnife
This feature is your `/help` command for all things **CakeSMP** related. By using the command, and adding an optional number for pages, **CakeSMP** will display all of the commands and features available to your players in a colorful and legible fashion.

| Command | Args | Description |
| --- | --- | --- |
| /cake | [page no.] | View the Help pages on **CakeSMP** and get quick answers to questions regarding the commands and features |

####
