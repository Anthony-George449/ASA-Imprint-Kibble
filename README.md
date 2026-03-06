# ASA-Imprint-Kibble

Imprint Kibble
==============
Mod ID: 939234

Spawn code: cheat giveitem "/Script/Engine.Blueprint'/ImprintKibble/PrimalItemConsumable_ImprintKibble.PrimalItemConsumable_ImprintKibble'" 1 0 0

This mod is inspired by the Magic Treat mod by Zogniton: https://www.curseforge.com/ark-survival-ascended/mods/magic-treat. It aims to be a more customizable version of this mod.

Description
--------------
This mod adds an "Imprint Kibble" that can be learned at level 16 for 0 engram points and crafted in a cooking pot or industrial cooker.

This kibble can be fed to a baby dinosaur or an adult female dinosaur.

If fed to a baby dinosaur, the kibble will increase imprint percentage and increase growth speed.

If fed to an adult female dinosaur, the kibble will provide a buff for a limited time. This buff will increase mutation chance, skip mating cooldown, and increase gestation speed.


Config options - GameUserSettings.ini
--------------
These are the settings that can be added to your GameUserSettings.ini file to customize this mod, with the default values:

[ImprintKibble]

EnableMutationBuff=True

MutationBuffTimer=1800.0

EnableImprintQuality=True

ImprintQuality=1.0

EnableExtraMatureSpeed=True

ExtraMatureSpeed=2.0

EnableNoMatingCooldownBuff=True

EnableExtraMutationChanceBuff=True

ExtraMutationChance=1.0

EnableExtraMutationsBuff=True

NumberOfMutations=1

PointsPerMutation=2.0

EnableFasterGestation=True

ExtraGestationInterval=6.0

ExtraGestationPercentage=0.01

EnableMatingTimeReduction=True

MatingTime=5.0

EnableAdultKibbleCooldown=False

AdultKibbleCooldownTime=1800.0

EnableBabyKibbleCooldown=False

BabyKibbleCooldownTime=1800.0

Config options - Game.ini
--------------
These are the settings that can be added to your Game.ini file to customize the crafting cost, unlock level, and engram point cost.

The example below would set the engram point cost to 10, the unlock level to 75, and would change the crafting cost to 3 raw meat + 2 element. Edit these as you see fit:

OverrideNamedEngramEntries=(EngramClassName="EngramEntry_ImprintKibble_C", EngramHidden=false, EngramPointsCost=10, EngramLevelRequirement=75)

ConfigOverrideItemCraftingCosts=(ItemClassString="PrimalItemConsumable_ImprintKibble_C",BaseCraftingResourceRequirements=((ResourceItemTypeString="PrimalItemConsumable_RawMeat_C",BaseResourceRequirement=3.0,bCraftingRequireExactResourceType=false),(ResourceItemTypeString="PrimalItemResource_Element_C",BaseResourceRequirement=2.0,bCraftingRequireExactResourceType=false)))

Config Description - GameUserSettings.ini
------------------

EnableMutationBuff: Enables the buff that the Imprint Kibble gives an adult female dinosaur. Default: True

MutationBuffTimer: The amount of time the Imprint Kibble buff will last. Default: 1800.0 (30 minutes)

EnableImprintQuality: Enables the ability for the Imprint Kibble to increase imprint percentage on a baby dinosaur. Default: True

ImprintQuality: The amount of imprint percentage one Imprint Kibble will add to a baby dinosaur. Range of 0.0 to 1.0 (1.0 = 100%, 0.3 = 30%, 0.05 = 5%, etc.). Default: 1.0

EnableExtraMatureSpeed: Enables the ability for the Imprint Kibble to increase the maturation speed of a baby dinosaur. Default: True

ExtraMatureSpeed: The multiplier that the baby dinosaur's maturation speed will increase by. This will equal your BabyMatureSpeedMultiplier x ExtraMatureSpeed. Default: 2.0

EnableNoMatingCooldownBuff: Enables the Imprint Kibble buff to remove the mating cooldown. Default: True

EnableExtraMutationChanceBuff: Enables the Imprint Kibble buff to increase the odds of a baby dinosaur receiving a mutation. Default: True

