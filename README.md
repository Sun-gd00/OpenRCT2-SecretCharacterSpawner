# OpenRCT2-SecretCharacterSpawner
OpenRCT2 Plugin, Adds a percent chance of encountering Easteregg Characters without the need to manually rename them.

<img width="914" height="571" alt="Forest Frontiers 2026-06-21 09-40-24" src="https://github.com/user-attachments/assets/1bc81f8d-7075-4f57-bc8d-87c4af897d11" />

I wanted to encounter these Characters "On the Wild", so i made a Plugin for it!

Secret Character List:

			//RCT1
            "Chris Sawyer",			//Photographs, Drives Fast 	-- Programmer
            "Simon Foster",			//Paints					-- Art Designer
			"David Ellis",			//"And here we are on..."	-- Sound Designer
			
			"Emma Garrell",			//Gifts Purple Clothes
			"Felicity Anderson",	//Causes Vomit on Others
			"John Wardley",			//"Wow"
            "Katie Brayshaw",		//Frequently Waves
			"Katie Smith",			//Frequently Jumps
			"Lisa Stirling",		//Litters
			"Nancy Stillwagon",		//Gifts Ice Cream
			
			//RCT2
			"Carol Young",			//Decreasing Happiness
			"Corina Massoura",		//"It's too crowded here."
			"Donald MacRae",		//"Im lost!"
			"Frances McGowan",		//Frequently uses Bathroom
			"Katherine McGowan",	//Frequently Eats
			"Mia Sheridan",			//Increasing Nausea
			"Melanie Warn",			//Happy+Energy, no Nausea
			"Joanne Barton",		//Gifts Pizza
			"John Mace",			//Pays Double for Rides
			"Eilidh Bell",			//Vandalizes
			"Katie Rodger",			//Wants to Leave
			
			//Karting
            "Mr. Bean",				//Drives Slow
			"Jacques Villeneuve",	//Drives Faster
			"Michael Schumacher",	//Drives Even Faster
            "Damon Hill"			//Drives Fastest

Base chance for spawn is 0.5%, this means 1 every 200 guests is a Easter Egg Character.

Change secretChance = x to edit percent chance to x.

Grab EITHER SecretCharacterSpawner OR SecretCharacterSpawner(LOWCHANCE), NOT BOTH.

----------

What does it do?

This Plugin first parses through the current guests in the Park, and marks them so they are not changed into a Secret Character.

After this, every new guests will have a percent chance of getting it's name changed into one from the list.

When the name is changed, the behavior of the guest will change, according to how Easteregg Characters work.

There should not be any repetition on names already used, so no "2 Mr. Beans".

----------

How to edit the Plugin?

There are two important ways in which the Plugin can be edited.

1. Percent Chance:
By modifying secretChance you can change the chance of encounter, if secretChance=100, then Secret Characters will appear as soon as possible, which can be fun but also very disruptive.

2. Name List:
This mod works by editing the name of a Character, so if you want to add your own EasterEgg Characters (with no special behavior, just name) you can expand the list by following the format and said name will enter the pool.

	...
   
	"Damon Hill",			//Drives Fastest

	"Amogus Sanchez",		//Doesn't change behavior

	"Uzumaki Goku"			//You may add whatever name you like

	];

Be sure to add a coma after the name, which has to be in quotations.

That's it, happy encounters!
