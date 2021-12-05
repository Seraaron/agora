---
alias:
  - martial combat
  - combat
tags:
  - CC-BY
  - conflict
  - subsystem
  - martial
author: Seraaron
license: CC BY 4.0
date created: 2021-10-20+1200
date updated: 2021-11-30 20:46
---

# Martial Combat

When a situation is turning into a fight with multiple combatants and **your differences can't be resolved by any means other than violence**; when you each know deep down that in order to leave this place alive today you'll need to muster all your skills and either kill your opponents outright, capture them, or make them flee; _this is when combat begins_.

Martial combats are most often utilized in games that feature high adventure, dungeon crawling, and wilderness exploration, or frequent encounters with [[Beasts & Nightmares]]. If the fight is more one-sided, with one side intending to murder the other and the other side wants to just escape from the start, then consider using a [[Chase Scene]] or just a simple [[Opposed Tasks|Opposed task]] instead.

Before you get into clashing steel or spilling any blood, there's a little bit of bookeeping and set up to do first, to ensure that the battle runs smoothly for all the players:

- **Each combatant must determine three things: [[#Positions]], [[#Poise]], and [[#Disposition]], in that order**.
- **The other important number to keep an eye on during the fight is [[Momentum]]**, which governs how intense the fight is getting and how close anyone is to being easily pacified.

> ### Nb.
> This system functions very similarly to [[Social Discourse|social discourse]], except using #martial jobs instead of #social ones. It can be used to run anything from single-opponent duels to small-scale military engagements, but it will become tedious and difficult to run with more than a dozen combatants.

## Positions

We generally aren't too concerned about tracking the exact positions of all the participants at all times in a combat, and [[Agora]] does not inherently require any kind of tile-sets or figurines to be played (though feel free to use visual aides if you wish to).

Instead, you should try to **gauge your position _relative to your target_ only when it's important**. These distances are broken down into five main brackets, indexed from 0 to 4 and usually called '**Close-Quarters**', '**Within a Few Paces**', '**Nearby**', '**Far Away**', and '**Remote**', using natural language.

#important Moving to a 'Remote' position will effectively place you outside of the battle, unless you have a long-ranged weapon (in which case see [[#Shooting into the Fray]], below).

### Starting Position

When the combat begins, your [[Facilitator]] will generally decide how close or far away everyone is from each other, based on all the descriptions so far.

> ### Eg.
> If there was a dialogue scene before the fight erupted, then everyone will probably start at the close-quarters range.
>
> If you're being ambushed in a valley, then you'll be at the center of the conflict and your enemies will be at nearby ranges on either side.

#important Avoid starting everyone too far away, because you'll either spend the first three rounds closing the distance, which will be very boring, or someone will just get out of range and  leave the battle.

---

###### Approximate Distances

|     | Bracket                     | _Appx. Feet_ | _Appx. Meters_ | Grid Sqs. |
| :-: | --------------------------- | :----------: | :------------: | :-------: |
|  0. | **Close-Quarters (Melee):** |    _~0-8_    |     _~0-2_     |    1-2    |
|  1. | **Within a Few Paces:**     |    _~8-30_   |     _~2-9_     |    2-6    |
|  2. | **Nearby:**                 |   _~30-100_  |     _~9-30_    |    6-20   |
|  3. | **Far Away:**               |  _~100-300_  |    _~30-90_    |   20-60   |
|  4. | **Remote:**                 |    _>300_    |      _>90_     |    >60    |

#question Grid square equivalents are also provided here for those that _do_ prefer to use visual aids, tile maps, and figurines.

---

### Ebb and Flow

The center of a battle is always moving, shifting across the terrain as small victories and minor losses blend together. This natural movement of combatants is accommodated into the positioning brackets, so that most characters involved a martial combat will always be within a few paces of one another.

As such, **whenever you use an offensive move with a melee weapon, you can automatically move from within a few paces to the close-quarters of your target**, as a free action, if you need to.

## Poise

Poise represents _your confidence in your armor or skill at dodging attacks, combined with your relative positioning, the weather, visibility, and cover usage_. **Poise is the minimum difficulty for most offensive moves used against you in the conflict**. First, let the [[Facilitator|FC]] describe the battlefield, the combatants, and any important objects in your nearby surroundings, **then calculate your Poise as follows:**

$$
roundup \left( (highest(Acrobat, Armor) + Helm + 0..3) \div 2 \right) + Shield
$$

That is:

- Start with the _highest_ of:
	- Your **[[Acrobat]]  level**
	- Your **Armor dice**
		- (ie. usually based on materials and weight)
- Then and your **Helm dice**, and some conditional benefits:
	- Add +1 _if you're on unstable, icy, or sloped terrain, or if fighting on a boat?_
	- Add +1 _if you're fighting in darkness, low visibility, or if fighting in bad weather?_
	- Add +1 _if there's lots of cover nearby, such as trees, rocks, pillars, crates, or the corners of buildings?_
- Divide the total by 2 and round up!
- Lastly, add your **Shield dice**.

Since you will need to quote this number to other players frequently, **write it down on your [[Character Sheets|character sheet]]**, or somewhere easy to see. Poise is also is also _added_ to your starting [[#Disposition]], but it otherwise remains static.

Poise only gets recalculated if you [[Disarm|drop]] or [[#Optional Shields Shall be Shattered|shatter]] your shield or if the environment you're fighting in changes drastically.

### Alternative Poise Jobs?

If you're mounted, riding a vehicle, or flying then you must instead use your [[Rider]], [[Driver]], or [[Pilot]] level, respectively, instead of [[Acrobat]]. You may also add a final bonus from your ride's #barding dice instead of your #shield.

## Disposition

Disposition here represents _the strength of your morale and spatial awareness or your sense of tactics and general disposition for violence, combined with your reaction speed relative to the other combatants_. Disposition does three main things during a fight:

- **It decides _the turn order_  (or 'initiative') for all combatants, from highest to lowest, which you can track using a [[momentumGrid.svg|grid of numbers]] and a token that represents your character. **
- **It is the amount of [[Momentum]] that is needed for an opponent to try to _[[Pacify]] you with no major penalties_**.
- **If you hit zero Disposition during the fight then you must either flee, surrender, or faint, or else you may be automatically _pacified_ by another character.**

### Roll Disposition!

Describe how you prepare yourself for the upcoming conflict, and thus which job you'll be using. **Your current [[Health]] score is also added to this roll as bonus dice**. If multiple reasons apply at once, then just choose the one you'd prefer to roll:

- **[[Guard]] + [[Health]]:** _You are being ambushed, you're starting the fight up close, you're defending a strategic location, or this is a duel._
- **[[Skirmisher]] + [[Health]]:** _You are initiating an ambush, you're starting the fight at a distance, you're attacking a strategic location, or this is a duel._

This roll works a lot more like a [[Checks|Check]], in that **you're just looking to count successes here**. There's no inherent difficulty or factors either.

### Base Disposition

**The successes from the job roll above are added to a base Disposition score** — which depends on the number of other combatants, using the table below — **in addition to your [[#Poise|Poise]]**, to give you a total Disposition.

The number of combatants also determines roughly how long each round is, in-game. Though the mechanical effect of this is minimal, it may help you to describe your movements and actions, and to get a sense of scale:

| № of Combatants | Base Disposition | _Appx. Round Duration_ |
| --------------: | :--------------: | ---------------------- |
|           **2** |        10        | _~5 sec_               |
|         **3-4** |        15        | _~10 sec_              |
|         **5-7** |        20        | _~20 sec_              |
|        **8-11** |        25        | _~40 sec_              |
|        **≥ 12** |        30        | _~80 sec_              |

#question [[Non-player Characters|NPCs]] usually use preset Poise and Disposition scores.

![[Momentum]]

## Stances

**At the start of each round, each standing combatant must choose and announce which 'stance' they enter.**

The announcement of your stance can just be verbal, if you like, or you can use slips of paper and write your stance on it, **or playing card suits** (ie. hearts ♥, spades ♠, diamonds ♦, and clubs ♣), and then all reveal your writings at the same time.

Your stance determines _how much [[Momentum]] you add to the conflict at this start of the round_, and which [[#Moves|moves]] you can choose from on your turn:

| ♣ **Aggressive Stance** ♣                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _This is pushing forward. You are attacking quickly and boldly, but also leaving yourself open to be flanked or outmaneuvered if there are other combatants around._ |
| _**Momentum**_ +2                                                                                                                                                    |
| _**Moves:**_  [[Assault]], [[Spur]], [[Flank]] (Charge), [[Pacify]] (Any), or [[Interact]]                                                                           |

| ♠ **Counteractive Stance** ♠                                                                                                                                      |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _This is holding the line. You are attacking occasionally, when you see a good opportunity, but you are otherwise keeping your guard up and trying to stay safe_. |
| _**Momentum**_ +1                                                                                                                                                 |
| _**Moves:**_ [[Flank]] (Any), [[Spur]], [[Rally]], [[Pacify]] (Grapple), or [[Interact]]                                                                          |

| ♦ **Defensive Stance** ♦                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| _This is pulling backward. You are mostly defending yourself, using every dodge, parry, and block in your repertoire, while trying to catch your breath or do something else._ |
| _**Momentum**_ +0                                                                                                                                                              |
| _**Moves:**_ [[Rally]], [[Reposition]], [[Treat]], [[Pacify]] (Intimidate), [[Flank]] (Disarm), or [[Interact]]                                                                |

#important Once you've made your decision, the only way to change your stance in the middle of a round is via the 'Change Stance' [[#Exploits|exploit]].

> ### Nb.
> The stance you choose each round should also depend on how you describe your character's actions, but don't worry too much if your descriptions don't match up exactly with your actions, your intentions are more important here.

### Prone

Some strikes can leave you staggered or knocked to the ground, which is a very vulnerable position to be in. While speechless:

- **Your [[#Presence]] is reduced to 0**,
- You cannot use any move or exploit that would change your position, and
- _Your next move suffers a +1 difficulty penalty_.

You may _stand up_ on your turn using the [[Interact]] move, to remove the effect immediately, or you can suffer through the penalties and use the move you were intending to use from the ground, then _automatically remove the effect and stand up at the end of the round_. Otherwise you must _use the 'Shake Off' [[#Exploits|exploit]]_, to stand up early.

### Hesitation

Some attacks can cause 'hesitation'. This simply means that **your next move roll suffers a +1 difficulty penalty**, and it's cleared immediately afterwards. _The only way to remove hesitation before a roll is to use the 'Shake Off' [[#Exploits|exploit]]_.

#important If multiple sources are causing hesitation _while you're already hesitating_ then **they do not stack**.

## Turn Order

**Start with the character who currently has the _highest_ Disposition, and progress the turn order down to the _lowest_**. A turn consists of: Rolling momentum, [[#Martial Moves List|choosing a move]], performing that move, and squeezing in any [[#Free Actions|free actions]] if you want.

#question You can only act outside of your turn if you're given the opportunity to use an [[#Exploits|exploit]] by another character.

### Rounds

**Once every combatant has had a chance to act, a 'round' is said to have passed**.

At the end of each round, if a character's Disposition has raised or lowered for any reason, then they will move up or down the turn order, respectively. To make sure that no one accidentally goes twice or has their turn skipped, **only apply Disposition changes at the end of each round**.

#important Each player need only track how much their own Disposition will change and _then tell the FC at the end of that round_, so their position on the momentum grid can be updated.

### Tied Disposition

If two or more characters have equal dispositions, then **they have to effectively take their actions simultaneously** on the same turn. This isn't physically possible in _out-of-game game time_, since each turn must be separately adjudicated, but _in game_ any "immediate" effects of each character's moves' are all applied instead at the end of the _collective turn_.

### No Disposition

If you're reduced to zero Disposition at the end of a round then you will collapse from exhaustion, or will be paralyzed with fear, and are _effectively treated as an unconscious combatant_. Unconscious combatants count as being [[#Prone|prone]], except _they can't use any moves_, and they may be automatically pacified.

#question Using the [[Pacify]] move on a character with zero Disposition will automatically succeed without need for a roll, unless you are trying to kill them (in which case make a [[Grit]] check).

## Martial Actions

There are three types of action a character can perform in combat each round: **[[#Moves]]**, **[[#Free Actions]]**, and **[[#Exploits]]**.

It is best to describe your actions first — according to your stance — then choose the move and job that best match what you said. You can also do it in reverse if you prefer though: Choosing the job and move first, and the describing how your character acts to get there.

### Moves

Moves are the _main actions_ available to you each [[#Turn Order|turn]], determined by your current [[#Stance Choice|stance]], and almost all moves require a job roll to be executed successfully (similar to a [[Tasks|Task]] roll but with most of the details already worked out for you).

**There are eight moves in total, which can be grouped into two categories, or four rough pairs:**

|     Offense |  —  | Utility        |
| ----------: | :-: | :------------- |
| [[Assault]] |  —  | [[Treat]]      |
|    [[Spur]] |  —  | [[Rally]]      |
|   [[Flank]] |  —  | [[Reposition]] |
|  [[Pacify]] |  —  | [[Interact]]   |

**Offensive** moves tend to either damage your opponent's Disposition, inflict [[Stress]], or cause other status effects, and benefit from the +MD; whereas **Utility** moves tend to either repair that damage, or let you change positions, or cause different kinds of effects.

- **A move can only be performed if you're in the right [[#Stance Choice|stance]] to use it**.
- Most moves require a particular [[Jobs|job]] or a choice of jobs to be used properly. (When you see the double-bar symbol ∥ it means 'or' — _choose one_).
- The bonuses and difficulties of the roll are all worked out as you read down the move, and should be fairly self-explanatory.
	- Though some moves also require you to be in the right postion, or to use the right kinds of [[Gear List#Weapons|weapons]], to get the most benefit from them.
- You _may_ [[KISSing|KISS]] move rolls, but remember to _keep it short and sweet_.
	- _[[Earning Experience|exp]]_ from KISSing may be applied immediately, but no exp is earned from a failed move roll.
- **You may not use the same move two rounds in a row**.

#question See the [[#Martial Moves List]] below to read each move separately, or print off the [[move cards]] from the resources chapter.

### Free Actions

Every combatant can only attempt to use one move per round, but they may also take any of the following _free actions_ on their turn:

- **Yell** — Shout out at the top of your lungs. _Single words or easy phrases only_.
- **Look** — Briefly take in your surroundings: Ask a simple question to your [[Facilitator|FC]] about the battle, such as the location and proximity of anything important in the scenery, or the positions of your enemies relative to you or your allies.
- **Drop** — Let go of something you're holding, like a weapon or another object, or an opponent you've grappled to the ground, or drop your concentration on a spell, or drop yourself [[#Prone|prone]].

Anything else that can be reasonably resolved with a simple [[Checks|Check]] in the middle of a fight may be deemed a free action by your [[Facilitator|FC]], so long as it doen't give any advantage over your opponents.

### Exploits

When an opponent uses a move against you that says _“your opponent may exploit you”_ as a failure consequence — which most offensive moves say, for example — this means that **you may choose one following responses** (as an immediate free action):

- **Dodge / Parry:** You deftly avoid your opponent's attack at the last moment, or beat it aside with your weapon or shield, which leaves them off-balanced and staggered, and counts as [[#Hesitation|hesitation]] on their next roll (ie. _+1 difficulty factor, which can stack with other penalties_).
- **Change Stance:** If you haven't had your turn yet, you may _change to a different stance_ from the one you chose at the start of the round. _This does not change the Momentum you already generated_.
- **Shake Off:** If you are currently [[#Hesitation|hesitating]], [[#Prone|knocked prone]], or otherwise hindered, they may shake it off and _remove all penalties or negative status effects_ that are afflicting them (or you may remove a point of stress from assaults, but only _temporarily_).
- **Raise the Stakes:** You riposte, and raise the Momentum of the battle for everyone by your opponent's [margin of failure] on their roll against you.
- **Break Away:** You may _move one distance bracket away_ from your opponent, without incurring any penalties or exploits from other combatants.

When you exploit an opponent, be sure to **describe what you do or say in response**, in proportion to their failure. This helps to keep everyone immersed in the action, so that the interaction isn't _purely mechanical_.

## Martial Moves List

When you come to choose your move each turn, it's okay if you'd prefer to describe your action first and then use that description to guide you towards a certain move and job choice, or you can make the mechanical decision first and let that guide how you act. This mostly comes down to personal preference, but your weapon choice and position relative to your target will also dictate some of the choices for you.

![[Assault]]

![[Treat]]

![[Spur]]

![[Rally]]

![[Flank]]

![[Reposition]]

![[Pacify]]

![[Interact]]

![[Shields Shall be Shattered]]

## Finishing a Fight

#unfinished

### Experience from Conflict

Instead of tracking your failures during a combat, which would slow down the game's pace, **you earn _[[Earning Experience|exp]]_ equal any [[Lots]] spent plus the MD bonus that the fight ended on**, and you must distribute those points _relatively evenly_ among all the jobs you rolled with during the battle.

## Shooting into the Fray

Weapons with the #hunter tag cannot be shot from a 'remote' range, whereas #archer and #gunner weapons *can be*, but they suffer a +3 difficulty penalty to all attacks, unless the weapon has a scope and then it's only a +1 penalty.

Also if your shooting into a conflict from remote range and miss, ...

#unfinished
