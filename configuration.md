# Configuration Sections
The config is a VAST land of values and flags, and should be treated carefully as you make changes to those values within. Below you will find a comprehensive list of key / value pairs that are muteable, but anything else should be left alone. Period. There are also custom configs that we will address below so you can truly customize your SMP server!
####
> NOTE:  
> We use **ColorCodes**, BUT, we translate them with the `&` symbol! If you change any text values with ColorCodes, be sure to denote the color with the orrect symbol!
####

## Default Config  
`config.yml`  
| Key                 | Value                       | Description                                                                                                   |
|:-------------------:|:---------------------------:|:-------------------------------------------------------------------------------------------------------------:|
| prefix                  | "&f[&4Cake&5SMP&f] >> "     | The **ColorCoded** message that is prepended to any message displaying from the CakeSMP plugin.           |
| welcome-ttl             | "&5Welcome, {PLAYER}!"      | Default Welcome Title message displayed to **NEW PLAYERS**                                                |
| welcome-back-ttl        | "&4Welcome Back, {PLAYER}!" | Default Welcome Title message displayed to **RETURNING PLAYERS**                                          |
| max-player-markers      | 7                           | Default amount of Fat Travel locations a player is **ALLOWED** to have. Defaults to 7                     |
| claim-buyout-amount     | 850                         | The amount a player will receive when they sell their claim back to the server                            |
| ranks                   | List of Values              | These are the default names for Ranks CakeSMP uses. These can be changed to whatever values you want      |
| shop-name               | "CakeSMP"                   | The default shop title that will write itself to the GUI of the server shop.                              |
| use-cerberus-claims     | false                       | Whether **CakeSMP** will use the Land Claims system or not. LEAVE TO FALSE!                               |
| cerberus-house-max      | 3                           | The amount of doors / homes a player is allowed to claim                                                  |
| use-minedash-delivery   | true                        | Whether MineDash uses a delivery wait-timer before items are given to player                              |
| minedash-delivery-timer | 3000                        | The amount of time in SECONDS the player needs to wait for their food delivery. Defaults to 3000 seconds  |

####  
####  

## MineDash Menu Config  -- _(NEW FEATURE)_
`minedash.yml`  

Although you *CAN* change the products, we recommend leaving them as-is and adding your own, custom products to the config! With that being said, F4ngdev takes NO responsibility for broken plugins and messed up configs. The way products are handled is a unique way of doing things that streamlines the process and allows for simple easy use within your server.

Example of Products:
```yml
minedash-menu:
  filetmignon: # (Product Name) Name of the item ALL LOWERCASE & One Word SIMILAR to what you are naming it
    name: "Filet Mignon" # Display Name for the item
    material: 'COOKED_BEEF' # Minecraft generated Material type
    price: 5000 # Price of the item(s)
    amount: 3 # Amount to be sold at one time
```
Each product will go UNDER the `minedash-menu` indicator, and will be labeled and formatted as shown above. The `(Product Name)` needs to be a SIMILAR name of the Display Name and needs to be spelled as shown above. Below that, you set the matching Material type *( Example is Filet Mignon so Material = COOKED_BEEF )* that is generated from the Minecraft side of the game. Following that is your `price` you want the item sold at, and then the `amount` of items to be sold at once *( think of it as like a package deal if its more than 1 )

####
####  

## Products Config  
`products.yml`  

Although you *CAN* change the products, we recommend leaving them as is, and adding you own products to the config. With that being said, F4ngdev takes NO responsibility for broken plugins and messed up configs. The way products are handled is a unique way of doing things that streamlines the process and allows for simple easy use within your server.

Example of Products:
```yml
product-listings:
  phantommembrane: # (Product Name) Name of the item ALL LOWERCASE & One Word
    material: 'PHANTOM_MEMBRANE' # Minecraft generated Material type
    price: 5000 # Price of the item(s)
    amount: 3 # Amount to be sold at one time
```
Each product will go UNDER the `product-listings` indicator, and will be labeled and formatted as shown above. The `(Product Name)` needs to be the EXACT name of the Minecraft item and needs to be spelled as shown above. Below that, you set the matching Material type *( Example is Phantom Membrane so Material = PHANTOM_MEMBRANE )* that is generated from the Minecraft side of the game. Following that is your `price` you want the item sold at, and then the `amount` of items to be sold at once *( think of it as like a package deal if its more than 1 )

####
####  

## Starter Configuration
`starter.yml`

The Starter file is where you can define all of the items and stats your players will begin with! The layout is simple and easy to implement, should the instructions be followed as below:

*Example of Starter:*

```yml
loadout:
  bank: '350' # Starting dollar value of each new player
  helmet: 'LEATHER_HELMET' # Material of matching item
  chestplate: 'LEATHER_CHESTPLATE'
  leggings: 'LEATHER_LEGGINGS'
  boots: 'LEATHER_BOOTS'
  weapon: 'WOODEN_SWORD'
  food: 'BREAD' # Food type, if any, the new player will recieve
  food-amount: 20 # Quantity of the food type
```

####

Each starter item *( aside from the `bank` and the `food-amount` )* refers to the **MATERIAL** of the item you are giving to the players. If you want your players to start off untouchable, then you would set each loadout piece to `DIAMOND_HELMET` and so on. The `food-amount` MUST be a positive integer!  

####
####

## JobCorps Configuration  
`jobcorps.yml`  
The **JobCorps** configuration is where you can handle all things job related within your SMP server. **DO NOT CHANGE / ADD TO THESE VALUES!** Should you want to have a new job added to the plugin, please contact us via the Discord and we will roll-out an update with the new jobs.

With that being said, you ***CAN*** change the `hourly` and `basepay (amount)` for each of the jobs! Just make sure that they are balanced and POSITIVE INTEGERS!

####

> NOTE:  
> *The `nomad-payout-distance` refers to the amount of steps a player must take before receiving any XP of money for having the job of `Nomad`*

####
####  

## Helplist Configuration  
`helplist.yml`

The Helplist Configuration refers to the help messages the player will receive when using the `/cake` command and looking for assistance with the **CakeSMP** plugin.
###
**DO NOT CHANGE THESE VALUES!**
