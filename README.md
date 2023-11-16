# ASA-Imprint-Kibble

This mod is inspired by the Magic Treat mod by Zogniton: https://www.curseforge.com/ark-survival-ascended/mods/magic-treat. It aims to be a more customizable version of this mod.

This mod adds an "Imprint Kibble" that can be learned at level 16 for 0 engram points and crafted in a cooking pot/industrial cooker.

This kibble can be fed to a baby dinosaur or an adult female dinosaur.
If fed to a baby dinosaur, the kibble will increase imprint percentage and increase growth speed.
If fed to an adult female dinosaur, the kibble will provide a buff for a limited time. This buff will increase mutation chance, skip mating cooldown, and increase gestation speed.

Config options:
These are the settings that can be added to your GameUserSettings.ini file to customize this mod, with the default values:

[ImprintKibble]
EnableImprintQuality=True
ImprintQuality=1.0
EnableExtraMatureSpeed=True
ExtraMatureSpeed=2.0
EnableMutationBuff=True
EnableNoMatingCooldownBuff=True
EnableExtraMutationChanceBuff=True
ExtraMutationChance=1.0
EnableExtraMutationsBuff=True
NumberOfMutations=1
EnableExtraGestationSpeed=True
ExtraGestationSpeed=5.0
MutationBuffTimer=1800.0


EnableImprintQuality: Enables the ability for the Imprint Kibble to increase imprint percentage on a baby dinosaur. Default: True

ImprintQuality: The amount of imprint percentage one Imprint Kibble will add to a baby dinosaur. Range of 0.0 to 1.0 (1.0 = 100%, 0.3 = 30%, 0.05 = 5%, etc.). Default: 1.0

EnableExtraMatureSpeed: Enables the ability for the Imprint Kibble to increase the maturation speed of a baby dinosaur. Default: True

ExtraMatureSpeed: The multiplier that the baby dinosaur's maturation speed will increase by. This will equal your BabyMatureSpeedMultiplier x ExtraMatureSpeed. Default: 2.0

EnableMutationBuff: Enables the buff that the Imprint Kibble gives an adult female dinosaur. Default: True

EnableNoMatingCooldownBuff: Enables the Imprint Kibble buff to remove the mating cooldown. Default: True

EnableExtraMutationChanceBuff: Enables the Imprint Kibble buff to increase the odds of a baby dinosaur receiving a mutation. Default: True

ExtraMutationChance: The chance of a baby dinosaur recieving mutation(s). Range of 0.0 to 1.0 (1.0 = 100%, 0.3 = 30%, 0.05 = 5%, etc.). Default: 1.0

EnableExtraMutationsBuff: Enables the Imprint Kibble buff to change the amount of mutations a baby dinosaur can receive. Default: True

NumberOfMutations: The number of mutations a baby dinosaur can get. Further explanation on this below. Default: 1

EnableExtraGestationSpeed: Enables the Imprint Kibble buff to increase the gestation speed of an adult dinosaur. Default: True

ExtraGestationSpeed: The multiplier that the parent dinosaur's gestation speed will increase by. This will equal your EggHatchSpeedMultiplier x ExtraMatureSpeed. Default: 2.0

MutationBuffTimer: The amount of time the Imprint Kibble buff will last. Default: 1800.0 (30 minutes)
 

ExtraMutationChance and NumberOfMutations:
In ASA, the value for ExtraMutationChance=0.025 (2.5%) and the value for NumberOfMutations=3
This means you have 3 2.5% chances to get a mutation, which is how you can get up to 3 mutations on a single baby
If you want to make the buff double mutation odds you can do ExtraMutationChance=0.05 and NumberOfMutations=3
If you want to make the buff give 10 guaranteed mutations you can do ExtraMutationChance=1.0 and NumberOfMutations=10
The default is just one guaranteed mutation, ExtraMutationChance=1.0 and NumberOfMutations=1
