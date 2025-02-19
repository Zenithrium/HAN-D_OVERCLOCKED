HAN-D is a tanky melee survivor who can heal himself and his allies to stay in the fight. His melee attacks have high knockback, and comboing them properly will allow him to knock away even the heaviest enemies!

We are looking for translators! Check the languages folder on the [GitHub](https://github.com/Moffein/HAN-D_OVERCLOCKED/tree/master/language) if you would like to submit a translation for your language.
Current Supported Languages: English, Simplified Chinese, Russian, French, Ukrainian

[![](https://i.imgur.com/9pHqh2i.jpg)]()
[![](https://i.imgur.com/5HoCYrq.png)]()

## For Skin Creators

To add custom DRONE models to your HAN-D skin, refer to mdlHANDOverclocked.prefab in the Unity project on the GitHub. The DRONE model is a disabled GameObject attached to the prefab, and the game will attempt to load the textures/mesh from that.

## Installation

Place the HAND_Overclocked folder in /Risk of Rain 2/BepInEx/plugins/  
Settings can be changed in BepInEx/config/com.EnforcerGang.HAND_Overclocked.cfg

## Credits

Moffein - Main dev

TheTimesweeper - HenryMod template, help with Unity/Animations, general polish. You're a lifesaver!

dotflare - HAN-D Model + Anims

LucidInceptor - DRONE Model

PapaZach - Skill Icons

Tera - FOCUS Skill Icon

Vale-X - SWARM_ARMOR Buff Icon

KoobyKarasu - SMASH Skill Icon

Jaysian - Bankroller

## Translation Credits

WockyTheWolf, JunJun_w - Simplified Chinese translation.

MoonsugarCrusader - Russian translation.

FyreBW - French translation.

Damglador - Ukrainian translation.

Sounds taken from Risk of Rain 1 and Starstorm

## Changelog

`1.1.12`

- Updated Ukrainian translation.

`1.1.11`

- Added Ukrainian translation (Thanks Damglador!)

`1.1.10`

- Added French translation (Thanks FyreBW!)

`1.1.9`

- SWARM_ARMOR now supports DroneMeld.

`1.1.8`

- Remembered to mark KingKombatArena as a softdependency so that it will always load before HAN-D.

`1.1.7`

- Updated SMASH to check InputBank instead of CharacterMotor.

`1.1.6`

- Minor tweak to HURT's self-force code.
	- HURT doesn't apply self-force if you are standing still. Before, this was checked via the CharacterMotor's move vector. Now it uses the actual Input move vector to check this.

`1.1.5`

- Fixed Scepter M2 anim not playing online.

`1.1.4`

- Fixed Mastery skin not being unlockable when using the Force Unlock config option.

`1.1.3`

- Fixed game not booting up with the Russian translation.

`1.1.2`

- Added Russian translation (Thanks MoonsugarCrusader!)

`1.1.1`

- Renamed Mastery skin. (Credits to Commando Gaming for the suggestion!)

`1.1.0`

- Added Mastery skin. (Thanks dotflare!)
	- Also thanks to TimeSweeper for getting it working in-game, and improving the mod's skin support!

- Updated portrait icon.
	- Old icon was from an older version of the mod when the textures were different.
	
- Fixed neck becoming tiny when looking backwards.

- SMASH
	- Replaced screenshake with subtle recoil.
	- Now only lunges forward if the forward movement button is pressed.
		- On gamepad, checks if movement input is within 50 degrees of the forward direction on either side.
	- Each enemy hit reduces lunge speed by 50%.
	
	*Adding extra control to this skill's movement. You can now easily choose whether you want to lunge or stay in place.*
	
- FORCED_REASSEMBLY
	- Increased fully charged hit OVERCLOCK extension time from 1.6s -> 2s

- FOCUS
	- Added a -30% speed penalty and +50 armor bonus.
	
	*Trying to make this feel more distinct from OVERCLOCK. Now has better crowdtanking potential, but worse mobility for chasing down enemies to keep your buff active.*
	
- DRONE
	- Healing allies with DRONE will now heal a minimum of 10% of their max HP.
		- Does not apply to your self-heal.
	- Fixed Spare Drone Parts and Illegal Drone Coolant interaction not working
		- DRONES are affected by the attack speed and on-hit effects of both items.
		- DRONES do NOT get the Spare Drone Parts minigun.
	
	*This should fix DRONES not being effective at healing NPCs that use AmbientLevel scaling (ex. Beetle Guards).*

`1.0.2`

- Added Simplified Chinese translation (Thanks WockyTheWolf and JunJun_w!)
- Added Spare Drone Parts item displays.
- Head can now rotate 360 degrees.
- Fixed DRONE not proccing on-impact effects like Behemoth.

`1.0.1`

- Changed default sort position from Before Rex to After MUL-T

`1.0.0`

- Rewrote the mod.
- Added new model + anims (made by dotflare)
- Added alt Primary and alt Utility.
- Added unlock condition.
	- Can be bypassed with Force Unlock config option.
- SWARM_ARMOR now gives damage reduction instead of armor.
- Added EmoteAPI support.
- Added ItemDisplays
- Added 3 built-in emotes.

*Special thanks to Jaysian for commissioning dotflare for the new HAN-D Model/Anims!*