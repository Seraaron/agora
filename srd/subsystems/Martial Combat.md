---
alias:
  - martial combat
  - combat
tags:
  - creativecommons
  - conflict
  - subsystem
  - martial
author: Seraaron
license: CC BY 4.0
date created: 2021-10-20+1200
last updated: Wednesday 2021-10-20 12:39:05 (UTC+0100)
date updated: 2021-11-17 15:31

---

## Martial Combat

When a situation is turning into a fight with multiple combatants and **your differences can't be resolved by any means other than violence**; when you each know deep down that in order to leave this place alive today you'll need to muster all your skills and either kill your opponents outright, capture them, or make them flee; _this is when combat begins_.

Martial combats are most often utilized in games that feature high adventure, dungeon crawling, and wilderness exploration, or frequent encounters with [[Beasts & Nightmares]]. If the fight is more one-sided, with one side intending to murder the other and the other side wants to just escape from the start, then consider using a [[Chase Scene]] or just a simple [[Opposed Tasks|Opposed task]] instead.

Before you get into clashing steel or spilling any blood, there's a little bit of bookeeping and set up to do first, to ensure that the battle runs smoothly for all the players:

-   **Each combatant must determine three things: [[#Starting Position|Positions]], [[#Poise|Poise]], and [[#Stamina|Stamina]], in that order**.
-   **The other important number to keep an eye on during the fight is [[Momentum]]**, which governs how intense the fight is getting and how close anyone is to being easily pacified.

> #nb
> This system functions very similarly to [[Social Discourse|social discourse]], except using #martial jobs instead of #social ones. It can be used to run anything from single-opponent duels to small-scale military engagements, but it will become tedious and difficult to run with more than a dozen combatants.

### Positions

We generally aren't too concerned about tracking the exact positions of all the participants at all times in a combat, and [[Agora]] does not inherently require any kind of tile-sets or figurines to be played (though feel free to use visual aides if you wish to).

Instead, you should try to **gauge your position _relative to your target_ only when it's important**. These distances are broken down into five main brackets, indexed from 0 to 4 and usually called '**Close-Quarters**', '**Within a Few Paces**', '**Nearby**', '**Far Away**', and '**Remote**', using natural language.

#imp Moving to a 'Remote' position will effectively place you outside of the battle, unless you have a very-long ranged weapon (in which case see [[#Shooting into the Fray]], below).

#### Starting Position

When the combat begins, your [[Facilitator]] will generally decide how close or far away everyone is from each other, based on all the descriptions so far.

> #eg
> If there was a dialogue scene before the fight erupted, then everyone will probably start at the close-quarters range.
>
> If you're being ambushed in a valley, then you'll be at the center of the conflict and your enemies will be at nearby ranges on either side.

#imp Avoid starting everyone too far away, because you'll either spend the first three rounds closing the distance, which will be very boring, or someone will just get out of range and  leave the battle.

---

###### Approximate Distances

|    | Bracket                     | _Appx. Feet_ | _Appx. Meters_ | Grid Sqs. |
| -- | --------------------------- | :----------: | :------------: | :-------: |
| 0. | **Close-Quarters (Melee):** |    _~0-8_    |     _~0-2_     |    1-2    |
| 1. | **Within a Few Paces:**     |    _~8-30_   |     _~2-9_     |    2-6    |
| 2. | **Nearby:**                 |   _~30-100_  |     _~9-30_    |    6-20   |
| 3. | **Far Away:**               |  _~100-300_  |    _~30-90_    |   20-60   |
| 4. | **Remote:**                 |    _>300_    |      _>90_     |    >60    |

#que Grid square equivalents are also provided here for those that _do_ prefer to use visual aids, tile maps, and figurines.

---

### Poise

Poise represents _your confidence in your armor or skill at dodging attacks, combined with your relative positioning, the weather, visibility, and cover usage_. First, let the [[Facilitator|FC]] describe the battlefield, the combatants, and any important objects in your nearby surroundings.

**Then calculate your Poise as follows:**

###### `roundup((highest(Acrobat, Armor+Helm) + 0-3)/ 2) + Shield`

-   Start with the highest of:
    -   Your **[[Acrobat]]  level**
    -   Your **Armor + Helm dice**
        -   (ie. usually based on craftsmanship, materials, and weight)
-   Add +1 _if you're on unstable, icy, or sloped terrain, or if fighting on a boat?_
-   Add +1 _if you're fighting in darkness, low visibility, or if fighting in bad weather?_
-   Add +1 _if there's lots of cover nearby, such as trees, rocks, pillars, crates, or the corners of buildings?_
-   Divide the total by 2 and round up!
-   Lastly, add _your shield dice_.

**Poise is the base difficulty of using most offensive moves against you**, and so you will need to quote this number to other players frequently. Write it down on your [[Character Sheets|character sheet]], or somewhere easy to see. Poise is also _rolled_ as part of your initial [[#Stamina|Stamina calculation]].

Poise only gets recalculated if you [[Disarm|drop]] or [[#Optional Shields Shall be Shattered|shatter]] your shield or if the environment you're fighting in changes drastically.

#imp #firearm and #flexible weapons will ignore the Poise added by shields.

#### Alternative Poise Jobs?

If you're mounted, riding a vehicle, or flying then you must instead use your [[Rider]], [[Driver]], or [[Pilot]] level, respectively, instead of [[Acrobat]]. You may also add a final bonus from your ride's _barding dice_ instead of your shield.

### Stamina

Stamina represents _the strength of your morale and spatial awareness or your sense of tactics and general disposition for violence, combined with your reaction speed relative to the other combatants_. Stamina does three main things during a fight:

-   **It decides _the turn order_ for all combatants, from highest to lowest, which you can track using a grid of numbers and a token that represents your character. **
-   **It is the amount of [[Momentum]] that is needed for an opponent to try to _pacify you with no major penalties_**.
-   **And, if you hit zero Stamina during the fight then you automatically count as being _pacified via intimidation_ and must either flee, surrender, or faint.**
-   **If you hit zero Stamina during the fight then you must either flee, surrender, or faint, and you may be automatically _pacified_ by another character.**

#### Roll Stamina!

Describe how you prepare yourself for the upcoming conflict, and thus which job you'll be using. If multiple reasons apply at once, then just choose the one you'd prefer to roll:

-   **[[Guard]] + [[#Poise|Poise]]:** _You are being ambushed, you're starting the fight up close, you're defending a strategic location, or this is a duel._
-   **[[Skirmisher]] + [[#Poise|Poise]]:** _You are initiating an ambush, you're starting the fight at a distance, you're attacking a strategic location, or this is a duel._

This roll works a lot more like a [[Checks|Check]] roll, in that **you're just looking to count successes here**, but you cannot [[KISSing|KISS]] these dice, and there's no inherent difficulty or consequences.

#que **The roll should always be made with your [[Grit]] rank**, unless you aren't using that [[Capabilities|capability]] in your campaign.

#### Base Stamina

**The successes from the job roll above are added to a base Stamina score** — which depends on your character [[Tier|tier]] and the number of other combatants, using the table below — to give you a total Stamina. _The highest possible total Stamina is 60_.

The number of combatants also determines roughly how long each round is, in-game. Though the mechanical effect of this is minimal, it may help you to describe your movements and actions, and to get a sense of scale:

| № of Combatants | Ordinary Tier | Heroic Tier | Legendary Tier | Mythic Tier | _Appx. Round Duration_ |
| --------------: | :-----------: | :---------: | :------------: | :---------: | ---------------------: |
|           **2** |       15      |      20     |       25       |      30     |               _~5 sec_ |
|         **3-4** |       20      |      25     |       30       |      35     |              _~10 sec_ |
|         **5-7** |       25      |      30     |       35       |      40     |              _~20 sec_ |
|        **8-11** |       30      |      35     |       40       |      45     |              _~40 sec_ |
|        **≥ 12** |       35      |      40     |       45       |      50     |              _~80 sec_ |

#que [[Non-player Characters|NPCs]] usually use a pre-set Poise and Stamina score, but it may be rolled if the [[Facilitator|FC]] wishes.

#### Ebb and Flow

The center of a battle is always moving, shifting across the terrain as small victories and minor losses blend together. This natural movement of combatants is accommodated into the positioning brackets, so that most characters involved a martial combat will always be within a few paces of one another.

As such, **whenever you use an offensive move with a melee weapon, you can automatically move from within a few paces to the close-quarters of your target**, as a free action, if you need to.

#que 'Offensive move' means [[Assault]], [[Spur]], [[Flank]], and [[Pacify]].

![[Momentum]]

### Stances

**At the start of each round, each standing combatant must choose and announce which 'stance' they enter.**

The announcement of your stance can just be verbal, if you like, or you can use slips of paper and write your stance on it and then all reveal your writings at the same time.

Your stance determines _which ability you should roll with to add to the [[Momentum]] this round_, and which [[#Moves|moves]] you can choose from this turn:

| **Aggressive Stance**                                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _This is pushing forward. You are attacking quickly and boldly, but also leaving yourself open to be flanked or outmaneuvered if there are other combatants around._ |
| _**Momentum:**_ +[[Swiftness]] check successes                                                                                                                       |
| _**Moves:**_  [[Assault]] ∥ [[Interact]] ∥ [[Pacify]] ∥ [[Spur]]                                                                                                     |

| **Counteractive Stance**                                                                                                                                          |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _This is holding the line. You are attacking occasionally, when you see a good opportunity, but you are otherwise keeping your guard up and trying to stay safe_. |
| _**Momentum:**_ +[[Finesse]] check successes                                                                                                                      |
| _**Moves:**_ [[Flank]] ∥ [[Interact]] ∥ [[Spur]] ∥ [[Rally]]                                                                                                      |

| **Defensive Stance**                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| _This is pulling backward. You are mostly defending yourself, using every dodge, parry, and block in your repertoire, while trying to catch your breath or do something else._ |
| _**Momentum:**_ +[[Endurance]] check successes                                                                                                                                 |
| _**Moves:**_ [[Interact]] ∥ [[Rally]] ∥  [[Reposition]] ∥ [[Treat]]                                                                                                            |

**In order to win a battle, proper use of attacks, feints, and blocks are necessary.**

> #nb
> The stance you choose each round should also depend on how you describe your character's actions, but don't worry too much if your descriptions don't match up exactly with your actions, your intentions are more important here.

#### Prone

Some attacks can knock you prone, which is a very vulnerable position to be in. We can present being prone like a stance, but it doesn't add any Momentum and your only real option is to spend your turn getting up:

| **Knocked Prone**                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _You have fallen prone or just woken up from unconsciousness. You are lying on the ground, and are vulnerable to attacks from all angles. You need to get back up as soon as possible._ |
| _**Momentum:**_ +0                                                                                                                                                                      |
| _**Moves:**_ [[#Interact]]                                                                                                                                                              |

#que In other words, being knocked prone means **you effectively lose your next turn**, unless you receive a lucky [[#Exploits|exploit]] before it starts.

#### Changing Stance

Everyone has to declare their stance at the start of the round, but you may occasionally find that circumstances have changed by the time it gets to your turn. Therefore:

-   **You _may_ change your stance to a different one on your turn, but the move you then use will suffer a +1 difficulty factor to any rolls as a result**.
-   **Alternatively:** You may get the opportunity to use the 'Change Stance' [[#Exploits|exploit]] before your turn starts, in which case no such penalty is applied.

### Turn Order

**Start with the character who currently has the _highest_ Stamina, and progress the turn order down to the _lowest_**. A turn consists of: Rolling momentum, [[#Combat Moves List|choosing a move]], performing that move, and squeezing in any [[#Free Actions|free actions]] if you want.

#que You can only act outside of your turn if you're given the opportunity to use an [[#Exploits|exploit]] by another character.

**Once every combatant has had a chance to act, a 'round' is said to have passed**.

-   If two or more characters _on the same team_ all have their turns one-after-another, then **they may reorder themselves at the start of the round**, swapping they're Stamina scores as they please.
-   If two or more characters _on opposing teams_ have the same Stamina then the one with the **highest Poise goes first**. (If these are also the same then the one who rolls the highest Momentum goes first).

At the end of each round, if a character's Stamina has raised or lowered for any reason, then they will move up or down the turn order, respectively. To make sure that no one accidentally goes twice or has their turn skipped, **only apply Stamina changes at the end of each round**.

#imp Each player need only track how much their own Stamina will change and _then tell the FC at the end of that round_, so their position on the momentum grid can be updated.

#### No Stamina

If you're reduced to zero Stamina at the end of a round then you will collapse from exhaustion, or will be paralyzed with fear, and are _effectively treated as an unconscious combatant_. Unconscious combatants count as being [[#Prone|prone]], except _they can't use any moves_, and they may be automatically pacified.

#que Using the [[Pacify]] move on a character with zero Stamina will automatically succeed without need for a roll, unless you are trying to kill them (in which case make a [[Grit]] check).

### Martial Actions

There are three types of action a character can perform in combat each round: **[[#Moves]]**, **[[#Free Actions]]**, and **[[#Exploits]]**.

It is best to describe your actions first — according to your stance — then choose the move and job that best match what you said. You can also do it in reverse if you prefer though: Choosing the job and move first, and the describing how your character acts to get there.

#### Moves

Moves are the _main actions_ available to you each [[#Turn Order|turn]], determined by your current [[#Stance Choice|stance]], and almost all moves require a job roll to be executed successfully (similar to a [[Tasks|Task]] roll but with all the details already worked out for you).

**There are eight moves in total, which can be grouped into two categories, or four pairs:**

|     Offense |  ∥  | Utility        |
| ----------: | :-: | -------------- |
| [[Assault]] |  —  | [[Treat]]      |
|    [[Spur]] |  —  | [[Rally]]      |
|   [[Flank]] |  —  | [[Reposition]] |
|  [[Pacify]] |  —  | [[Interact]]   |

**Offensive** moves tend to either damage your opponent's Stamina or inflict [[Stress]], and benefit from the +MD, whereas **Utility** moves tend to either repair that damage or let you change positions.

-   Each move can only be performed if you're in the right [[#Stance Choice|stance]] to use it.
-   Most moves require a particular [[Jobs|job]] or a choice of jobs to be used properly.
    -   When you see the double-bar symbol ∥ it means 'or'. _Choose one._
-   The bonuses and difficulties of the roll are all worked out as you read down the move, and should be fairly self-explanatory.
    -   Though some moves also require the right kinds of [[Gear Examples List#Weapons|weapons]] to get the most benefit from them.
-   _You **may** these [[KISSing|KISS]] move rolls, but remember to keep it short and sweet._

#que See the [[#Combat Moves List]] below to read each move separately, or print off the [[move cards]] from the resources chapter.

#### Free Actions

Every combatant can only attempt to use one move per round, but they may also take any of the following _free actions_ on their turn:

-   **Yell** — Shout out at the top of your lungs. _Single words or easy phrases only_.
    -   Requires an [[Endurance]] check if you need others to hear you over the noise of battle.
-   **Look** — Briefly take in your surroundings: Ask a simple question to your [[Facilitator|FC]] about the battle, such as the location and proximity of anything important in the scenery, or the positions of your enemies relative to you or your allies.
    -   Requires a [[Wits]] check if the thing you're looking for is hard to see.
-   **Drop** — Let go of something you're holding, like a weapon or another object, or an opponent you've grappled to the ground, or drop your concentration on a spell, or drop yourself [[#Prone|prone]].

#### Exploits

When a move says _“your opponent may exploit you”_ as a failure consequence — which most offensive moves say, for example — this means that your target may choose to take one following responses (as an immediate free action, also called a 'reaction'):

-   **Beat Aside:** The target beats your attack to one side and leaves you off-guard and staggered, counting as a hindrance (_+1 difficulty factor_) to your next move roll (_which can stack with other penalties_).
-   **Break Away:** The target may _move one distance bracket away_ from you, without incurring any penalties or exploits from other combatants.
-   **Change Stance:** If they haven't had their turn yet, the target may _change to a different stance_ from the one they chose at the start of the round, without incurring any penalties to their next move.
-   **Shake Off:** If the target is staggered, hesitating, or otherwise hindered, they may shake it off and _remove a penalty or negative status effect_ that's afflicting them. (Or if they are prone, they may immediately stand up).
-   **Raise the Stakes:** The target may may raise the Momentum of the battle for everyone by the margin of failure on your roll against them. They should describe what they do or say in response to you, in proportion to your failure, which raises the tension for everyone.

### Combat Moves List

#imp Instead of tracking your failures during combat, which would slow down the game's pace, _[[#Ending a Fight|at the end of a conflict]]_ **you earn _[[Earning Experience|exp]]_ equal any [[Lots]] spent plus the MD bonus that the fight finished on**, and you must distribute those points _relatively evenly_ among all the jobs you rolled with during the battle.

![[Assault]]

![[Treat]]

![[Spur]]

![[Rally]]

![[Flank]]

![[Reposition]]

![[Pacify]]

![[Interact]]

### Ending a Fight

#unfinished

#### _Optional:_ Shields Shall be Shattered

When you are using a shield — that is, a _proper_ #shield, not just a weapon with a #hand-guard — and a [[Kill|kill]] move is successfully used against you, **your shield will shatter and negate the killing blow**, and you will take a point a point of stress instead (ie. [[Pain|pain]] if you're in aggressive stance, [[Shock|shock]] if you're in counteractive stance, or [[Fatigue|fatigue]] if you're in defensive stance). You lose the protective benefit of your shield, unless you find another, but at least you're still alive!

However, if the weapon being used against you has the #great tag, _and your shield doesn't_, then your shield still shatters but the blow isn't negated. That is, **only a #great shield can negate a killing blow from a #great weapon**.

#imp Similarly, only #magic shields can be shattered against #magic attacks.

#que Therefore, if you're fighting a dual with shields but don't want it to be deadly, you can fight until the first shield is shattered (or the first to three) and then declare the victor.

### Shooting into the Fray

#unfinished
