# ap-weedpicking
A simple QB-target Weed Picking and Drying Script

add this to your qb-target init.lua

Config.BoxZones = {
	["weeddrying"] = {
        name = "weeddrying",
        coords = vector3(-113.0726, -11.14904, 69.51),
        length = 1.2,
        width = 1.2,
        heading = 135,
        debugPoly = false,
        minZ = 69.51,
        maxZ = 70.74,
        options = {
            {
                type = "client",
                event = "qb-weedpicking:dryIngCannabis",
                icon = "fas fa-cannabis",
                label = "Dry Weed",
            }
        },
        distance = 2.5
    },
}

-------------------------------------------------------------------------

Config.TargetModels = {
	["weedpicking"] = {
        models = {
            "prop_weed_01",
        },
        options = {
            {
                type = "client",
                event = "qb-weedpicking:pickedUpCannabis",
                icon = "fas fa-cannabis",
                label = "Weed Picking",
            },
        },
        distance = 2.5,
    },
