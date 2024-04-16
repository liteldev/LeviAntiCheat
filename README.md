# LeviAntiCheat

English | [简体中文](README-zh_CN.md)

Powerful anti-cheating for LeviLamina

## Install

```bash
lip install github.com/LiteLDev/LeviAntiCheat
```

## Commands

`/lac ban <Player> [reason] [duration(minute)]` Ban a player manually
`/lac unban <Player>` Pardon a player manually

## Configuration File

```jsonc
{
    "version": 1,
    "consoleLog": true,
    "worldSafety": {
        "fakeSeed": {
            "enable": true,
            "randomSeed": false,
            "seed": 0
        },
        "offlineInventoryProtection": false,
        "illegalBreakingCheck": true
    },
    "cheatPrevention": {
        "antiXray": {
            "enable": true,
            "DimensionConfigs": {
                "overworld": {
                    "Enable": true,
                    "EngineMode": 2,
                    "UpdateRadius": 2.0,
                    "MaxBlockHeight": 64,
                    "HiddenBlocks": [
                        "minecraft:copper_ore",
                        "minecraft:deepslate_copper_ore",
                        "minecraft:raw_copper_block",
                        "minecraft:deepslate_coal_ore",
                        "minecraft:diamond_ore",
                        "minecraft:deepslate_diamond_ore",
                        "minecraft:gold_ore",
                        "minecraft:iron_ore",
                        "minecraft:deepslate_gold_ore",
                        "minecraft:deepslate_iron_ore",
                        "minecraft:raw_iron_block",
                        "minecraft:lapis_ore",
                        "minecraft:deepslate_lapis_ore",
                        "minecraft:redstone_ore",
                        "minecraft:deepslate_redstone_ore",
                        "minecraft:coal_ore"
                    ],
                    "ReplacementBlocks": [
                        "minecraft:stone",
                        "minecraft:deepslate"
                    ]
                },
                "nether": {
                    "Enable": true,
                    "EngineMode": 3,
                    "UpdateRadius": 2.0,
                    "MaxBlockHeight": 128,
                    "HiddenBlocks": [
                        "minecraft:ancient_debris",
                        "minecraft:nether_gold_ore",
                        "minecraft:quartz_ore"
                    ],
                    "ReplacementBlocks": [
                        "minecraft:netherrack"
                    ]
                },
                "the end": {
                    "Enable": false,
                    "EngineMode": 1,
                    "UpdateRadius": 2.0,
                    "MaxBlockHeight": 0,
                    "HiddenBlocks": [],
                    "ReplacementBlocks": []
                }
            }
        },
        "antiToolbox": true,
        "antiFakeName": true,
        "antiSpawnXpOrbs": true,
        "antiXpHack": true
    },
    "bugFixes": {
        "uiItemDuplicateFix": true,
        "sleepTeleportFix": true
    },
    "inventoryManagement": {
        "antiAutoOffhand": true,
        "rectifyUiItemDrop": true,
        "invalidItemDetection": true,
        "anvilEnchantLimits": true,
        "invalidStackDetection": true,
        "antiInvalidNbtItem": true,
        "banItem": {
            "enable": true,
            "blacklist": []
        },
        "enchantCheck": {
            "enable": false,
            "maxEnchantLevel": {
                "example_enchant": 5
            }
        }
    },
    "playerInteractions": {
        "illegallyTradeRestrictions": true,
        "antiSpam": {
            "enable": true,
            "maxChatLength": 60,
            "maxRate": 1
        },
        "itemNameLengthCheck": {
            "enable": true,
            "maxStringLength": 90
        }
    },
    "movement": {
        "containerMoveCheck": true,
        "illegalMovementCheck": true,
        "timerCheck": {
            "enable": true,
            "maxPacketSpeed": 24,
            "detectLevel": 15
        },
        "noPacketCheck": {
            "enable": true,
            "maxNoPacketTime": 5
        }
    },
    "combat": {
        "autoClickCheck": {
            "enable": true,
            "maxCps": 10,
            "detectLevel": 10
        },
        "reachDistanceCheck": {
            "enable": true,
            "detectLevel": 5
        }
    },
    "securityMeasures": {
        "antiLoginFloodCheck": false
    },
    "punish": {
        "enable": true,
        "kickVL": 100,
        "banVL": -1,
        "banDuration": 0
    }
}
```

## Features

### Bugfixes

- Fix UI item duplication
- Fix sleep teleport

### Client Cheating

- Prevent X-ray vision of minerals
- Prevent Toolbox using
- Prevent auto click
- Prevent Reach
- Prevent fake name
- Prevent spawn xp orbs
- Prevent `xp` hack
- 

### Inventory

- Check anvil enchantment
- Prevent automatic tool selection
- Prevent invalid items
- Prevent invalid nbt items
- Ban illegal items
- Check enchantment level
- Prevent invalid stack
- Prevent some resource packs cheating

### Movement

- Prevent interacting with containers while moving
- Prevent illegal movement such as fly, speed hack, wall hack
- Prevent NoPacket
- Prevent Timer(another type of speed hack by adjust client's speed)

### Interaction

- Prevent illegal trades
- Prevent long item nametag
- Prevent spam(including selector spam, command spam etc.)

### Secure

- Prevent LoginFlood attack

### World

- Fake seed
- Prevent illegal breaking
- Patch player's inventory when online mode is off

## Contributing

Ask questions by creating an issue.

Since this project is closed source, you can't contribute to the code directly.

## License

Copyright © LiteLDev
