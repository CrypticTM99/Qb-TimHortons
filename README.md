# Qb-TimHortons


░█████╗░██████╗░██╗░░░██╗██████╗░████████╗██╗░█████╗░░██████╗
██╔══██╗██╔══██╗╚██╗░██╔╝██╔══██╗╚══██╔══╝██║██╔══██╗██╔════╝
██║░░╚═╝██████╔╝░╚████╔╝░██████╔╝░░░██║░░░██║██║░░╚═╝╚█████╗░
██║░░██╗██╔══██╗░░╚██╔╝░░██╔═══╝░░░░██║░░░██║██║░░██╗░╚═══██╗
╚█████╔╝██║░░██║░░░██║░░░██║░░░░░░░░██║░░░██║╚█████╔╝██████╔╝
░╚════╝░╚═╝░░╚═╝░░░╚═╝░░░╚═╝░░░░░░░░╚═╝░░░╚═╝░╚════╝░╚═════╝░

░██████╗░█████╗░██████╗░██╗██████╗░████████╗░██████╗
██╔════╝██╔══██╗██╔══██╗██║██╔══██╗╚══██╔══╝██╔════╝
╚█████╗░██║░░╚═╝██████╔╝██║██████╔╝░░░██║░░░╚█████╗░
░╚═══██╗██║░░██╗██╔══██╗██║██╔═══╝░░░░██║░░░░╚═══██╗
██████╔╝╚█████╔╝██║░░██║██║██║░░░░░░░░██║░░░██████╔╝
╚═════╝░░╚════╝░╚═╝░░╚═╝╚═╝╚═╝░░░░░░░░╚═╝░░░╚═════╝░

New Tim Hortons Script for a Tim Hortons MLO I am working on for FiveM
--
--
--

Insert into @qb-smallresources --> server --> consumables.lua
-
-


--Tim Hortons restaruant 

--Drinks
QBCore.Functions.CreateUseableItem("timmies-doubledouble", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Drink", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-tea", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Drink", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-icecap", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Drink", source, item.name)
    end
end)

--Food
QBCore.Functions.CreateUseableItem("timmies-donut", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-donut2", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-donut3", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-egg&muffin", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-timbits", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

QBCore.Functions.CreateUseableItem("timmies-sandwich", function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
	if Player.Functions.RemoveItem(item.name, 1, item.slot) then
        TriggerClientEvent("consumables:client:Eat", source, item.name)
    end
end)

-
-
-- Insert into @qb-smallresources --> config.lua --

ConsumeablesEat = {

-- Tim Hortons
    ["timmies-donut"] = math.random(35, 54),
    ["timmies-donut2"] = math.random(35, 54),
    ["timmies-timbits"] = math.random(20, 45),
    ["timmies-egg&muffin"] = math.random(40, 60),
    ["timmies-donut3"] = math.random(35, 54),
    ["timmies-sandwich"] = math.random(35, 54),
} 

ConsumeablesDrink = {
     -- Timmies
    ["timmies-doubledouble"] = math.random(40, 50),
    ["timmies-icecap"] = math.random(40, 50),

}

--Insert this into @qb-core --> Shared.lua --

-
-


-- Tim Hortons
-- Food
	["timmies-donut"] 				 = {["name"] = "timmies-donut", 			 		["label"] = "Glazed Donut", 					["weight"] = 250, 		["type"] = "item", 		["image"] = "timmies-donut1.png", 					["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Good for the soul."},
	["timmies-donut2"] 			 = {["name"] = "timmies-donut2, 			 	["label"] = "Chocolate Sprinkles", 			["weight"] = 300, 		["type"] = "item", 		["image"] = "timmiesdonut2.png", 			["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Sates Hunger."},
	["timmies-sandwich"] 				 = {["name"] = "timmies-sandwich", 			 	["label"] = "Cold Cut Combo", 		["weight"] = 310, 		["type"] = "item", 		["image"] = "timssandwich.png", 				["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Sates Hunger."},
	["timmies-timbits"] 		 	 = {["name"] = "timmies-timbits", 				["label"] = "Box of Timbits", 			["weight"] = 2500, 		["type"] = "item", 		["image"] = "timbits.png", 			["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Sates Hunger."},
	["timmies-donut3"] 		 	 = {["name"] = "timmies-donut3", 				["label"] = "Honey Gruller", 			["weight"] = 125, 		["type"] = "item", 		["image"] = "honeydonut.png", 			["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Sates Hunger."},
	["timmies-egg&muffin"] 				 	 = {["name"] = "timmies-egg&muffin", 			 	  	["label"] = "Egg & Muffin", 					["weight"] = 125, 		["type"] = "item", 		["image"] = "eggnmuffinsandwich.png", 					["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Sates Hunger."},
		-- Drinks

	["timmies-doubledouble"] 			 	 = {["name"] = "timmies-doubledouble", 				["label"] = "Double Double Coffee", 				["weight"] = 125, 		["type"] = "item", 		["image"] = "doubledouble.png", 				["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A warm soothing coffee to start the day!"},
	["timmies-icecap"] 			     	 = {["name"] = "timmies-icecap", 					["label"] = "Medium Icecap", 				["weight"] = 125, 		["type"] = "item", 		["image"] = "timsicecap.png", 					["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Whipped and ready, enjoy!"},

	--Tim Hortons Ingredients
	["tim-sandwichmeat"] 				 	 = {["name"] = "tim-sandwichmeat", 			 	  		["label"] = "sandwich meat", 						["weight"] = 125, 		["type"] = "item", 		["image"] = "sandwichmeat.png", 						["unique"] = false, 	["useable"] = false, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "An Ingredient"},
	["tim-dough"] 				 	 = {["name"] = "tim-dough", 			 	  		["label"] = "Dough", 			["weight"] = 125, 		["type"] = "item", 		["image"] = "dough.png", 		    		["unique"] = false, 	["useable"] = false, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "An Ingredient"},
	["tim-water"] 				 = {["name"] = "tim-water", 			 		["label"] = "Jug of water", 					["weight"] = 220, 		["type"] = "item", 		["image"] = "waterjug.png", 	    			["unique"] = false, 	["useable"] = false, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "An Ingredient"},
	
(Will add more ingredients)



