# Elixir Pets
Available here:

# Info
We have created a script that allows you to buy, own, and take care of animals / pets! In addition to being fully configurable, it is also very easy to use.
The configured slash command can be used to manage your pet, and you will find many options there. There is also a pet store built into the script that allows you to purchase pets, food, and other items. This Script Also contains a Pet Clinic if your pets get sick you can get them treated.

# Features
1. QBCore supported.
2. Custom QBCore rename supported in config.
3. Fully configurable.
4. Open-Source.
5. Pet can get ill too and you'll have to take them at pet clinic to get them cured.
6. Pet has a food and health system so they can die

# How to install
### Rename Core
* Go to ``shared.lua`` and search for this:
```
Config.Corename = 'qb-core'
```

### Choose target, input and menu
* Go to ``shared.lua`` and search for this:
```
Config.Target = 'qb-target' -- qb-target/bt-target Whatever You use
Config.Menu = 'qb-menu'
Config.Input = 'qb-input'
```

### Configuration
* Go the ``shared.lua`` file
* Configure Searchable Items by Police K9
```
Config.SearchableItems = {

['IllegalItems'] = {

	['weed'] = 10,
	['coke'] = 1,
	['bread'] = 1,
	['water'] = 1,
},
}
```
* Configure K9 Message (For Police):
```
Config.K9Message = 'The K9 has been alerted to something!' -- If the Police dog finds something
```
* Configure Tennis Ball Price:
```
Config.TennisBallPrice = 200
```
* Configure Illness Chance For Pet:
```
Config.IllnessChance = 5 -- Chance to get Sick (For Pets) - If Police, has two chances to get sick
```
* Configure Heal Price for Pet:
```
Config.HealPrice = 500
```
* Configure Food Price and Item Name For Pet:
```
Config.FoodPrice = 250
Config.FoodItem = 'petfood' -- Database name of item
```
* Configure Tennis Ball Price:
```
Config.TennisBallPrice = 100
```
* Changing pets in store
* You can add pets to Store like this:
```
Config.PetNumber = 'a_c_pig' --https://wiki.altv.mp/wiki/GTA:Ped_Models
Config.PetNumberPrice = 1000
Config.PetNumberLabel = 'Pig'
```

### Items
* Add the Following to your items list in your core/base:
```
	["petfood"] 					 = {["name"] = "petfood", 				["label"] = "Pet Food", 	     	   						 ["created"] = nil, 		["decay"] = 14.0,		["weight"] = 150, 		["type"] = "item", 		["image"] = "petfood.png", 				["unique"] = false,   	["useable"] = true,    ["shouldClose"] = false,    ["combinable"] = nil,   ["description"] = "Feed your pet ma boy.."},	
	["tennisball"] 			 			 = {["name"] = "tennisball", 			["label"] = "Tennis Ball", 				["created"] = nil, 		["decay"] = 14.0, 			["weight"] = 550, 		["type"] = "item", 		["image"] = "tennisball.png", 	["unique"] = false, 					["useable"] = true, 	["shouldClose"] = true,	   ["combinable"] = nil,   ["description"] = "Tennis ball Play Cricket"},
```
* Add these items to your qb-inventory > html > images, images found in images folder

![Tennis Ball](https://cdn.discordapp.com/attachments/627417439566561290/1064592747522183198/tennisball.png) 
![PetFood](https://cdn.discordapp.com/attachments/627417439566561290/1064592747790610522/petfood.png)

### Database
* Insert the pets.sql file in your database
* ⚠️ DO NOT CHANGE ANYTHING IN SQL FILE OR IT WON'T WORK ⚠️

### Pet Store Map (Not Owner of this map)
* [Pet Store MLO](https://nl.gta5-mods.com/maps/mlo-pet-shop)

### Support
For issues join our [Discord](https://discord.gg/JMTPdBV), and we will help you asap!
