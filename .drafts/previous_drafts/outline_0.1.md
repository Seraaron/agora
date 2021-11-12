<!-- parts of the markdown files are commented in FULL CAPS for ease of Ctrl+F searching -->
# game structure stuff / core philosophies:
- section titles are shorthands for the rules themselves
  - general game are in **bold**, but aren't capitalized
    - specific game terms are Capitalized
      - the only exception is **knacks**, which aren't capitalized but are *italicized*
    - some terms are also shortened, with most vowels removed and using a $spcl$ $fnt$ to make them easier to pick out
      - this font is also used for mathematical expressions and calculations
    - `monospace font` is used for changable game figures, indicating when to roll dice and what modifiers to add
      - small case `d` is used for Checks (roll-above) and rolling on random tables
      - upper case `D` is used for Tasks (pool-based successes) and only refers to D10s
- speak to the reader: always use second person pronoun, 'you'
  - let context determine whether 'you' means the GM, a player, or their character
- session types & segments
  - normal sessions
    - preamble
    - (game)play
    - meta(game)
    - debriefing
  - downtime sessions
    - used to pass in-game time quickly (weeks, months, years)
    - spend lots to have brief role-play scenes and earn $exp$ in a related skill
  - solo sessions
  - development sessions
    - session 0
    - character creation / development
      - allows for re-jigging your character, changing some $caps$ or advancing to a new tier 
    - worldbuilding
  - anyone can ask for any kind of session in advance, but the assumed default is a normal session
