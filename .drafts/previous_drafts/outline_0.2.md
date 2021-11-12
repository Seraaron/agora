## design goals
- make a game that **I** want to play
  - versatile and scalable to most settings / situations (but especially my own worldbuilding project)
    - will require frontloading the character assembly process
    - but then the crunch for actual gameplay should be relatively low
  - focus on different types of conflict resolution or presenting actions with interesting choices resulting in memorable storytelling / narrative experiences
  - modular subsystems
    - modular character assembly sections
    - even the tasks system may be modular (play test this first!)
  - free and open source! anyone can contribute
- avoid making direct references to other ttrpg games and / or buzzwords
  - or at least the proprietary ones
  - linking to other creative commons resources is probably fine
- play-test often, every two weeks if possible
  - and get the first public release out within a month or two
- stream parts of the creation process at least once per week
  - (and make the VODs creative commons too)
- core mechanics (if this game was listed on RPGgeek.com)
  - standard d20 & dice pool resolution
  - strand character generation
  - attribute / ability based core capabilities
  - level & points based distribution
  - trait / aspect based gameplay
  - skill learning & advancement system
  - narrative / descriptive focus
  - wagering (metacurrencies) during gameplay
  - highlighted / wishlist features:
    - food and fashion choices matter
    - your character sheet tells a story about who you are and what you want

---

# game structure stuff / core philosophies:
<!-- parts of the markdown files should be commented in FULL CAPS for ease of Ctrl+F searching -->
- section titles are shorthands for the rules themselves
  - general game are first introduced in **bold**, but aren't capitalized
    - specific game terms are Capitalized
      - the only exception is **knacks**, which aren't capitalized but are *italicized*
    - Judge, Jury, Player, and Character are also capitalized
      - this means character is different from Character
    - some terms are also shortened, with most vowels removed and using a $spcl$ $fnt$ to make them easier to pick out
      - this font is also used for mathematical expressions and calculations
    - `monospace font` is used for changable game figures, indicating when to roll dice and what modifiers to add
      - small case `d` is used for Checks (roll-above) and rolling on random tables
      - upper case `D` is used for Tasks (pool-based successes) and only refers to D10s
    - use American spellings and use natural (or even casual) language
- speak to the reader: always use second person pronoun, 'you'
  - let context determine whether 'you' means the Judge, a player, or their character
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
    - character assembly / development
      - allows for re-jigging your character, changing some $caps$ or advancing to a new tier 
    - worldbuilding
  - anyone can ask for any kind of session in advance, but the assumed default is a normal session