ExtraMutationChance: The chance of a baby dinosaur receiving mutation(s). Range of 0.0 to 1.0 (1.0 = 100%, 0.3 = 30%, 0.05 = 5%, etc.). Default: 1.0

EnableExtraMutationsBuff: Enables the Imprint Kibble buff to change the number of mutations a baby dinosaur can receive. Default: True

NumberOfMutations: The number of mutations a baby dinosaur can get. Further explanation on this below. Default: 1

PointsPerMutation: The stat points a single mutation gives. ASA gives 2 by default. Default: 2.0

EnableFasterGestation: Enables the Imprint Kibble buff to increase the gestation speed of an adult dinosaur. Default: True

ExtraGestationInterval: The interval that the gestation time will increase by the ExtraGestationPercentage. Further explanation on this below. Default: 5.0

ExtraGestationPercentage: The percentage that the gestation bar will increase every ExtraGestationInterval. Range of 0.0 to 1.0 (1.0 = 100%, 0.3 = 30%, 0.05 = 5%, etc.). Default: 0.05

EnableMatingTimeReduction: Enables the Imprint Kibble buff to reduce the amount of time it takes 2 dinos to mate. Default: True

MatingTime: How long it takes the mating bar to fill up. Default: 5.0

EnableAdultKibbleCooldown: Enables giving an adult dino a cooldown after using the Imprint Kibble. The dino can still eat a kibble, but will not get any benefit. Further explanation below. Default: False

AdultKibbleCooldownTime: How long an adult dino has to wait before being able to benefit from an Imprint Kibble again. Default: 1800.0 (30 minutes)

EnableBabyKibbleCooldown: Enables giving a baby dino a cooldown after using the Imprint Kibble. The dino can still eat a kibble, but will not get any benefit. Further explanation below. Default: False

BabyKibbleCooldownTime: How long a baby dino has to wait before being able to benefit from an Imprint Kibble again. Default: 1800.0 (30 minutes)
 


ExtraMutationChance and NumberOfMutations
-----------------------------------------

In ASA, the value for ExtraMutationChance=0.025 (2.5%) and the value for NumberOfMutations=3

This means you have 3 2.5% chances to get a mutation, which is how you can get up to 3 mutations on a single baby

If you want to make the buff double mutation odds you can do ExtraMutationChance=0.05 and NumberOfMutations=3

If you want to make the buff give 10 guaranteed mutations you can do ExtraMutationChance=1.0 and NumberOfMutations=10

The default is just one guaranteed mutation, ExtraMutationChance=1.0 and NumberOfMutations=1


ExtraGestationInterval and ExtraGestationPercentage
-----------------------------------------

Example: ExtraGestationInterval=6.0 and ExtraGestationPercentage=0.01.

This means that every 6.0 seconds, the gestation bar will increase by an extra 1%, and it will take 600 seconds (10 minutes) for a dinosaur to finish gestating.

This time will be the same for every dino. So a Mosasaurus will take the same amount of time to gestate as a Phiomia would with this setting.

AdultKibbleCooldown and BabyKibbleCooldown
-----------------------------------------
These settings will allow you to customize how frequently the Imprint Kibble benefits can be granted. After the Imprint Kibble buff falls off, it is replaced by a debuff that will prevent the benefits of the Imprint Kibble.

The debuff that is applied will carry over to adulthood for a baby dino. Let me give an example using the following settings:
EnableAdultKibbleCooldown=True
AdultKibbleCooldownTime=60.0
EnableBabyKibbleCooldown=True
BabyKibbleCooldownTime=1800.0

In this case, an adult dino would have to wait 60 seconds between receiving the Imprint Kibble buff, and a baby would have to wait 30 minutes (1800 seconds). However, let's say your baby only takes 10 minutes to fully grow after using the Imprint Kibble on it. If you then wanted to replace the previous adult dino with the fully grown baby, the baby would still have 20 minutes left on the debuff timer, which means you have to wait 20 minutes before using the Imprint Kibble on the grown baby. This allows you to customize how quickly players can cycle mutations.