- scenes, rounds, turns, & beats
  - turns start with the GM and then always go clockwise
    - (or in the order that the players turned up to the session)
  - once a round passes where noone has anything else to add (or skips their turn) then the scene ends
  - any player (including the GM) can also use [script change tools](https://briebeau.com/thoughty/script-change/) to pause, speedup, slowdown, or even rewind play
- two types of roll:
  - checks (simple verbs / actions)
    - straight-forward, quick and dirty, binary outcomes
    - target number based success critea, roll with `1d20 + Y + Z`
      - target = action type (i.e. 1 - 4) $\times$ 5 + circumstancial penalties (up to max target 30)
        - OR: target = opposing faculty score $\times$ 3 + circumstancial penalties
      - result = `1d20` die roll + appropriate faculty score (i.e. 1 - 9) `Y` + appropriate swatch choice `Z`
        - count a natural 20 as an auto-pass
        - and a natural 1 as an auto-fail
      - check success = get result equal to or higher than target
        - margin of success or failure does not matter
        - and there is no notion of a 'critial'
  - tasks (complex verbs / skills)
    - complicated, slow but clean, potential for marginal outcomes
    - pool based success criterions, roll with `XD10 =< Y`
      - difficulty = action type (i.e. 1 - 4) + circumstancial penalties (up to max difficulty 10)
        - OR: difficulty = opposing faculty score + circumstancial penalties
      - pool size `X` = skill level + circumstancial / staked advantages + help
      - total successes = count all rolls under given faculty score `Y` appropriate to the task
        - count all 0's rolled as successes
        - all 0's count as double-successes by spending a meta currency (tracked with beans)
      - task success = get total successes equal to or greater than the difficulty
        - margin of success or failure may matter in certain instances
          - meeting or exceeding the difficulty by *double* may result in a 'critial success'
          - getting successes equal to *half* the difficulty or less may result in a 'critial failure'
  - this means players only need a handful of D10's, a d20 (and some beans for trackers) to play
  - so the proprietary elements / barriers to entry are kept low
    - would be nice to re-work the system with D6's, since everyone has access to D6's (or can make them)
    - but I think it's easier to think in basic chance-increments of 5 or 10%, rather than 16.66%
- it's also easier to do addition than it is to subtract
  - bonuses should always add to your dice or roll
  - penalties should always add to the difficulty
    - only *execptional* powers / attributes, should break these heuristics
    - (as they are the exceptions)
- similarly, division is hard, so no all numbers used should be integers
  - if a calculation results in a fractional amount then *always round down*
- always set stakes, and be clear about failure conditions
  - set narrative stakes
  - failing better (not always failing forward)
  - players can offer potential failure solutions
    - and can narrate both their successes and their failings, if they want to
  - avoid re-rolling without changing the stakes
- **GM** stands for 'game moderator', or maybe it should be D/M for 'director / manager'? (referee is also acceptable)
  - *all* players are expected to adjudicate the game rules, not just the GM
    - expl
  - the GM is not necessarily in a position of power over the other players
    - it should be possible to play without a GM, but this will not be covered
- the **jury** refers to all the other players at the table except you
  - the jury is a relative term, each player's jury is different
    - and the GM's jury is all the other players
  - rules can be changed, broken, or removed by *any* player (including the GM) at any time
    - but only with permission from that player's jury
- let players direct/frame scenes!
  - maybe something that regenerates ego?
- the GM never rolls (or at least never performs tasks)
  - contested tasks mostly work against faculty or stat scores
  - defending yourself is a skill
- all mechanics are abstract representations of reality
- (nearly) everything is modular
  - core game engine [venus] will be `CC BY 4.0` (free cultural work)
  - everything else [evening_star] will be `CC0` (public domain)
    - this means anyone who wants to make content for the game can do so, and sell it if they want
    - but they must reference the venus engine in some way to bring a bit of unity to all projects
  - though both will be `All Rights Reserved` until the first major release
- everything is relative
  - time, distances, difficulties
- common sense vs. suspension of disbelief
- no half measures, no sitting in the middle of the road
  - when categorising weapons and armour and such, there is no 'medium' option, all ranks are from 1 to 4 (or 0 to 5):
    - weights are: very light, light, heavy, or very heavy
    - lengths are: very short, short, long, or very long
    - ranges are: very near, near, far, or very far
    - actions are: very simple, simple, complex, or very complex
    - durations are: very fast, fast, slow, or very slow
    - visibilities are: very clear, clear, obscure, or very obscure
    - little effort, some effort, great effort, or monumental effort
    - ages are: infant, young, adult, aged, elder, senile
      - (requires jury permission to play an infant or senile character, since they are both so vulnerable)

## design goals
- make a game that **I** want to play
  - versatile and scalable to most settings / situations (but especially my own worldbuilding project)
    - will require frontloading the character creation process
    - but then the crunch for actual gameplay should be relatively low
  - focus on different types of conflict resolution or presenting actions with interesting choices resulting in memorable storytelling / narrative experiences
  - modular subsystems
    - modular character creation sections
    - even the tasks system may be modular (play test this first!)
- avoid making direct references to other ttrpg games and / or buzzwords
  - or at least the proprietary ones
  - linking to other creative commons resources is probably fine
- play-test often, every two weeks if possible
  - and get the first public release out within a month or two
- stream parts of the creation process at least once per week
  - (and make the VODs creative commons too)

---

# minimum viable product / first play-test version
- pre-made characters for the players, consisting of
  - name, circumstances, swatch choices
  - age, faculty scores, attributes
  - VINPCs and essential gear?
  - stats
- checks *only*, no tasks
- a roleplay heavy scenario
  - since the basic system, using only checks, is very similar to most existing OGL RPGs this should just end up playing like an 'OSR' game
  - hence, it should handle dungeon crawling just fine, and I don't need to test that
  - so by focusing on a roleplay / action-oriented test session we'll get to see how granular checks are by themselves and whether tasks are even necessary

---

# character creation stuff
- **tier**
  - tier sets the approximate 'power level' for play
    - bronze: no faculty allowed over 4, bonus faculty $pts$ = 0, max unique swatches = 5, average difficulty range 1-3
    - silver: no faculty allowed over 7, bonus faculty $pts$ = 8, max unique swatches = 7, average difficulty range 4-6
    - gold: no faculty allowed over 9, bonus faculty $pts$ = 18, max unique swatches = 11, average difficulty range 7-9
  - the tiers are just shorthands and should not be taken absolutely
  - they are there to set expectations for the players and to make decision making easier for the GM
    - which also makes the moments when the GM decides to break out a higher-tiered monster or difficulty more interesting and noteworthy

- **circumstances**
  - immutable (can't typically be changed after character creation)
    - e.g. species, heritage, ethnicity, culture, upbringing, etc.
  - variable (can change over time, during development sessions, or after certain choices or realizations made in play)
    - e.g. religion, community, class, gender, size, age, etc.
- *swatches*
  - swatches represent archtypical roles that your character has fulfilled at various points throughout their life
    - be they occupations, periods of studentship, service, or incarceration, snippets of your upbringing, or the 
    - they are generic, but personalized; and peice by peice they build up the tapestry that implicitly tell the story of your character's life so far
  - swatches affect what skills, qualities, and knacks you can aquire and advance during character creation
    - and how many $caps$ (points) you have to spend on those things
  - swatches have a title, followed by a list of potential skills, qualities, and knacks that you can take
    - all swatches have at most 9 of these
      - all swatches without requirements offer precisely 3 skills, 3 knacks, and 3 qualities
      - swatches with requirements mix it up a bit more, but still stick to the 9 total limit
  - swatches also list items and equipment that you would likely own as a result of taking them
  - in general, the more swatches you take the older your character will be when the game starts
    - (we will use human years for this calculation, so if you are playing as a different species then make an appropriate conversion)
    - 5 plus the number of unique swatches you've taken multiplied by 3 is your character's minimum age
    - then roll `1d10` for each swatch you've taken more than once and add as many or as few of these rolled numbers to your final age as you wish
      - why? a little bit of randomness like this can produce some interesting choices
      - however, if this randomness gives you an age that you are not comfortable playing as, then you can either re-roll, or just pick whatever you feel is an appropriate age with permission from your jury
    - you *can* play a character with no swatches, but they will likely be very young and will have to learn every thing from scratch
- *age*
  - age affects your faculty score spread
    - younger characters tend to have higher physical faculty scores
    - older characters tend to have higher mental faculty scores
    - `TEMP:`
    - Maybe replace age number with age brackets {very young, young, old, very old}

| **Age Range** | Mental $:MF_{pts}$ | Physical $:PF_{pts}$ | *Total* |
| :-----------: | :-----------: | :-------------: | :-----: |
|   **0 — 4**   |       3       |        4        |   *7*   |
|  **5 — 11**   |       4       |        5        |   *9*   |
|  **12 — 15**  |       4       |        7        |  *11*   |
|  **16 — 18**  |       5       |        9        |  *14*   |
|  **19 — 21**  |       7       |       10        |  *17*   |
|  **22 — 24**  |       8       |       11        |  *19*   |
|  **25 — 29**  |      10       |       10        |  *20*   |
|  **30 — 35**  |      11       |        9        |  *20*   |
|  **36 — 41**  |      11       |        8        |  *19*   |
|  **42 — 49**  |      11       |        7        |  *18*   |
|  **50 — 57**  |      10       |        7        |  *17*   |
|  **58 — 66**  |       9       |        6        |  *15*   |
|  **67 — 76**  |       9       |        5        |  *14*   |
|  **77 — 87**  |       8       |        5        |  *13*   |
|  **88 — 99**  |       7       |        4        |  *11*   |
| **100 — XX**  |       6       |        3        |   *9*   |
```
Notes:
  - at SILVER tier: add +4 points to each faculty pool (for a total of +8 points)
  - and at GOLD tier: add another +3 points to each faculty pool (for a total of +14 points)
```
- **faculty scores**
  - $MF$ [mental faculties]
    - Appeal (App) — mental grace, charisma, personal charm, social understanding, and emotional senses
    - Resolve (Res) — mental resilience, wisdom, determination, memory retention, and temporal senses
    - Wits (Wit) — mental power, intelligence, logical reasoning, shrewdness, instinct, and spatial senses
  - $PF$ [physical faculties]
    - Endurance (End) — physical resilience, constitution, vigour, and long-distance movement upkeep
    - Finesse (Fin) — physical grace, dexterity, coordination, style, and balanced movements
    - Swiftness (Swi) — physical power, strength, fitness, and short-distance movement speed
  - scores all start at 1 [▮▯▯ ▯▯▯ ▯▯▯] and range up to 9 [▮▮▮ ▮▮▮ ▮▮▮]
    - increase scores from 1 by spending the $MF$ and $PF$ $pts$ from each pool listed above
    - use a pencil to fill in the boxes as they increase
      - because after character creation faculty scores can only go up (or down) during development sessions
      - this partly depends on your new age (if a lot of time has passed), but is mostly voted on by your jury
  - you use your faculties to perform checks (simple verbs)
    - roll `1d20+X` where X is your faculty score
    - try to meet or exceed the target set by the GM (3 $\times$ the difficulty)
    - checks have binary 'pass' or 'fail' criterions
  - your faculty score also sets the base difficulty when certain checks and tasks are performed against you
    - when this happens it's important to be clear about the failure conditions, and make sure the other player agrees to be tested against
  
- **characteristic attribution points** $(caps)$
  - each new swatch taken grants only +3 $caps$ the first time (to encourage diversification)
  - but each swatch taken more than once grants +7 $caps$ each time (to encourage specialisation)
    - e.g. taking Soldier $\times$ 3 grants a total of 17 $caps$
  - $caps$ are used to buy skill levels, knacks, and qualities

- **skills**
  - you use skills when performing tasks (complex verbs)
    - roll `XD10` where X is equal to your skill level plus any modifers and advantages that you've advocated for in the negotiation phase:
      - if more than one skill seems to be related and applicable to the task then use the lowest one, and grant a bonus die for the task
      - similarly if an ally wants to help, then they must use a related skill, and the lowest levelled one between you rolls and gets a bonus dice from the other
        - each character can only help with one skill at a time
        - when helping, if the task fails, the helpers each get an experience point in the skill the helped with
      - between related skills and help, you may only gain a maximum total of `+3D`
    - each die must roll equal to or below the faculty tie for the given task to count as a success
    - if total successes meet or exceed the difficulty then the task is completed successfully
    - margin or success or failure may matter, depending on circumstances
  - they are tracked and levelled individually by counting total failed tasks over time
    - twice the current level is the number of failed tasks needed to advance a skill level
  - each skill is tied to two faculties, resulting in 15 possible combinations:
    - App$/$Res, App$/$Wit, App$/$End, App$/$Fin, App$/$Swi, Res$/$Wit, Res$/$End, Res$/$Fin, Res$/$Swi, Wit$/$End, Wit$/$Fin, Wit$/$Swi, End$/$Fin, End$/$Swi, Fin$/$Swi
      - (for the sake of consistency, each tie should always be ordered alphabetically)
        - so you should never write Res$/$App, for example
        - but if you do by mistake then it's okay, because it just means the same thing as App$/$Res
    - plus some skills may have special exemptions related to their ties, or may have unique uses with certain stats, these have a superscript star symbol ($\star$) next to their listed ties and a note explaining the special case in the skill's description / effects
    - the tie's score is the faculty value to roll under when performing a task with the dice of that skill
      - which one you roll against depends on the circumstances of the task / the way you use the skill
  - bought with $caps$
    - if the skill is listed in any of your swatches then it costs 1 $cap$ per level up to level 5, then 2 $caps$ per level
    - if the skill is not listed, then you learned it by yourself, and so costs 2 $caps$ per level and can't be raised higher than level 5 during character creation 

- **qualities** (adjectives)
  - qualities are either Aesthetic $(As)$, Potent $(Pt)$, or Limiting $(Lm)$
  - (ie. quirks, flaws, features, powers, etc.)
    - aesthetic qualities don't grant direct bonuses to tasks, but they can award lots at the end of each session for representing them well during play
      - cost 1 $caps$ if they were listed in your swatches, or 2 $caps$ otherwise
    - potent qualities grant magical powers or special talents to use, allowing your character to do more than they would be able to without them
      - potent qualities are explicitly allowed to break the normal rules of play
      - cost 1 $caps$ if they were listed in your swatches, or 4 $caps$ otherwise
      - some potent qualities can be bought first as an aesthetic quality and then upgraded to potent
        - these only cost +1 $caps$ to upgrade
    - limiting qualities are typically health conditions (injuries, disfaculties, or diseases), but may be other characteristic factors, that increase the difficulty of certain tasks and checks for your character
      - taking a limiting quality from your swatch list grants you 2 $caps$, otherwise they only grant 1 $caps$
      - limiting qualities can eventually 'heal' to become aesthetic qualities, like scars, or be removed completely (this happens in development sessions)
  - some qualities are innate and given out for free depending on your circumstances and swatch choices (marked by a $*$ in swatch descriptions)

- **knacks** (nouns)
  - knacks are speciality interests, natural talents, reputations, or quirks that grant special knowledge, access to new locations, or other special privilages
    - they are *not* used directly with any tasks or checks
      - to use them, you must draw on the knack for descriptive or narrative inspiration
      - then the GM will respond in kind if they have information to give you that your character *should already know*, based on their knacks
      - this can esablish a new (i.e. previously unknown to the jury) fact about yourself, the world, or the current situation
        - both you and the GM can contribute to this information, collaborating until you settle on something that you both like and which makes sense in context
        - but the GM is the final arbiter of 'the whole truth' in this instance
    - however, your use of a knack may enable you to make a roll that you would not normally be able to make
      - you don't get any inherent bonuses because of the knack, just a chance where any other character would not have one
  - bought with $caps$:
    - 1 $cap$ per knack if listed in your swatches
    - or 3 $caps$ if not listed

- **kith & kin / VINPCs** (proper nouns)
  - these are 'very important non-player characters' (pronounced vin-pee-see) that you have designated as being very important your character or the story
  - you are limited to a maximum of 3 VINPCs in total, regardless of your tier
    - only the GM may raise or lower this limit, since they are the one that will most-likey have to design and portray them all
    - therefore, you must also discuss each one in detail with your GM
    - if you have no ideas about which characters may be important to you, don't worry
      - you can ask for an NPC you've met ingame to be designated as a VINPC during downtime or development sessions
      - similarly, a character whom you thought would be important may turn out not to be
        - it's ok to downgrade them back to being normal NPCs
  - you can also use your swatches and circumstances to guide which sorts of NPCs you are most likely have relationships with
  - VINPCs can occasionally function like knacks, in that: they can offer you advice, tell you secrets, grant you acess to special places, award you with titles or powers, and so forth
    - but you have little to no control over them, they are the GMs characters ultimately
  - they are always written in Upper-Case *Italics*

- **gear & sundry**
  - swatches list the sorts of items, equipment, & property that you would likely own as a result of taking them
    - you can add one item from this list to your sheet each time your take the same swatch
      - e.g. taking Soldier $\times$ 3 gives you 3 different items from it's list
  - the lists on the swatches are meant to be evocative, more than anything, rather than being strict accouterments 
  - as such, once you have chosen everything you want off the lists, you can also pick up any other bits and peices that you think are appropriate for your character to own (with your jury's permission)
    - how much to write in depends on play style, game themes, and personal preference
    - if playing with survival themes then it might make sense to track every penny and morsel
    - but if you're using the wealth stat then the stat itself can be used to define what you own, when it becomes relevant through play
    - as such, by default, this game has no precious metal peices, credits, or other currencies to keep track of that are spendable during character creation
      - but once the game begins, if your game needs them, then the GM's wouldbuilding will decide how much everything is worth, and how much money you own, based on your circumstances and swatch choices, and you would write them in with all your other possessions
      - this an aspect of play that's very much time-period and setting specific
      - economies are complex, so no further guidance is offered in this respect, at this time, sorry

---

- **stats** (derived faculties) [module]
  - stats function almost identically to faculties, except that:
    - they are *derived* from your character creation choices up until this point
    - they can only be used to perform checks, not tasks
      - (unless you have a special skill tied them)
      - often, failing a stat check takes a certain amount of agency away from your character for a brief time 
    - they are also completely optional / modular, and tagged based on game-themes
      - if you know your game won't contain any of those themes then you can pretty safely ignore those stats
    - however, sticking to a theme is important so that the game doesn't get diluted, so you may only choose up to 3
      - decide as a group which ones you feel would be necessary or useful for your game
      - different PCs *can* each have different stats, but only if it makes sense...
        - it's better to try to be consistent
      - since they are all derived, you can change out stats in a development session for new ones if your game theme has shifted
      - and re-derive them again if the theme shifts back
  - *Grit* (#violence, #combat, #war)
    - tolerance for injuring others and governs instinctual reactions in a fight
    - calculated by: Add Wits and Swiftness, divide by 4, + questionnaire answers
  - *Guts* (#violence, #combat, #mystery, #horror)
    - tolerance for being injured and governs how long you can keep up the fight
    - calculated by: Add Endurance and Resolve, divide by 4, + questionnaire answers
  - *Wealth* (#feudalism, #capitalism, #intrigue, #politics)
    - represents money management, investments, access to funds, etc. not for games where you want to track every penny 
      1. someone else's property; a vagrant; a fugative; an untouchable
      2. living beneath the poverty line; an indentured servant; or just down on your luck 
      3. living within your means; free but poor; living a nomadic lifestyle; or caged in comfort 
      4. starting to turn a profit; an apprentice; a student; a hustler; or a seasonal-soldier
      5. enough savings for emergencies an special occasions; a guild-member; an itinerant trader; or a mercenary
      6. full records, insurance, and regular savings; a master artisan; a residential merchant; or a professional-soldier
      7. an aristocrat living off of investments and interest, or the exploitation of others; a superintendent; a guild-master; a knight; or a criminal kingpin
      8. born into wealth and sworn to fealty; lesser nobility; a viceroy; a chancellor; or robber baron
      9. a true blue-blood; practically (or literally) royalty; greater nobility; a warlord; or the cheif executive of a merchantile empire
    - calculated by: jury decision based on circumstances, swatches, and questionnaire answers
  - *Links* (#politics, #intrigue, #factionalism, #war)
    - represents a 'social wealth' of sorts: your current contacts, faction affiliations, past associates, rivals, or lovers, and any favors still owed or contracts you've entered into with them
    - good for social games set in a single city or county, not great for world-hopping adventures (better to just use 'first-impessions' Appeal checks in that case when meeting new people)
    - calculated by: half your Appeal score + questionnaire answers
  - *Vigilance* (#exploration, #mystery, #survival, #horror, #supernatural)
    - mental resilience to abnormal events and existential dread
    - calculated by: age (in human years) since first contact with the supernatural, divide by 10, + questionnaire answers
  - *Honor* (#feudalism, #politics, #chivalry)
    - calculated by: questionnaire answers
  - *Soul* (#supernatural, #magic, )
    - calculated by: questionnaire answers
  - *Custom*
    - all of the above are just suggestions
    - if you don't like the names of some you can change them
      - the stats section of the character sheet has blank spaces so you can write-in whichever ones you need
    - or if want to make your own to suit your game themes you can do so easily
      - just think about how faculties work in relation to skills
      - make sure that the stat is something you can only perform checks with, otherwise it might be better suited to being a custom a skill
      - think of a questionnaire that can help to generate the score
  - *NPC stats*
    - npcs generally don't roll dice (or don't perform tasks, at least)
    - so the npcs need a few extra stats that player characters don't, in order to set the difficulty for opposing rolls
      - defences

- **goals, habits, & creeds** [module]
  - write about your character
  - 3 slots total — rewarded with lots
  - discuss with other players and the GM

- **lots & ego** (metacurrencies) [sub-module]
  - *lots*
  - you can have up to 10 lots at a time
    - lots spent on tasks can reroll a die of your choice
      - or make all 0s rolled count as successes twice
    - one lot can be spent per check to reroll too
    - you can earn a portion of your lots back in the debreif every session by advocating for your portrayal of your character's aesthetic qualities and reflecting their choices throughout the session expressed via goals, habits, &/or creeds 
    - lots earned during the debreif that would bring you above the maximum, 10, are converted into $exp$ to help you level up any skills of your choice
  - *ego*
  - you either have ego at any given time, or you dont
    - spending ego on a just-failed task lets you retry it as a check
    - ego can't be spent on checks
    - earn back ego from introducing your own scenes
    - you also earn ego back in the debreif automatically (in Gold tier only?)
  - you start the game with ego and a number of lots chosen by the GM, depending on the starting situation (reccomended: 3-5)

---

### levelling up skills (failure bookeeping = $exp$)
- two times the level of the skill is the number of tasks you must *fail* with that skill to level it up
  - i.e. you only learn from your mistakes
- levelling the skill happens immediately after the last task is failed (or as soon as you notice that the exp bar is filled thereafter)
- every time you level up a skill, the $exp$ slate is wiped clean for that skill
  - e.g. level 4 skill requires 8 failed tasks to become level 5, then it needs 10 new failures
- 10 is the soft level cap for all skills
  - only keep tracking exp / failures beyond level 10 if you are playing at GOLD tier and your GM allows it
    - in this case, there's technically no level cap, but once you fill the slate up again you must aquire supernatural training or utilize advanced technologies, each time, to increase the skill level by 1

#### learning new skills
- when you enter a situation where you would need to perform a task but don't have the right skill
- make a check instead with one of the associated faculties (as appropriate to the task)
- then add the unlearned skill to your sheet at level 0 with the first $exp$ checkbox checked
- mark additional $exp$ for all future checks made on behalf of that skill (regardless of success or failure)
- once the exp bar is filled completely (18 checks total):
  - the new skill immediately levels up to be the same level as your lowest known skill that shares the same ties
  - if you do not know of any other skills with those ties, then the newly learned skill only raises to level 1

#### skill list example
- skills are all doing-words: verbs, with a clarifying nouns after a comma (if required)

| Skill           | Level | $exp$ Slate                  | Ties            |
| --------------- | :---: | ---------------------------- | --------------- |
| Debate          |   3   | ☒☒ ☒☒ ☒☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Res/Wit         |
| Sew             |   5   | ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Wit         |
| Fight, swords   |   4   | ☒☒ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Swi         |
| Conjure, spells |   0   | ☒☒ ☒☒ ☒☒ ☒☒ ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % | App/End$^\star$ |
| Research        |  10   | % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | End/Wit         |

## knack examples
- knacks are all places, things, or ideas: nouns, but not proper nouns (and usually pluralized)
- they are always presented in lower-case *italics*
- since all knacks do the essentially same thing but for different fields of interest, their names should be fairly self-explanatory
  - that is, they shouldn't need descriptions unless they refer to foreign or fantastical concepts

## quality examples
- qualities are all descriptive words relating to your character: adjectives, or the adjective form of certain nouns, or a short descriptive sentence if a single word or two can't seem to encapsulate the concept
- $As:$ **Lovely Smile**
  - *description (if any)*
  - upgrade option (if any)
- $Lm:$ **Blind in one Eye**
  - *description*
  - effect `n`
    - *notes / clarifications (if any)*
  - effect `n+1`
- $Pt:$ **Chosen**
  - *description*
  - effect

---

# additional / modular gameplay features
ultimately, almost all mechanics can be abstracted into different kinds of conflicts. each kind may have it's own system of resolution
- internal conflict resolutions
  - healing / recovery
  - changing your mind
- character conflict resolutions
  - battles
  - chases
  - debates
  - duels
- environmental conflict resolutions
  - animals
  - envrionmental penalties are grouped such that you only apply the highest if multiple are applicable:
    - light / visibility levels
    - terrain stability
- supernatural conflict resolutions
  - religions
  - summoning weird things
- technological conflict resolutions
  - vehicles
- societal conflict resolutions
  - politics
  - wars