- scenes, rounds, turns, & beats
  - scene types
    - encounters
    - interludes
    - vingnettes
  - turns start with the Judge and then always go clockwise
    - (or in the order that the players turned up to the session)
  - once a round passes where noone has anything else to add (or skips their turn) then the scene ends
  - any player (including the Judge) can also use [script change tools](https://briebeau.com/thoughty/script-change/) to pause, speedup, slowdown, or even rewind play
- two types of roll:
  - checks (simple verbs / actions)
    - straight-forward, quick and dirty, binary outcomes
    - target number based success critea, roll with `1d20 + Y + Z`
      - target = action type (i.e. 1 - 4) $\times$ 5 + circumstancial penalties (up to max target 30)
        - OR: target = opposing ability score $\times$ 3 + circumstancial penalties
      - result = `1d20` die roll + appropriate ability score (i.e. 1 - 9) `Y` + appropriate strand choice `Z`
        - count a natural 20 as an auto-pass
        - and a natural 1 as an auto-fail
      - check success = get result equal to or higher than target
        - margin of success or failure does not matter
        - and there is no notion of a 'critial'
  - tasks (complex verbs / skills)
    - complicated, slow but clean, potential for marginal outcomes
    - pool based success criterions, roll with `XD10 =< Y`
      - difficulty = action type (i.e. 1 - 4) + circumstancial penalties (up to max difficulty 10)
        - OR: difficulty = opposing ability score + circumstancial penalties
      - pool size `X` = skill level + circumstancial / staked advantages + help
      - total successes = count all rolls under given ability score `Y` appropriate to the task
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
- a target is what you aim for, don't shoot blind
  - always tell the players what the target / difficulty is before rolling 
- similarly, division is hard, so no all numbers used should be integers
  - if a calculation results in a fractional amount then *always round down*
- always set stakes, and be clear about failure conditions
  - set narrative stakes
  - failing better (not always failing forward)
  - players can offer potential failure solutions
    - and can narrate both their successes and their failings, if they want to
  - avoid re-rolling without changing the stakes
- your **Judge** refers to the GM or 'game moderator', or maybe it should be D/M for 'director / manager'? (referee is also acceptable)
  - *all* players are expected to adjudicate the game rules, not just the Judge
    - expl
  - the Judge is not necessarily in a position of power over the other players
    - it should be possible to play without a Judge, but this will not be covered
- your **Jury** refers to all the other players at the table except you
  - the Jury is a relative term, each player's Jury is different
    - and the Judge's Jury is all the other players
  - rules can be changed, broken, or removed by *any* player (including the Judge) at any time
    - but only with permission from that player's Jury
- let players direct/frame scenes!
  - maybe something that regenerates ego?
- the Judge never rolls (or at least never performs tasks)
  - contested tasks mostly work against ability or capability scores
  - defending yourself is a skill
- all mechanics are abstract representations of reality
- common sense vs. suspension of disbelief
- everything is relative
  - time, distances, difficulties
- no half measures, no sitting in the middle of the road
  - when categorising weapons and armour and such, there is no 'medium' option, all ranks are from 1 to 4 (or 0 to 5):
    - weights are: very light, light, heavy, or very heavy
    - lengths are: very short, short, long, or very long
    - ranges are: very near, near, far, or very far
    - actions are: very simple, simple, complex, or very complex
    - durations are: very fast, fast, slow, or very slow
    - visibilities are: very clear, clear, obscure, or very obscure
    - little effort, some effort, great effort, or monumental effort
    - ages are: infant 0, young 1, adult 2, aged 3, elder 4, senescent 5
- (nearly) everything is modular
  - core game engine [venus] will be `CC BY 4.0` (free cultural work)
  - everything else [evening_star] will be `CC0` (public domain)
    - this means anyone who wants to make content for the game can do so, and sell it if they want
    - but they must reference the venus engine in some way to bring a bit of unity to all projects
  - though both will be `All Rights Reserved` until the first major release, just in case

---

# minimum viable product / first play-test version
- pre-made characters for the players, consisting of
  - name, circumstances, strand choices
  - age, ability scores, attributes
  - VINPCs and essential gear?
  - capabilities
- checks *only*, no tasks
- a roleplay heavy scenario
  - since the basic system, using only checks, is very similar to most existing OGL RPGs this should just end up playing like an 'OSR' game
  - hence, it should handle dungeon crawling just fine, and I don't need to test that
  - so by focusing on a roleplay / action-oriented test session we'll get to see how granular checks are by themselves and whether tasks are even necessary

---

use some kind of metaphor for character creation
 - i like 'assmbly' because it implies that the character is built out of many separate peices that come to be something greater than the sum

# character assembly
0. **concept**

1. **tier**
  - tier sets the approximate 'power level' for play, it determines:
    - starting Ability Pool ($AP$) size, for distributing among your ability scores
  - all players must make characters of the same tier, unless they have their Jury's permission
    - tier can only change during development sessions, and must be unanimously voted on by all players

|   Tier | BRONZE | SILVER | GOLD  | PLATINUM |
| -----: | :----: | :----: | :---: | :---: |
|   $AP$ |   15   |   25   |  35   | |
| $caps$ |   +3   |   +5   |  +7   | |
| pass range | 8-10 | 6-10 | 4-10 | 2-10 | 


1. **circumstances**
  - *name*
    - your character's name
      - you can come back to this if you can't think of anything in the beginning
  - *background* — immutable
    - list aspects of your character's life circumstances that you think are improbable or impossible to ever change after character assembly
    - or use the space to declare which parts of your character's identity you have pre-determined and aren't interested in thinking about again
      - e.g. species, ancestry, roots, culture, colors, size, etc.
    - *size:* size is most likely determined by your species choice, roots, and age.
      - the GM may choose an appropriate range for the average size of your species to fall into, and you can then choose a size for your character specifically within that range (a special character feature would have to be taken to pick a different size from those offered by your GM)
        - for example, most adult humans on Earth are either tall or short, exhibiting a form of height-based sexual dimorphism; but a human child would be considered small, and babies are tiny
      - size is indexed from 1 to 6 as follows:
        - 1: tiny
        - 2: small / very short
        - 3: short
        - 4: tall
        - 5: large / very tall
        - 6: giant
      - size usually has very little mechanical effect, but sometimes the absolute difference in size between you and someone (or something) else may added as a penalty or a bonus to your actions, depending on what you're trying to do
      - (there are also two other typically unplayable sizes, '0: miniscule' and '7: colossal', these require GM permission to play as because their size differences compared to everything else can create some unexpected inconveniencies)
        - 0: miniscule
        - 7: colossal
  - *foreground* — variable
    - list aspects of your character's life circumstances that you think are might change over time (changable during development sessions, or after certain choices or realizations made in play)
    - or use the space to highlight parts of your character's identity that may be open to question, or at least not fully known (to you, or to anyone)
      - e.g. heritage, religion, community, class, gender, age, etc.
    - *age:* influences your ability score spread, and directly determines how many steps on your strand you may take.
      - age is indexed from 1 to 4:
        - 1: young characters (teenagers) get +1 $M_{AP}$, +3 $P_{AP}$, and 1-2 strands
        - 2: adult characters get +2 $M_{AP}$, +2 $P_{AP}$, and 3-4 strands
        - 3: matured characters get +3 $M_{AP}$, +1 $P_{AP}$, and 5-6 strands
        - 4: aged characters get +2 $M_{AP}$, +0 $P_{AP}$, and 7-10 strands
      - (there are also two other typically unplayable ages, '0: junior' or '5: senior', these require Jury permission to play as since they are quite vulnerable and likely to be difficult to roleplay respectfully)
        - 0: junior characters (children) get +0 $M_{AP}$, +1 $P_{AP}$, and 0 strands
        - 5: senior characters (elders) get +1 $M_{AP}$, +0 $P_{AP}$, and 11+ strands
  

3. **strands of life**
  - strands represent archtypical roles or vocations that your character has fulfilled or pursued at various points throughout their life
    - be they full occupations, periods of studentship, service, incarceration, or exile, snippets from your upbringing, or other walks of life
    - they are generic, but personalized; and thread by thread they weave together to make a tapestry that implicitly tells the story of both your character's life so far or the situations they've lived though
  - strands affect what attributes (skills, features, and knacks) your character can aquire and advance during assembly
  - and how many $caps$ (character attribution points) you have to spend on those things:
    - each new strand taken grants +5 $caps$ the first time (to encourage diversification)
    - but each strand taken more than once grants +9 $caps$ each time (to encourage specialisation)
      - e.g. taking 'Soldier $\times$ 3' grants a total of 23 $caps$
  - $caps$ are used to buy skill levels, knacks, and features (see below for pricing)
  - strands have a title, followed by a list of potential skills, features, and knacks that you can take
    - all strands have 9 of these
      - all strands without requirements offer precisely 3 skills, 3 knacks, and 3 features
      - strands with requirements mix it up a bit more, but still stick to the 9 total limit
        - some strands use other strands as pre-requisities, others use your age, or certain features
    - when you take a strand, roll `1d10`, the listed attribute that the roll lands on (counting from 1, left to right, top to bottom) is given to you for free
      - if you roll a 0 then you may choose your free attribute
        - if you are taking the same strand multiple times and roll the same attribute more than once, then you may also choose
      - if the rolled / chosen attribute is a skill then it just opens at level 1 for free
        - and +1 level for each time you roll / choose the same skill if you take the same strand multiple times 
    - this randomness is injected to make your character a bit more unique and to force you think about how the circumstances that lead them to learning that skill, or picking up that feature, or earning that knack
  - strands also list items and equipment that you would likely own as a result of taking them

4. **ability scores**
  - you use your abilities to perform checks (simple verbs)
    - roll `1d20+X` where X is your ability score
    - try to meet or exceed the target set by the Judge (3 $\times$ the difficulty)
    - checks have binary 'pass' or 'fail' criterions
  - $MA$ [mental abilities]
    - Appeal (App) — mental grace, charisma, personal charm, social understanding, and emotional senses
    - Resolve (Res) — mental resilience, wisdom, determination, memory retention, and temporal senses
    - Wits (Wit) — mental power, intelligence, logical reasoning, shrewdness, instinct, and spatial senses
  - $PA$ [physical abilities]
    - Endurance (End) — physical resilience, constitution, stamina, vigour, and regular movement upkeep (aerobics)
    - Finesse (Fin) — physical grace, dexterity, flexibility, style, overall body coordination and balanced movements
    - Swiftness (Swi) — physical power, strength, reflexes, alacrity, and quick movement speed (anaerobics)
  - scores all start at 0 `▯▯▯▯ ▯▯▯▯` and range up to 8 `▮▮▮▮ ▮▮▮▮`
    - increase scores by spending the $AP$ based on your tier, and the bonus points to each pool from your age
      - it is advised for most characters to try to keep all their abiltiy scores in the 2-6 range
    - after character assembly, ability scores can only go up (or down) during development sessions
      - this partly depends on your new age (if a lot of time has passed), but is mostly voted on by Jury when it's decided to advance the tier for a character
  - your ability score also sets the base difficulty when certain checks and tasks are performed against you
    - when this happens it's important to be clear about the failure conditions, and make sure the other player agrees to be tested against
  
5. **spending your $caps$**

- **skills** (verbs)
  - you use skills when performing tasks (complex verbs)
    - roll `XD10` where X is equal to your skill level plus any modifers and advantages that you've advocated for in the negotiation phase:
      - if more than one skill seems to be related and applicable to the task then use the lowest one, and grant a bonus die for the task
      - similarly if an ally wants to help, then they must use a related skill, and the lowest levelled one between you rolls and gets a bonus dice from the other
        - each character can only help with one skill at a time
        - when helping, if the task fails, the helpers each get an experience point in the skill the helped with
      - between related skills and help, you may only gain a maximum total of `+3D`
    - each die must roll equal to or below the ability tie for the given task to count as a success
    - if total successes meet or exceed the difficulty then the task is completed successfully
    - margin or success or failure may matter, depending on circumstances
  - they are tracked and levelled individually by counting total failed tasks over time
    - twice the current level is the number of failed tasks needed to advance a skill level
  - each skill is tied to two abilities, resulting in 15 possible combinations:
    - App$/$Res, App$/$Wit, App$/$End, App$/$Fin, App$/$Swi, Res$/$Wit, Res$/$End, Res$/$Fin, Res$/$Swi, Wit$/$End, Wit$/$Fin, Wit$/$Swi, End$/$Fin, End$/$Swi, Fin$/$Swi
      - (for the sake of consistency, each tie should always be ordered alphabetically)
        - so you should never write Res$/$App, for example
        - but if you do so by mistake then it's okay, because it just means the same thing as App$/$Res
    - plus some skills may have special exemptions related to their ties, or may have unique uses with certain capabilities
      - these have the letters $Sp$ in superscript next to their listed ties and a note explaining the special case in the skill's description / effects
    - the tie's score is the ability value to roll under when performing a task with the dice of that skill
      - which one you roll against depends on the circumstances of the task / the way you use the skill
  - bought with $caps$
    - if the skill is listed in any of your strands then it costs 1 $cap$ per level up to level 5, then 2 $caps$ per level
    - if the skill is not listed, then you learned it by yourself, and so costs 2 $caps$ per level and can't be raised higher than level 5 during character assembly 

- **features** (adjectives)
  - features are either Aesthetic ($As$), Potent ($Pt$), or Limiting ($Lm$), and they represent your characters quirks, flaws, features, powers, handicaps, and so forth
    - aesthetic features don't grant direct bonuses to tasks, but they can award lots at the end of each session for representing them well during play
      - cost 1 $cap$ if they were listed in your strands, or 2 $caps$ otherwise
    - potent features grant magical powers or special talents to use, allowing your character to do more than they would be able to without them (i.e. potent features are explicitly allowed to break the normal rules of play)
      - cost 2 $caps$ if they were listed in your strands, or 4 $caps$ otherwise
    - limiting features are typically health conditions (injuries, disabilities, or diseases) that increase the difficulty of certain tasks and checks for your character
      - as such, taking a limiting feature from your strand list *grants you* +2 $caps$, otherwise they only grant +1 $caps$
      - (you may only take a maximum of 3 non-strand limiting features)
  - some features can be considered either one type or another, or sometimes both at the same time — called 'combined features'
    - $As/Pt$ features are aesthetic features that can be upgraded to include a potent effect
      - it costs +1 $cap$ to buy the upgraded effect (for a total of 2-3 $caps$)
    - $Lm/As$ features are limiting features that can eventually 'heal' to become aesthetic features, like scars, or things which no longer physically limit you but still show some sign of having once affected you (allowing you to earn lots from them if portrayed through play)
      - these features cost +1 $cap$ to 'heal' (for a total of -1-0 $caps$)
    - $Pt/Lm$ features are potent features with limiting downsides or handicaps
      - these are dicounted by -1 $cap$ from their normal price (for a total of 1 or 3 $caps$)

- **knacks** (nouns)
  - knacks are speciality interests, natural talents, trained knacks, , or other quirks that grant bonus knowledge, access to new locations, the expertise to use certain kinds of gear, or other special privilages
    - they are *not* used directly with any tasks or checks
      - to use them regularly, you must draw on the knack for descriptive or narrative inspiration
      - then the Judge will respond in kind if they have information to give you that your character *should already know*, based on their knacks
      - this can esablish a new (i.e. previously unknown to the Jury) fact about yourself, the world, or the current situation
        - both you and the Judge can contribute to this information, collaborating until you settle on something that you both like and which makes sense in context
        - but the Judge is the final arbiter of 'the whole truth' in this instance
    - alternatively, your knack may enable you to make a roll that you would not normally be able to make
      - you don't get any inherent bonuses because of the knack, in this case, just a chance where any other character would not have one
    - the use of any given knack should be implicit, based on it's name
      - but in the cases where it is obscure, some use-cases will be suggested
    - or maybe they lower the difficulty of a roll?
  - bought with $caps$:
    - 1 $cap$ per knack if listed in your strands
    - or 3 $caps$ if not listed
  - they are always written in *lower-case italics*

- *innate attributes*
  - some attributes are denoted as *innate* in the strand description
    - denoted with the letters $In$ in superscript next to their name when listed 
  - they are so important to that strand that it is either expected that you would attain them from that strand or that they are somehow necessary to take the strand in the first place
  - therefore, you may add them to your character without spending any $caps$
    - innate features and knacks are simply added for free
    - innate skills only start at level 1 for free

1. **kith & kin** (proper nouns)
  - these are very important non-player characters or VINPCs (pronounced 'vin-pee-see') that you have designated as being very important your character or the story
  - you are limited to a maximum of 3 VINPCs in total, regardless of your tier
    - only the Judge may raise or lower this limit, since they are the one that will most-likey have to design and portray them all
    - therefore, you must also discuss each one in detail with your Judge
    - if you have no ideas about which characters may be important to you, don't worry
      - you can ask for an NPC you've met ingame to be designated as a VINPC during downtime or development sessions
      - similarly, a character whom you thought would be important may turn out not to be
        - it's ok to downgrade them back to being normal NPCs
  - you can also use your strands and circumstances to guide which sorts of NPCs you are most likely have relationships with
  - VINPCs can occasionally function like knacks, in that: they can offer you advice, tell you secrets, grant you acess to special places, award you with titles or powers, and so forth
    - but you have little to no control over them, they are the Judge's characters ultimately
  - they are always written in *Upper-Case Italics*

7. **gear & sundry**
  - strands list the sorts of items, equipment, & property that you would likely own as a result of taking them
    - you can add one item from this list to your sheet each time your take the same strand
      - e.g. taking Soldier $\times$ 3 gives you 3 different items from it's list
  - the lists are meant to be evocative, more than anything, rather than being strict accouterments or uniforms
  - as such, once you have chosen everything you want off the lists, you can also pick up any other bits and peices that you think are appropriate for your character to own (with your Jury's permission)
    - how much to write in depends on play style, game themes, and personal preference
    - if playing with survival themes then it might make sense to track every penny and morsel
    - but if you're using the wealth capability then the capability itself can be used to define what you own, when it becomes relevant through play
    - as such, by default, this game has no precious metal peices, credits, or other currencies to keep track of that are spendable during character assembly
      - but once the game begins, if your game needs them, then the Judge's wouldbuilding will decide how much everything is worth, and how much money you own, based on your circumstances and strand choices, and you would write them in with all your other possessions
      - this an aspect of play that's very much time-period and setting specific
      - economies are complex, so no further guidance is offered in this respect, at this time (sorry)

---

8. **capability scores** (derived abilities) [module]
  - capabilities function almost identically to abilities, except that:
    - they are *derived* from your current ability scores and choices mades during a questionnaire
    - they can only be used to perform checks, not tasks
      - (unless you have a special skill tied them)
      - often, failing a capability check takes a certain amount of agency away from your character for a brief time 
    - they are also completely optional / modular, and tagged based on game-themes
      - if you know your game won't contain any of those themes then you can pretty safely ignore those capabilities
    - however, sticking to a theme is important so that the game doesn't get diluted, so you may only choose up to 3
      - decide as a group which ones you feel would be necessary or useful for your game
      - different PCs *can* each have different capabilities, but only if it makes sense...
        - that said, it's better to try to be consistent
      - since they are all derived, you can change out capabilities in a development session for new ones if your game theme has shifted
      - and re-derive them again when the theme shifts back
        - you may find you have different or new answers to the questions asked in the derivation process, and that's okay (arguably intentional)
  - *Grit* (#violence, #combat, #war)
    - a measure of your general audacity and your readiness to injure others, your disposition
      - governs instinctual reactions in a fight
    - calculated by: Add Wits and Swiftness, divide by 4, + questionnaire answers
  - *Guts* (#violence, #combat, #mystery, #horror)
    - a measure of your physical and mental tolerance for putting yourself in harms way and potentially being injured, your mettle
      - governs how long you can keep up the fight (akin to HP)
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
    - calculated by: Jury decision based on circumstances, strands, and questionnaire answers
  - *Links* (#politics, #intrigue, #factionalism, #war)
    - represents a 'social wealth' of sorts: your current contacts, patrons, factions you are affiliated with, past associates, rivals, or lovers, and any favors still owed or contracts you've entered into with them
    - good for social games set in a single city or county, not great for world-hopping adventures (better to just use 'first-impessions' Appeal checks in that case when meeting new people)
    - calculated by: half your Appeal score + questionnaire answers
  - *Vigilance* (#exploration, #mystery, #survival, #horror, #supernatural)
    - mental resilience to abnormal events and existential dread, your spirit or temperance
    - calculated by: age bracket (1-4) + questionnaire answers
  - *Honor* (#feudalism, #politics, #chivalry)
    - calculated by: questionnaire answers
  - *Soul* (#supernatural, #magic, )
    - calculated by: questionnaire answers
  - *Custom*
    - all of the above are just suggestions
    - if you don't like the names of some capabilities you can, of course, change them for your group
      - as long as you're consistent
      - the capabilities section of the character sheet has 3 blank spaces so you can write-in whatever you like
    - or if want to make your own to suit your game themes you can do so easily
      - recall how abilities work in contrast to skills
        - make sure that the capability is something you can only perform checks with, otherwise it might be better suited to just being a custom a skill
        - think of some potential checks that could be performed with the capability, and how their outcomes could affect your players or their characters
      - think of a a short questionnaire and use the player's answers can help to generate the score
      - test out the capability through play, if you don't like it then tweak it during development sessions
  - *NPC capabilities*
    - npcs generally don't roll dice (or don't perform tasks, at least)
    - so the npcs need a few extra capabilities that player characters don't, in order to set the difficulty for opposing rolls:
      - or do they?

9. **goals, habits, & creeds** [module]
  - write about your character
  - 3 slots total — rewarded with lots
  - discuss with other players and the Judge

10. **lots & ego** (metacurrencies) [sub-module]
  - *lots*
  - you can have up to 10 lots at a time
    - lots spent on tasks can reroll a die of your choice
      - or make all 0s rolled count as successes twice
    - one lot can be spent per check to reroll too
    - you can earn a portion of your lots back in the debreif every session by advocating for your portrayal of your character's aesthetic features and reflecting their choices throughout the session expressed via goals, habits, &/or creeds 
    - lots earned during the debreif that would bring you above the maximum, 10, are converted into $exp$ to help you level up any skills of your choice
  - *ego*
  - you either have ego at any given time, or you don't
    - spending ego on a just-failed task lets you retry it as a check
    - ego can't be spent on checks
    - earn back ego from introducing your own scenes
  - you start the game with ego and a number of lots chosen by the Judge, depending on the starting situation
    - (reccomended: 3-5)

---

### levelling up skills (failure bookeeping = $exp$)
- two times the level of the skill is the number of tasks you must *fail* with that skill to level it up
  - i.e. you only learn from your mistakes
- levelling the skill happens immediately after the last task is failed (or as soon as you notice that the exp bar has been filled sometime thereafter)
- every time you level up a skill, the $exp$ slate is wiped clean for that skill
  - e.g. level 4 skill requires 8 failed tasks to become level 5, then it needs 10 new failures
- 10 is the soft level cap for all skills
  - the only way to advance above 10 in a skill is with the aid of a custom-made potent feature, supernatural training, or the used of advanced technologies

#### learning new skills
- when you enter a situation where you would need to perform a task but don't have the right skill
- make a check instead with one of the skill's tied abilities (as appropriate to the task)
- then add the unlearned skill to your sheet at level 0 with the first $exp$ checkbox checked
- mark additional $exp$ for *all* future checks made on behalf of that skill (regardless of success or failure)
- once the exp bar is filled up completely (18 checks total):
  - the new skill immediately levels up to be the same level as your lowest known skill that shares the same ties
  - if you do not know of any other skills with those ties, then the newly learned skill only raises to level 1


| Skill           | Level | $exp$                                | Ties            |
| --------------- | :---: | ------------------------------------ | --------------- |
| Debate          |   3   | ☒☒ ☒☒ ☒☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Res/Wit         |
| Sew             |   5   | ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Wit         |
| Fight, swords   |   4   | ☒☒ ☐☐ ☐☐ ☐☐ % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | Fin/Swi         |
| Conjure, spells |   0   | ☒☒ ☒☒ ☒☒ ☒☒ ☒☒ ☒☐ ☐☐ ☐☐ ☐☐ % | App/End$^\star$ |
| Research        |  10   | % ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ ☐☐ | End/Wit         |

## skill list example
- skills are all doing-words: verbs, with a clarifying nouns after a comma (if required)

## knack examples
- knacks are all places, things, or ideas: nouns, but not proper nouns (and usually pluralized)
- they are always presented in lower-case *italics*
- since all knacks do the essentially same thing but for different fields of interest, their names should be fairly self-explanatory
  - that is, they shouldn't need descriptions unless they refer to foreign or fantastical concepts, or unless they do something special like 'longswords'

## feature examples
- features are all descriptive words relating to your character: adjectives, or the adjective form of certain nouns, or a short descriptive sentence if a single word or two can't seem to encapsulate the concept


###### $As:$ **Lovely Smile** ######
*description (if any)*
  - upgrade option (if any)


###### $Lm:$ **Blind in one Eye** ######
*description*
- effect `n`
  - *notes / clarifications (if any)*
- effect `n+1`


###### $Pt:$ **Chosen** ######
*description*
- effect

---

# additional / modular gameplay features
ultimately, almost all mechanics can be abstracted into different kinds of conflicts. each kind may have it's own system of resolution
- internal conflict resolutions
  - healing / recovery
  - changing your mind
  - problems that cannot be solved with your character sheet
    - i.e. player skill vs character skill
- character conflict resolutions
  - battles
    - active-initiative battle system?
  - chases
  - debates
  - duels
  - sex, money and violence
- environmental conflict resolutions
  - animals
  - traps
  - envrionmental penalties are grouped such that you only apply the highest if multiple are applicable:
    - light / visibility levels
    - terrain stability
  - natural disasters
- supernatural conflict resolutions
  - religions
  - summoning weird things
- technological conflict resolutions
  - vehicles
- societal conflict resolutions
  - politics
  - wars

### (mars)
fully optional (i may never actually write this) supplemental material for combat heavy / borderline weapons-fetishistic games where the capabilities of every minute detail are really important