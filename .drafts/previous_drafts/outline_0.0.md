<!-- parts of the markdown files are commented in FULL CAPS for ease of Ctrl+F searching -->
# game structure stuff / core philosophies:
- section titles are shorthands for the rules themselves
  - general game are in **bold**, but aren't capitalized
    - specific game terms are Capitalized
      - the only exception is **knacks**, which aren't capitalized but are *italicized*
    - some terms are also shortened, with most vowels removed and a $spcl$ $fnt$ to make them easier to pick out
      - this font is also used for mathematical expressions and calculations
    - `monospace font` is used for changable game figures, including dice rolls and modifiers
      - small case `d` is used for Checks (roll-above) and rolling on random tables
      - upper case `D` is used for Tasks (pool-based successes) and only refers to D10s
- speak to the reader: use second person pronoun 'you'
- sessions & segments
  - normal sessions
    - preamble
    - (game)play
    - meta(game)
    - debriefing
  - downtime sessions
    - used to pass in-game time quickly (weeks, months, years)
    - spend lots to have brief role-play scenes and earn $exp$ in a related skill
  - development sessions
    - session 0
    - character creation / development
      - allows for re-jigging your character, changing some $caps$ or advancing to a new tier 
    - worldbuilding
  - solo sessions
  - anyone can ask for any kind of session in advance, but the assumed default is a normal session
- scenes, rounds, turns, & beats
  - once a round passes where noone has anything else to add (or skips their turn) then the scene ends
  - [script change tools](https://briebeau.com/thoughty/script-change/) can also speedup or slowdown play
- its generally easier to do addition than it is to subtract
  - bonuses add to your dice or roll, penalties add to the difficulty
  - very few things reduce your dice or reduce the difficulty
    - (they are the execptions, like special attributes; things that break the rules)
- always set stakes, and be clear about failure conditions
  - players can offer potential failure solutions
  - simulationism vs narrativism
  - failing better
  - avoid re-rolling without changing the stakes
- GM stands for 'game moderator', or maybe it should be D/M for 'director / manager'?
  - *all* players are expected to adjudicate the game rules, not just the GM
  - the GM is not necessarily in a position of power over the other players
    - it should be possible to play without a GM, but this will not be covered
  - rules can be changed, broken, or removed by any player (including the GM)
    - but only with permission from all the other players (including the GM)
- the GM never rolls (or at least never performs tasks)
  - contested tasks mostly work against ability or stat scores
  - defending yourself is a skill 
- everything is relative
  - time, distances, difficulties

# character creation stuff:
- **tier**
  - tier sets the approximate 'power level' for a session of play
    - bronze: max ability score = 3, max unique jobs = 5, average difficulty range 1-3
    - silver: max ability score = 6, max unique jobs = 7, average difficulty range 4-6
    - gold: max ability score = 9, max unique jobs = 11, average difficulty range 7-9
  - the tiers are just shorthands and should not be taken absolutely
  - they are there to set expectations for the players and to make decision making easier for the GM
    - which also makes the moments when the GM decides to break out a higher-tiered monster or difficulty more interesting and noteworthy
- **circumstances**
  - immutable (can't typically be changed after character creation)
    - species, heritage, ethnicity, culture, etc.
  - variable (can change over time, with character development)
    - religion, community, class, gender, etc.
- **job history & age**
  - jobs have a title, followed by a list of potential skills, knacks, and attributes, plus any other job leads or requirements
    - all jobs have at most 9 of these
      - all jobs without requirements offer precisely 3 skills, 3 knacks, and 3 attributes
      - jobs with requirements mix it up a bit more, but still stick to the 9 total limit
    - in general, the more jobs you take the older your character will be when the game starts
      - (we will use human years for this calculation, so if you are playing as a different species then make an appropriate conversion)
      - 5 plus the number of jobs you've had multiplied by 3 is your character's minimum age
        - each time you take the same job again add +1 to your minimum age
      - then roll `2d10` and add none, one, or both of these rolled numbers to your final age
        - why? a little bit of randomness like this can produce some interesting choices
        - however, if this randomness gives you an age that you are (or another player is) not comfortable with playing, then you can either re-roll or just pick whatever you feel is an appropriate age
      - you *can* play a character with no job history, but they will likely be very young and will have to learn every new skill from scratch
  - age affects your ability score spread
    - younger characters tend to have higher physical ability scores
    - older characters tend to have higher mental ability scores
- **abilitiy scores**
  - [physical] — Endurance (con), Finesse (dex), Swiftness (str)
  - [mental] — Appeal (cha), Resolve (wis), Wits (int)
  - scores range from 1 [▮▯▯ ▯▯▯ ▯▯▯] to 9 [▮▮▮ ▮▮▮ ▮▮▮]
    - ability scores can only go up or down during development sessions, and are voted on
  - the total number of ability points allowed per character at character creation *must be a prime number*, to force an uneven distribution
  - your ability score also sets the base difficulty when checks and tasks are performed against you
    - when this happens it's important to be clear about the failure conditions, and make sure the other player agrees to be tested against
- **characteristic assignment points** $(caps)$
  - base $caps$ depends on age and circumstances
  - each new job taken grants only +3 $caps$ the first time (to encourage diversification)
  - but each job taken more than once grants +7 $caps$ each time (to encourage specialisation)
    - e.g. taking "Soldier $\times 3$" grants a total of 17 $caps$
  - $caps$ are used to buy skills (verbs), knacks (nouns), and attributes (adjectives)
- **skills** (verbs)
  - skills give you the majority of the dice for a given task, equal to the level of that skill
  - they are tracked and levelled individually by counting total failed tasks over time
      - if more than one skill seems to be related and applicable to the task then use the lowest one, and grant a bonus die for the task
      - similarly if an ally wants to help, then they must use a related skill, and the lowest levelled one between you rolls and gets a bonus dice from the other
        - each character can only help with one skill at a time
        - when helping, if the task fails, the helpers each get an experience point in the skill the helped with
      - between related skills and help, you may only gain a maximum total of `+3D`
  - each skill is tied to two abilities, resulting in 15 possible combinations:
      - App/Res, App/Wit, App/End, App/Fin, App/Swi, Res/Wit, Res/End, Res/Fin, Res/Swi, Wit/End, Wit/Fin, Wit/Swi, End/Fin, End/Swi, or Fin/Swi
      - the tie's score is the value to roll under when performing a task with the dice of that skill
        - which one you roll against depends on the circumstances of the task / the way you use the skill
  - bought with $caps$
    - if the skill is listed in any of your jobs then it costs 1 $cap$ per level up to level 5, then 2 $caps$ per level
    - if the skill is not listed, then you learned it by yourself, and so costs 2 $caps$ per level and can't be raised higher than level 5 during character creation 
- **knacks** (nouns)
  - knacks are speciality interests, natural talents, reputations, or quirks that reduce the difficulty of checks and tasks by 1 during the negotiaion phase, they are not levelled
    - to do this, you must draw on the knack for descriptive or narrative inspiration
    - either using it to esablish a new (prviously unknown) fact about the yourself, the world or the current situation
    - or using it to perform a 'stunt', so long as it still leaves failure of the main task an open possibility
  - bought with $caps$: 1 point per knack, but must be listed in your jobs
- **attributes** (adjectives)
  - attributes are either Aesthetic $(As)$, Potent $(Pt)$, or Limiting $(Lm)$
  - (ie. quirks, flaws, features, powers, etc.)
    - aesthetic attributes don't grant direct bonuses to tasks, but they can award lots at the end of each session for representing them well during play
      - cost 1 $caps$ if they were listed in your jobs, or 2 $caps$ otherwise
    - potent attributes grant magical powers or special talents to use, allowing your character to do more than they would be able to without them
      - potent attributes are explicitly allowed to break the normal rules of play
      - cost 1 $caps$ if they were listed in your jobs, or 4 $caps$ otherwise
      - some potent attributes can be bought first as an aesthetic attribute and then upgraded to potent
        - these only cost +1 $caps$ to upgrade
    - limiting attributes are typically health conditions (injuries, disabilities, or diseases), but may be other characteristic factors, that increase the difficulty of certain tasks and checks for your character
      - taking a limiting attribute from your job list grants you 2 $caps$, otherwise they only grant 1 $caps$
      - limiting attributes can eventually 'heal' to become aesthetic attributes, like scars, or be removed completely (this happens in development sessions)
  - some attributes are innate and given out for free depending on your circumstances and job choices (marked by a $*$ in job descriptions)
- **VINPCs** (very important non-player characters)
  - these are special NPCs that you have designated being very important your character or the story
  - limited to a maximum of 3 in total, since the GM must portray them
    - you must discuss each in detail with your GM
    - if you have no idea which characters may be important to you, don't worry
      - you can ask for an NPC you've met ingame to be designated as a VINPC during- development sessions
      - similarly, a character whom you thought would be important may turn out not to be
        - it's ok to downgrade them back to being normal NPCs
  - use job history and circumstances to guide which sorts of NPCs you are most likely have relationships with
- **stats** (derived abilities)
  - stats function almost identically to abilities, except that:
    - they are *derived* from your character creation choices up until this point
    - they can only be used to perform checks, not tasks
      - often, failing a stat check takes a certain amount of agency away from your character for a brief time 
    - they are also completely optional / modular, and tagged based on game-themes
    - if you know your game won't contain any of those themes then you can pretty safely ignore those stats
    - however, sticking to a theme is important, so you may only choose up to 3
      - decide as a group which ones you feel would be necessary or useful for your game
      - different PCs *can* each have different stats, but only if it makes sense...
        - it's better to try to be consistent
      - since they are all derived, you can change out stats in a development session for new ones if your game theme has shifted
      - or re-derive them again when the theme shifts back
  - Grit (#violence, #combat, #war)
      - tolerance for injuring others and governs instinctual reactions in a fight
  - Guts (#violence, #combat, #mystery, #horror)
      - tolerance for being injured and governs how long you can keep up the fight
  - Wealth (#feudalism, #capitalism, #intrigue, #politics)
    1. someone else's property; a vagrant; a fugative; an untouchable
    2. living beneath the poverty line; an indentured servant; or just down on your luck 
    3. living within your means; free but poor; living a nomadic lifestyle; or caged in comfort 
    4. starting to turn a profit; an apprentice; a student; a hustler; or a seasonal-soldier
    5. enough savings for emergencies an special occasions; a guild-member; an itinerant trader; or a mercenary
    6. full records, insurance, and regular savings; a master artisan; a residential merchant; or a professional-soldier
    7. an aristocrat living off of investments and intrest, or the exploitation of others; a superintendent; a guild-master; a knight; or a criminal kingpin
    8. born into wealth and sworn to fealty; lesser nobility; a viceroy; a chancellor; or robber baron
    9. a true blue-blood; practically (or literally) royalty; greater nobility; a warlord; or the cheif executive of a merchantile empire
  - Sense (#exploration, #mystery)
  - Links (#politics, #intrigue, #factions, #war)
    - contacts, social circles
  - Vigilance (#exploration, #mystery, #survival, #horror)
    - mental resilience to supernatural events
  - Otherness (#supernatural, #magic, #horror)
  - *Custom*
    - all of the above are just suggestions
    - if you don't like the names of some you can change them
      - the stats section of the character sheet has blank spaces so you can write-in whichever ones you need
    - or if want to make your own to suit your custom game themes you can do so easily
      - just think about how abilities work in relation to skills
      - make sure that the stat is something you can perform tasks and checks with, otherwise it might be better suited to being a custom a skill
  - *NPC stats*
    - npcs generally don't roll dice (or don't perform tasks, at least)
    - so the npcs need a few extra stats that player characters don't, in order to set the difficulty for opposing rolls
      - defences
- **items / equipment**
- **goals, habits, & creeds**
  - write about your character
  - 3 slots total — rewarded with lots
  - discuss with other players and the GM
- **lots & ego** (metacurrencies)
  - you can have up to 10 lots at a time
    - lots spent on tasks can reroll a die of your choice
      - or make all 0s rolled count as successes twice
    - one lot can be spent per check to reroll too
    - you can earn a portion of your lots back in the debreif every session by advocating for your portrayal of your character's aesthetic attributes and reflecting their choices throughout the session expressed via goals, habits, &/or creeds 
    - lots earned during the debreif that would bring you above the maximum, 10, are converted into $exp$ to help you level up any skills of your choice.
  - you either have ego at any given time, or you dont
    - spending ego on a just-failed task lets you retry it as a check
    - ego can't be spent on checks
    - you earn ego back in the debreif automatically
  - you start the game with ego and a number of lots chosen by the GM, depending on the starting situation (reccomended: 3-5)
  
### levelling up skills (failure bookeeping $=$ exp)
- two times the level of the skill is the number of tasks you must *fail* with that skill to level it up
  - i.e. you only learn from your mistakes
- levelling the skill happens immediately after the task is failed, or as soon as you notice that the exp bar is filled
- every time you level up a skill, the exp slate is wiped clean for that skill
  - e.g. level 4 skill requires 8 failed tasks to become level 5, then it needs 10 new failures
- 10 is the highest level for a skill, so you don't bother to track exp for a skill after that

#### learning new skills
- when you enter a situation where you would need to perform a task but don't have the right skill
- make a check instead with one of the associated abilities (as appropriate to the task)
- then add the unlearned skill to your sheet at level 0 with the first $exp$ checkbox checked
- mark additional $exp$ for all future checks made on behalf of that skill (regardless of success or failure)
- once the exp bar is filled completely (18 checks total):
  - the new skill immediately levels up to be the same level as your lowest known skill that shares the same ties
  - if you do not know of any other skills with those ties, then the newly learned skill only raises to level 1

#### skill list example
- skills are all doing-words: Verbs, with aclarifying nouns after a comma (if required)

| Skill           | Level | $exp$                        | Ties    |
| --------------- | :---: | ---------------------------- | ------- |
| Debate          |   3   | ☒☒ ☒☒ ☒☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Res/Wit |
| Sew             |   5   | ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Wit |
| Fight, swords   |   4   | ☒☒ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Swi |
| Conjure, spells |   0   | ☒☒ ☒☒ ☒☒ ☒☒ ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % | App/End |
| Research        |  10   | % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | End/Wit |

## knack examples
- knacks are all places, things, or ideas: nouns, but not proper nouns (and usually pluralized)
- they are always presented in lower-case *italics*
- since all knacks do the essentially same thing but for different fields of interest, their names should be fairly self-explanatory
  - that is, they shouldn't need descriptions unless they refer to foreign or fantastical concepts

## attribute examples
- attributes are all descriptive words relating to your character: adjectives, or the adjective form of certain nouns
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

# gameplay stuff:
- internal conflict resolutions
- character conflict resolutions
  - debates
  - duels
  - chases
  - battles
  - (positioning & wound tracking)
- environmental conflict resolutions
- supernatural conflict resolutions
- technological conflict resolutions
- societal conflict resolutions
  - wars