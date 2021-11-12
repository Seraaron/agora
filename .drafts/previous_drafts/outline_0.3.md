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
  - archetype character generation
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
  - general game terms are first introduced in **bold**, but aren't capitalized
    - specific game terms are Capitalized
      - FC and Peer are also capitalized
    - some terms are also shortened, with most vowels removed and using a $spcl$ $fnt$ to make them easier to pick out
      - this font is also used for mathematical expressions and calculations
    - `monospace font` is used for changable game figures, indicating when to roll dice and what modifiers to add
      - small case `d` is used for Checks (roll-above) and rolling on random tables
      - upper case `D` is used for Tasks (pool-based successes) and only refers to D6s
    - use American spellings and use natural (or even casual) language
    - this document is written in an outlining style
      - where sub-bullets add clarity or additional thoughts to the main bullet
- speak to the reader: always use second person pronoun, 'you'
  - let context determine whether 'you' means the FC, a player, or their character
- structuring campaigns, major and minor arcs, and chapters
  - campaigns (1-3 major arcs = 30-100 sessions)
  - major arcs (1-3 minor arcs = 10-30 sessions)
  - minor arcs (1-3 chapters = 3-9 sessions)
  - chapters (1-3 sessions)
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
  - rounds start with the FC's turn and then always progress clockwise
    - (or left-to-right or top-to-bottom if playing online)
  - once a round passes where no one has anything else to add (or skips their turn) then the scene ends
  - any player (including the FC) can also use [script change tools](https://briebeau.com/thoughty/script-change/) to pause, speedup, slowdown, or even rewind play
- two types of roll:
  - checks (simple verbs / actions)
    - straight-forward, quick and dirty, binary outcomes
    - target number based success criteria, roll with `1d20 + X + h(Yd6)`
      - target = absolute difficulty (0-5) $\times$ 5 + relative difficulty factors, up to +4 (ie. target spread = 0-29)
      - result = `1d20` die roll + appropriate ability score `X` (chosen by the FC) + the highest roll `h()` of `Yd6`, where `Y` is the sum of any appropriate (ie. peer reviewed) bonus factors from your archetypes, attributes, spent lots, or aid.
        - no autopass for Bronze, 20s for Silver, 19-20s for Gold, and 18-20s for Platinum
      - check success = get result equal to or higher than target
        - margin of success or failure does not matter
        - there is no inherent notion of a 'critial'
        - you will not automatically fail on a natural 1
  - tasks (complex verbs / skills)
    - complicated, slow but clean, potential for marginal outcomes
    - pool based success criterions, roll with `(X+Y)D6 > W`
      - threshold = appropriate (ie. peer reviewed) difficulty + relative difficulty factors, up to +6 (ie. threshold spread = 1-10)
      - pool size = job level `X` + up to 2 aiding dice `Y` (rolled separatately by the aiding allies)
      - total passes = pass target per die depends on ability rank (chosen by the FC):
        - bronze = 5s and 6s only, silver = 4-6, gold = 3-6, platinum = 2-6 
      - KISS individual dice to reroll them: kismet, insight, stunts, or specialties.
        - use ego to double-count all 6s rolled (ie. each 6 counts as a pass twice)
      - task success = total passes greater than the threshold
        - margin of success or failure may matter in certain instances:
          - meeting or exceeding the difficulty by *double* may result in a 'critial success'
          - getting successes equal to *half* the difficulty or less may result in 'total failure'
        - otherwise, you should still 'fail-forward' in some capacity, or get 'success with a twist'
  - this means players only need a handful of d6's and a d20 to play — which most ttrpg people *already have*
    - so the proprietary elements / barriers to entry are kept low
- it's easier to do addition than it is to subtract
  - bonuses should always add to your dice or roll
  - penalties should always add to the difficulty
    - only *execptional* powers / attributes, should break these heuristics
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
- your **FC** refers to the Facilitator ('referee' and 'game manager' are also acceptable)
  - *all* players are expected to adjudicate the game rules, not just the FC
    - expl
  - the FC is not necessarily in a position of power over the other players
    - it should be possible to play without a FC, but this will not be covered
- your **Peers** refers to all the other players at the table except you
  - the Peer is a relative term, each player's Peer is different
    - and the FC's Peers are all the other players
  - rules can be changed, broken, or removed by *any* player (including the FC) at any time
    - but only with permission from that player's Peer
  - if something is said to require 'peer review' then it offers a a moment to open the discussion up to the whole table
- let players direct/frame scenes!
  - maybe something that regenerates ego?
- the FC never rolls (or at least never performs tasks)
  - contested tasks mostly work against ability or capability scores
  - defending yourself is a skill
- all mechanics are abstract representations of reality
- common sense vs. suspension of disbelief
- rulings not rules
- everything is relative
  - time, distances, difficulties
- no half measures, no sitting in the middle of the road
  - when categorising weapons and armour and such, there is no 'medium' option, all indexes are from 1 to 4 (or 0 to 5)
- (nearly) everything is modular
  - core game engine [venus] will be `CC BY 4.0` (free cultural work)
  - everything else [evening_star] will be `CC0` (public domain)
    - this means anyone who wants to make content for the game can do so, and sell it if they want
    - but they must reference the venus engine in some way to bring a bit of unity to all projects
  - though both will be `All Rights Reserved` until the first major release, just in case

---

# minimum viable product / first play-test version
- pre-made characters for the players, consisting of
  - name, circumstances, archetype choices
  - age, ability scores, attributes
  - VINPCs and essential gear?
  - capabilities
- checks *only*, no tasks?
- a roleplay heavy scenario
  - since the basic system, using only checks, is very similar to most existing OGL RPGs this should just end up playing like an 'OSR' game
  - hence, it should handle dungeon crawling just fine, and I don't need to test that
  - so by focusing on a roleplay / action-oriented test session we'll get to see how granular checks are by themselves and whether tasks are even necessary

---

# character assembly

## 0. concept
  - think about what kind of character you want to make given the setting and the tone of the game that your FC wants to run
    - in some cases, your FC may wish to run several development sessions where you collaboratively world-build with the other players before you even begin to think about what sort of characters you'll each play
      - this can be done purely improvisationally, or with the guidance of a proprietary worldbuilding game
    - in other cases, your FC will be using a preestablished or well-recognised setting
      - either one that they've made up themselves or run games in before; a setting that you all know and love from popular culture; or a game set in a part of Earth's real or alternative world history, or a shared imagined future
  - a good character concept is a single sentence or picture that sums up your idea for them
    - the concept might initially be very out-of-focus or loaded with stereotypes, references, or tropes
    - but that's okay because you don't need to write it down anywhere, you just spitball your ideas at first and see how your Peers react to them 
    - plus the rest of the character assembly process will determine how your character differs from those touchstones — and perhaps how they are still the same — until they are slowly brought forth into enough mental clarity that you feel comfortable and confident to protray them in game  

## 1. circumstances
##### *names*
  - your character's name, alias, or title (and optionally, their pronouns)
    - you can come back to this later if you can't think of a character name right at the beginning of assembly
    - or you may even decide to change your name during play, either because of some in-game revelation, or because you simply don't think their current one suits them any more
  - and your own name, as a player, so the FC can tell who's who

#### tier
  - tier sets the approximate 'power level' for play, it determines a few major character aspects according to the table below
  - all players should make characters of the same tier, unless they have their Peer's permission
  - tier can only change during development sessions, and must be unanimously voted on by all players

|                        Tier | REALISTIC | HEROIC | MYTHIC | DEIFIC |
| --------------------------: | :-------: | :----: | :----: | :----: |
| $N^o$ *free* Rank Increases |     1     |   3    |   5    |   7    |
|             Bonus Archtypes |     0     |   1    |   2    |   3    |

  - The realistic tier represents historic and political characters acting in an assumedly normal world. It represents people like you and I, most likely, and nearly everyone else who has lived and died on Earth.
  - Heroic tier is for playing out believable tales about people who quest for glory or struggle to leave their mark on the annals of history, culture, or legend — gifted-rogues, warrior-poets, adventurer-prophets, philosopher-engineers, or sorcerer-monarchs — whose efforts may not be really possible without either a story-teller's embellishments or a true touch of magic. You may also want to refer to this as the 'cinematic' tier.
  - The mythic tier is the place of spirits, demigods, superheroes, and exalted mortals; where paranormal events occur regularly and legendary deeds may be performed with few questions asked — though not without consequence.
  - Characters in the deific tier may not necessarily be literal deities, but perhaps their personas are large enough or their powers are great enough to be revered as divine or immortal by specific religious groups, or perhaps they are shards of an even greater being given mortal form.

#### background — immutable circumstances
  - list aspects of your character's life circumstances that you think are improbable or impossible to ever change after character assembly
    - e.g. ancestry, people, roots, culture, hues, tones, values, patterns, etc.
  - or use the space to declare which parts of your character's inward identity or personality you have pre-determined and aren't interested in ever changing

###### size 
  - most typically determined by species, ethnicity, diet, and age; it represents an approximate combination of your height, length, and weight
    - for example, most adult humans on Earth are between 5 and 6 feet (150-180 cm) tall, so this puts them at a modest size; but a human child would be considered small or tiny.
    - Meanwhile, tigers and horses are of ample size, and hippos would be considered large; despite generally being shorter than most humans at the shoulder, they are simply more massive than us once they reach maturity.
  - size is indexed from 1 to 4 as follows (with approximate metrics for Earth-like settings)
    1. Small ~ 2-5" (90-150 cm) & less than a quintal
    2. Modest ~ 5-6" (150-180 cm) & 100-250 lbs (45-110 kg)
    3. Ample ~ 6-7" (180-210 cm) & 250-2200 lbs (110-1000 kg)
    4. Large ~ 7-9" (210-270 cm) & more than a tonne
  - size usually has very little mechanical effect, but sometimes a difference in size between you and someone else may added as a relative factor — either as a penalty or a bonus — to your actions depending on what you're trying to do
  - (there are also some other unplayable sizes, typically reserved for animals and monsters, and which would require FC permission to play as because their size differences compared to everything else can create some unexpected inconveniencies)
    - These include: miniscule, tiny, giant, enormous, colossal, and immense.

#### foreground — variable circumstances
  - list aspects of your character's life circumstances that you think could be open to change over time (changable during development sessions, or after certain choices or realizations made in play)
    - e.g. religion, community, class, gender, physique, colors, shapes, etc.
  - or use the space to highlight parts of your character's outward identity or appearance 

###### age
  - influences your starting ability score spread, and directly determines how many archetypes you may take.
    - age is indexed from 1 to 4, for adults:
      1. young characters get +1 MA$_{sp}$, +3 PA$_{sp}$, and 1-2 Archetypes
      2. mature characters get +2 MA$_{sp}$, +2 PA$_{sp}$, and 3-4 Archetypes
      3. aged characters get +3 MA$_{sp}$, +1 PA$_{sp}$, and 5-6 Archetypes
      4. old characters get +2 MA$_{sp}$, +0 PA$_{sp}$, and 7-9 Archetypes
   - (there are also two other typically unplayable ages, '0. junior' or '5. senior', usually reserved for NPCs. These require Peer permission to play as since they are quite vulnerable and likely to be difficult to roleplay respectfully)
      - junior characters (children) get +0 MA$_{sp}$, +2 PA$_{sp}$, and 0-1 Archetypes
      - senior characters (elders) get +1 MA$_{sp}$, +0 PA$_{sp}$, and 9+ Archetypes
  
## 2. archetypes
  - archetypes (or ATs) represent roles or vocations that your character has fulfilled or pursued at various points throughout their life
    - be they full occupations, periods of studentship, service, incarceration, or exile, snippets from your upbringing, or other walks of life
    - they are generic, but personalized; and step by step they implicitly tell the story of both your character's life so far and the settings they've lived in
      - that said, the order that you take archetypes in does not need to be chronological
      - and you *cannot* take the same archetype multiple times
    - some archetypes have prerequisites; such as being a specific age or tier, having certain attributes, being a member of a given social or economic class, or requiring that you have a different archetype first
  - archetypes have a name or a title, which you should write at the top of your character sheet as you take them
  - archetypes may be divided and grouped into sectors, for example:
    - production, manufacturing, service, scholastic, management, and rogue.
    - this just helps to organize them, and may not have any actual effect
  - each archetype adds +1 to your ability score pool or $sp$ by presenting either an 'MA', a 'PA', or a pair of specific abilities 'X/Y', or the word 'Any':
    - MA and PA mean you can add +1 to any mental or physical ability of your choice, respectively
    - a pair of abilities, such as 'App/Res', means you must choose one of those two abilities to add +1 to
    - and 'Any' means that you add +1 to any ability you like
  - all archetype grants +5 $caps$ (character attribution points) and +9 $jips$ (job incrementation points)
  - each archetype also provides you with two main lists, to spend those points on:
    - a numbered list of up to 6 attributes that you can purchase at a 1 point discount with your $caps$ in step 5
    - and a bulleted list of jobs that you are allowed to start and level up with your $jips$ during step 6
  - when you take an archetype, you should roll a `d6` and look up the result on the numbered list for that archetype: you may then take the corresponding attribute *for free*
    - if there are less than 6 items on a list and you roll a number that isn't present, then you may choose which attribute you want as your freebie from the rest of that same list
      - similarly, if you roll an attribute that you have already rolled / chosen from another archetype, then just choose a different one for free
    - this randomness is injected to make your character a bit more unique and to force you think about what the circumstances may have that lead to you picking up that attribute — be it positive, or negative
  - similarly, once you have taken all the archetypes you wish to, if there is an overlap of jobs on the lists provided (*ie.* if any given job appears more than once across two or more different archetypes) then you may start any of those jobs *for free*
  - you can make up new archetypes, but since the list of all available archetypes sort of implicitly describes the larger setting that you're playing in, the creation of new archetypes is left to the FC
    - though you can of course suggest ideas to your FC and see if they can come up with anything on the spot
    - guidelines for FCs to help them make new archetypes are given in their own chapter / section (not written yet)  

## 3. abilties
  - Mental Abilities (MA)
    - **Appeal** ($App$)
      - mental grace, charisma, social prowess, artistic sentiment, and emotional senses
      - used for: feigning ignorance, making a good first impression, offering ideas or trading goods, and pleading for help  
    - **Resolve** ($Res$) 
      - mental resilience, wisdom, patience, determination, memory retention, and temporal senses
      - used for: counting, finding, and mending things, remembering information you should already know, and working long hours
    - **Wits** ($Wit$) 
      - mental power, intelligence, shrewdness, logical reasoning, instinct, and spatial senses
      - used for: aiming projectiles, problem solving, identifying and inspecting things and making connections, and watching, listening, or reading
  - Physical Abilities (PA)
    - **Endurance** ($End$) 
      - physical resilience, constitution, stamina, vigour, and regular movement upkeep (aerobics)
      - used for: long-distance walking or jogging, holding your breath, treading water, wrestling, and eating or drinking strange things
    - **Finesse** ($Fin$) 
      - physical grace, dexterity, flexibility, style, overall body coordination and balanced movements
      - used for: hitting things with weapons, balancing and stretching, crawling and sneaking around, and escaping binds
    - **Swiftness** ($Swi$) 
      - physical power, strength, reflexes, alacrity, and quick movement speed (anaerobics)
      - used for: dodging or parrying, catching things, jumping and landing safely, pushing or pulling things around, and quick sprints

#### ranks vs. scores
*rank* represents your potential to succeed as raw talent, whereas *score* represents your training and growth
  - your ranks depends primarily on your tier (see above), as all your abilities start at Bronze rank and then you may assign 1-7 *free* rank increases according to your tier
  - rank can also increase by buying special attributes with your $caps$
    - but they are expensive and are rarely offered in archetypes
  - at the end of each major story arc (ie. about once every 15-30 sessions), your peers may discuss whether you deserve a rank increase in recognition of your character's achievements thus far
    - and if you do, then you may choose which ability to allocate it to
  - rank affects the natural success range of your d20 roll for Checks
    - and determines the pass range for all the D6's in your dicepool for Tasks

| Ability Rank                       | Bronze $(Br)$ | Silver $(Si)$ | Gold $(Go)$ | Platinum $(Pl)$ |
| ---------------------------------- | :-----------: | :-----------: | :---------: | :-------------: |
| Natural Success Range *for Checks* |      NA       |      20       |    19-20    |     19-20*      |
| Natural Success Chance *per d20*   |      0%       |      5%       |     10%     |       10%       |
| Pass Range *for Tasks*             |      5-6      |      4-6      |     3-6     |       2-6       |
| Pass Chance *per D6*               |      33%      |      50%      |     67%     |       83%       |
\* Does not auto-fail on a 1
  - scores all start at $+1$ and may range up to $+8$, but they will probably sit in the 1-3 range for most characters starting out
    - increase scores by distributing the score pool $sp$ generated by your age and archetype choices (see above)
    - after character assembly, ability scores can only change during development sessions
      - at the end of each minor story arc (ie. about once every 5-10 sessions) and after some discussion, your Peers may vote on which of your abilities should advance by 1, based on what they think you have most commonly been using
      - or when so much time passes that your age increase, then some of your scores may go up or down, which you may allocate yourself
  - scores are added to your Checks as a flat bonus
    - and are used in Tasks to determine your starting level for a given job (based on the *lowest* of it's two inherited abilities)
      - or the amount of dice to roll while learning a new job (based on the *highest* of it's two inherited abilities)
  
## 4. attributes
  - **Assets**
    - $Rs:$ Resources — 4 $caps$
      - property and real estate, great funds, fortunes, or inheritances, stocks and bonds, vehicles and machines, fine art and furniture, rare artefacts and treasures, livestock, or other large quantities of wealth or stores of value that are not easily transferable
      - resource assets typically have a physical use: for example, buildings can be lived in, land can be worked, ships and trains can transport people or things, magical swords can slay monsters, and art can be used as tax write-offs
        - in all of these cases, the usefulness of item in question should be fairly implicit or else come with a description or explanation
          - in the case of magical items, rare artefacts, and advanced technologies, they may *themselves* have uses that effectively function as Powers (see below), but as possessions they still *also* count as resources — very potent indeed
      - other things like gold, company shares, or a stockpile of scarce resources are more obvious forms of wealth that can put you in a position of power over others, especially in a capitalistic or feudalistic society
        - when appropriate, this grants a bonus factor to checks, or can be used to KISS dice for tasks
          - or if you have the 'wealth' capability then your capital asssets help determine your starting score, by effectively using them as collateral to take out loans to secure funding when you need it, without ever having to sell directly
      - in a post-scarcity setting, something like 'social credit' may replace traditional capital
      - every capital asset is more-or-less unique and nonfungible; so you can buy multiple houses, for example, but each house will be different
    - $It:$ Items — 1 $caps$
      - mundane gear, equipment, and kit, tools and weapons, special articles of clothing and outfits, armour and other panoply, supplies and sundry goods, personal effects, or simple cash money
      - itemized assets exist to highlight the most important things you own, the objects you hold dearest or rely upon regularly
      - as with other attributes they can grant an advantage factor for a check, *but they aren't required to make rolls*
      - your character is assumed to have the bare necessities to adequately fulfill their job roles, to fit into their society, and to have generally gotten as far as they have in life
        - so there is no need to specify every single bit of kit, trinket, and possession
      - your items can be lost, traded, or stolen, but equally new assets can be aquired by finding, buying, or stealing them in kind.
      - some items things are consumable, disposable, or otherwise *finite* — like medicines and poisons, alchemical reagents, certain tools, aummunitions, or magic and technological gizmos — they can grant you a temporary bonus effect or power, equivalent to a gambit feature, but may also have a limiting side-effect or two
        - if the item is something that should have an obviously finite number uses, then roll `2d6` when you aquire it and count the total as the amount of times you can use it before it runs out
        - if the item is more like a tool or gadget that could break with use, then roll `1d20` after each use and if you roll a 1 then the   
      - itemized assets can include just about any object not already covered by capital assets, so making up new ones is fairly simple
      - yes, if an item is listed in one of your archetypes then the discount lets you take *one* for free
        - that is, itemized assets are the only attribute that you can buy multiple times, so each subsequent purchase of the same item costs an additional +1 $cap$ (ie. the cost increases cumulatively)
    - $St:$ Standings — 3 $caps$
      - your inportance within or connections to organization, a repuation for something that makes you in/famous (and any powers or privlages that you recieve because of that notoriety), or anything else that might bring you prestige, influence, or clout
      - standing assets most commonly get you access to places or people than you would otherwise struggle to get, with no (or fewer) questions asked
        - they make you important with a given context or faction, and more likely to be listened to or taken seriously in certain social settings
        - or they might help you strike fear into your enemies if your repute makes you particularly domineering or dreadful
        - or if you have the 'links' capability then your standing asssets may help determine your starting score
  - **Features**
    - $As:$ Aesthetics — 1 $cap$
      - your fashion and style choices, parts of your personal or cognitive make-up, your cultural expressions or a stereotype you've embraced, or any unusual physical features or other identifying qualities that you posses
      - they are largely cosmetic, and function best as signposts to guides you to back to a neutral point for your character to help you roleplay them
        - especially after an interlude in gameplay, or if you're coming back to the game after a missed session or two
      - you don't need to buy every aesthetic that perfectly describes your character though
        - after all, you can describe them however you like in the circumstances portion of your character sheet
        - these attributes are just meant to include the highlights of your personality, or the most memorable aspects of your appearance if a stranger were to describe you
          - For example, maybe you think you're pretty short for your size, but you're not capital-s 'Short' unless you take it as an aesthetic attribute; then you're the *shortest* person around. Your actual physical height doesn't matter, it's just the impression you seem to give off.
      - if you are using Kismet (see below), then you can also earn Lots during the debrief of each session for portraying your asthetics well
      - aesthetics are just words — usually adjectives, or the adjective form of certain nouns, or a short descriptive sentence if a single word or two can't seem to encapsulate the concept — with dictionary definitions attached to remind you what they mean
        - they can also be interpreted literally, metaphorically, or poetically
        - so making up new ones on the fly is pretty easy
        - but be sure to only use one definition / interpretation when you add it to your sheet, if there are multiple, and then stick to it
      - and yes, if an aesthetic feature is listed in one of your archetypes then the discount lets you take it for free
    - $Lm:$ Limits — 0 $caps$
      - health conditions, injuries and scars (both mental and physical), phobias and obsessions, and vices or bad habits; and just about anything else that could hold a person back in life in some way
      - for checks, these limiting features may occasionally count as relative difficulty factors for rolls, if your FC remembers that you have them or if you or your peers kindly remind them
      - but for tasks, they can work quite differently:
        - they either *prevent* you from spending beats on certain consequences
        - or they *force* you to spend your first beats on a particular consequences before anything else
          - if you see that two or more limits conflict on a given task then let your peers choose the most appropriate
        - and the most severe limiting features can even *lower the rank* of an ability by one step
          - the rank below Bronze is called 'Copper' (Cp); it auto-fails on a 1-2 for checks, and only get beats on a 6 for tasks
      - on the surface, making up new limits on the fly may seem simple, since you could look up just about any medical condition you can think of and represent it with one
        - but health is a complicated science, and it can sometimes be difficult to respectfully roleplay a character with a particular condition if you don't know enough about it
        - rather, making new limiting features requires some time and research and then a careful condsideration of the ways in which what you've learned may hinder a character
          - the trick is not to double-up on effects; only choose the most direct or pertinent thing 
            - limits generally only affect one specific aspect of your character sheet at a time
          - and sometimes there's a counter-balance too; an unexpected up-side that hepds you out occassionaly
            - try not to get too mechanical with it though
            - not everything has a silver lining
      - also yes, if a limiting feature is listed in one of your archetypes then the discount means you actaully *gain* a $cap$ if you take it (ie. it costs -1 $cap$)
        - and yes, this also means that you could *theoretically* take every limiting feature in the game to handicap yourself as much as possible, but doing this probably isn't very fun and would slow down the game , so taking too many limits should not really pass peer review
          - 3 or 4 should be enough for most characters, unless they are really crucial to your concept
    - $Mr:$ Merits — 4 $caps$
      - delibrately bend or break the normal rules of play; may be via some supernatural potency, bestowed gifts or charms by a greater force, social or cultural powers, or from honed skill and great training
      - each gambit is somewhat unique, so you'll have to read their descriptions, but most have explicit conditions underwhich they can be used
        - usually when you do or say something specifc, or when something happens that allows you respond in a certain way
        - some can only be used once per session
        - others can be used every turn, but only in specific scenes or situations
        - some will make certain dice rolls explode
          - meaning that for every 6 you roll, roll another `D6` and the result on top of what's already been rolled
            - and any 6s they roll can explode too — potentially *ad infinitum!*
        - some can even temporarily *raise the rank* of an ability for specific rolls
          - though there is no rank higher than platinum.
        - and a scarce few are passively *always active*
      - they often have a catchy phrase as their name or title, which hepds to encapsulate or summarize them, along with their description and rules explanations
      - making up new gambit features is possible, but requires some careful thought and peer review, so harder to do on the fly than with other custom attributes
  - **Gambits**
    - $Ds:$ Disciplines — 2 $caps$
      - fields of study, subjects of particular interest to you, objects that you've trained to use properly, hobby projects, places or types of people you're overly familiar with, profficiencies and special methods, or just a certain aptitude or working knowledge you've garnered over time
      - disciplinary merits are quite diverse and may each be used in up to five ways:
        - they guarantee that you know how to safely interact with the creature, object, or place in question
        - they to allow you to easily point to a specialty while KISSing (see tasks)
        - they may act as a qualification for starting certain jobs
        - they let you remember things your character already knows about the topic, using a Resolve check
        - or they let you discover or establish new facts about the topic, using a Wits check
      - disciplines are just words — usually pluralized nouns or proper nouns — with explanations attached to remind you what they mean
        - so making up new ones on the fly is pretty easy
      - if you see a generic noun listed as a discipline with an underscore '_' on the end, then you should replace that with a proper noun specific to your game
        - for example, the discipline 'City_' should become 'London' when you add it to your sheet if your character lived or worked in or around London when they aquired that attribute
          - rather than interpreting that to mean a discipline for *all* cities
    - $Gn:$ Genetics — *Not for Sale*
      - these are innate attributes given to you *for free* at character assembly based on your species and heritage choices, they are either congenital or come naturally to you in some other capacity
        - so, in essence, the way to describe any playable creature in this game is just as a collection of genetic merits that all members of that species naturally share
          - or if you're not playing as a natural-born creature then you may also refer to these as 'synthetic' metrics
        - think of them as mainly as the things that disinguish or identify one species from another
          - they are *not* stereotypes about an ancestry or people
          - and should generally not be used to just give flat bonuses to specific abilities
      - in essence, they may resemble other existing attributes — in that they can guide the way your portray your character, grant special powers, be used to KISS dice, or perhaps even hinder you at times — but they are generally unique to your kind
      - they cannot be bought normally by anyone else with $caps$
        - though, under truely exceptional circumstances they may granted by powerful magics or advanced sciences, or lost via extreme bodily damage, disease, or other traumas
    - $Od:$ Oddities — 3 $caps$
      - attributes that do not fit into any other category
        - either because they are so complicated that they practically need their own subsystem to explain
        - or because they are so weird, specific, or rare that it doesn't make sense to group them with the other attributes
      - odd merits *always* need peer approval before they can be taken, and are rarely offered in archetypes
        - so they usually have to be bought for full price 
          - but this also makes them prime candidates for your special attributes, since that would makes them free instead (see below)
      - this is also where you'll find those attributes that permanently raise the ranks of your abilities by one
        - note that there is no rank higher than Platinum

##### special attribute
you may take any one attribute of any type *for free* as your 'special' attribute
  - all your other attributes are considered 'general' by contrast
    - no other other player character may take your special attribute as a general attribute
    - and similarly, you may not take the special attribute of another player character
    - if there is a disagreement about who gets to take which attribute, then each of you should make a pitch to your peers based on your character concept as to *why* the attribute should be uniquely yours and yours alone
      - and then put it to a vote, if you have to
  - your special attribute cannot be lost or removed by any means, unless you willingly discard or swap it
  - if you can't decide which attribute you want to be your special, then you may wait and see through play, or vote one on later

##### using attributes
  - for checks, any appropriate attribute for the action you're trying to perform (subject to peer review) may be added to your pool of up to four `+1d6` bonus factors
    - of which, you would choose the highest roll and then add it to your main `1d20` rresult
  - for tasks, an attribute may be used to name and justify your 'specialties' when KISSing, disciplines especially, allowing you to re-roll a die with it
  - but generally, every type of attribute already does its own thing; so the benefit to rolls from attributes is not overly great

##### under or over spending your caps
- if you have any $caps$ left over that either can't be spent on anything else, or you don't want to spend them on anything else, then you may take the 'Lucky' (Wd) attribute at the cost of those remaining points
- similarly, if there's an attribute that you absolutely must have, but can't quite seem to afford it, then you may take the 'Unlucky' (Wd) attribute to make up for those missing points.
- both attributes work in the same way, but as opposites:
  - when there's a chance that some some weird random event could happen, the FC might typically flip a coin or choose odds or evens and then roll a d6 (for 50/50 odds)
  - but if you have the Lucky or Unlucky then those odds start to lean in or out of your favour, resectively:
    - instead of a d6 or a coin, the FC rolls a d20
      - and adds the spare points you had if you are Lucky
      - or subtracts the points you owe if you are Unlucky
    - and sees if the total result is 11 or higher
    - this is a permanent effect, and happens every time, so long as you keep the attribute
- the maximum amount of caps you can under or over spend is ±8
  - and doing so either way requires your peer's permission 

#### earning new attributes
during development sessions *between* arcs the FC may call for a round-table discussion of everyone's playstyles and accomplishments, where your peers may vote for you to gain or lose new attributes:
  - they will each suggest a new attribute for you to gain (based on how you've portrayed your character thus far or what you've discovered through play), then move on to the next person at the table 
    - once you each have a list of potential attributes you could gain and you've had some time to think, go round the table again, and one-by-one make a pitch to your peers for each attribute they've suggested as to why you should gain it
      - you may veto any attributes that you *really don't like* at this stage, by simply not pitching them
      - then your peers should vote on which attribute they now think you should gain, based on your pitches
      - and the attribute with the most votes is then gained, or if there is a tie then you can choose which one you like best between the tying options
  - afterwards, go around the table again and make a pitch for any attributes you think you should *drop* entirely or *swap* for something different because you have not been playing them or because you feel they have shifted into something new
    - swapping attributes like this needs unianimous agreement to pass
    - whereas dropping attributes only needs a majority vote
  - such sessions are also when score and rank increases may be voted on

## 5. kith & kin
  - these are 'very important non-player characters' or VINPCs (pronounced /vɪn:pi:si/) that you have designated as being crucially interesting to your character or the story
    - they may be your family members, a lifelong friend, a lover or rival, a mentor, an animal companion or loyal steed, a business associate, your guardian or an aide, or whoever else you may think of who's life and objectives could be relevant to your own
  - you are limited to a maximum of 3 VINPCs in total, regardless of your tier
    - only the FC may raise or lower this limit, since they are the one that will most-likey have to design and portray them all
    - therefore, you must also discuss each one in detail with your FC
    - if you have no ideas about which characters may be important to you, don't worry
      - you can ask for an NPC you've met ingame to be designated as a VINPC during downtime or development sessions
      - similarly, a character whom you thought would be important may turn out not to be
        - it's ok to downgrade them back to being normal NPCs
  - you can also use your archetypes and circumstances to guide which sorts of NPCs you are most likely have relationships with
  - you can ask a VINPC for aid, if they're present in a given scene, but they usually won't give it freely
    - since their aid ties them to the consequences of your actions, VINPCs will most-likely try to trade favors with you over time
  - VINPCs have extra protections over normal NPCs, sometimes euphemistically called 'plot armor'
    - meaning that they cannot randomly die or be killed by another NPC without it being dramatically appropriate and without the express permission of the player who has taken them as a VINPC
    - but they are otherwise under complete control of the FC and will act like any other person in their world
      - that is, from an in-game perspective, none of these characters are aware in any way that they are special
        - it is a purely *meta* consideration

## 6. jobs
  - jobs don't always have to be a literal professional position or a trade that you ply, they can also simply refer to roles or responsibilities that you are capable of undertaking or fulfilling (and may be closer to groups of related skills, in that sense)
    - making up new jobs is possible, usually by taking the verb you want to perform and converting it to it's noun form
      - but sometimes there's a perfectly good noun that already exists that describes the job your thinking of, without needing to fiddle around with suffixes
      - and although every job should come with a short definition for clarity, the use-case of every job should be fairly self-explanatory
    - still, it's a good idea to try to design new jobs that don't overlap too much with existing ones
      - make sure you have a really clear idea about what each new job would do and what sorts of situations they might be used in
      - and to always run a new job you've invented past your peers before adding it to your sheet
    - some jobs have multiple titles, and are ordered alphabetically and separated by slashes
      - either because they are gender-specific, synonymous, or because they involve largely the same skillsets and perform similar activities to one another
      - regardless, they do not count as separate jobs, so just add the one you feel is most appropriate for your character (or all of the ones that overlap from your archetypes)
  - starting a job that's listed on any of your archetypes costs 1 $jip$ (job incrementation point)
    - starting any other job costs 2 $jips$ 
    - and all of the jobs that you see *listed more than once across all the archetypes you've taken* can be started for free
  - when you start a job, it's opening level is your *lowest score* of it's two inherited abilities
  - advancing any job level beyond it's starting value costs 1 $jip$ per level, regardless of whether it was listed on your archetypes or not
  - the maximum level a job can be advanced to is 8
    - though some attributes can boost your level, and these boosts can bring the *effective level* above an 8
      - but be sure to only apply such attributes once all your $jips$ have been spent
  - from then on jobs gain $exp$ (experience) as you use them in play
    - and the level advances by 1 when you accumulate enough $exp$ equal to twice the current level

## 6. principles — goals, habits, & creeds
- write about your character
- always discuss with your peers

#### Kismet (metacurrencies)
###### Lots
  - you can have up to 10 Lots at a time
    - Lots spent on chacks add `+1d6` to your pool of advantages
    - Lots spent on tasks let you KISS and reroll a die of your choice
    - one Lot can be spent per check to reroll too
    - you can earn a portion of your Lots back in the debreif every session by advocating for your portrayal of your character's aesthetic features and reflecting their choices throughout the session expressed via goals, habits, &/or creeds 
    - Lots earned during the debreif that would bring you above the maximum, 10, are converted into $exp$ to help you level up any skills of your choice
  - you start the game with `1d6` Lots

###### Ego
  - you either have Ego at any given time, or you don't
    - spending Ego either KISSes all the dice your want or counts all your 6s twice
    - Ego can't be spent on checks
    - earn back Ego from introducing your own scenes
  - flip a coin, or roll a die and call even or odds, to see if you'll start the game with Ego or not

---

## 8. Modular Character Aspects

#### capabilities (optional abilities)
  - capabilities function almost identically to abilities, except that:
    - they are *derived* from your current abilities and the answers given during a questionnaire
      - the rank of a capability is equal to the lowest rank of two other abilities
      - the score of a capability is equal to the number of questions you answer 'yes' to
        - answer the questions honestly, as they will be subject to peer review
    - they can only be used to perform checks, not tasks
      - often, failing a capability check takes a certain amount of agency away from your character for a brief time
      - that is, failing a capability check will always result in consequence that you or your Peers choose from a list and then you should react or roleplay appropriately
    - they are also completely optional / modular, and which ones you should use are heavily based on your game's current tone or themes
    - however, sticking to a theme is important so that the game doesn't get diluted, so you may only choose up to 3
      - decide as a group which ones you feel would be necessary or useful for your game
      - different PCs *can* each have different capabilities, but only if it makes sense...
        - that said, it's better to try to be consistent
      - since they are all derived, you can change out capabilities in a development session for new ones if your game theme has shifted
      - and re-derive them again when the theme shifts back
        - you may find you have different or new answers to the questions asked in the derivation process, and that's okay (arguably intentional)

###### *examples*
  - *Grit* (#violence, #combat, #war)
    - a measure of your general audacity and your readiness to injure others, your disposition
      - governs instinctual reactions in a fight
    - calculated by: Add Wits and Swiftness, divide by 4, + questionnaire answers
  - *Guts* (#violence, #combat, #mystery, #horror)
    - a measure of your physical and mental tolerance for putting yourself in harms way and potentially being injured, your mettle
      - governs how long you can keep up the fight (akin to HP)
    - calculated by: Add Endurance and Resolve, divide by 4, + questionnaire answers
  - *Wealth* (#feudalism, #commerce, #intrigue, #politics)
    - represents money management, investments, access to funds, etc. not for games where you want to track every penny 
      1. someone else's property; a vagrant; a fugative; an untouchable
      2. living beneath the poverty line; an indentured servant; or just down on your luck 
      3. living within your means; free but poor; living a nomadic lifestyle; or caged in comfort 
      4. starting to turn a profit; an apprentice; a student; a hustler; or a seasonal-soldier
      5. enough savings for emergencies an special occasions; a guild-member; an itinerant trader; or a mercenary
      6. full records, insurance, and regular savings; a master artisan; a residential merchant; or a professional-soldier
      7. an aristocrat living off inheritance, investments, or exploitation; a superintendent; a guild-master; a knight; or a criminal kingpin
      8. one born into wealth and sworn to fealty; lesser nobility; a viceroy; a chancellor; or robber-baron
      9. a true blue-blood; greater nobility; practically sovereign; a warlord or dictator; or the cheif executive of a merchantile empire
    - calculated by: Peer decision based on circumstances, archetypes, and questionnaire answers
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

###### custom capabilities
  - all of the above are just suggestions
  - if you don't like the names of some of the capabilities above you can, of course, change them for your group or your setting
    - the capabilities section of the character sheet has 3 blank spaces, for this reason, so you can write-in whatever you like
    - just so long as you're consistent
  - or if want to make your own to suit your game's specific themes you can do so easily:
    - make sure that the capability is something you can only perform checks with, typically as a reaction or something for which there are only a limited number of responses if you fail
      - otherwise it might be better suited to being a custom job with some special requirements or usage conditions
    - list of an ability or two to base the rank of the derived capability on
      - do not make a compound capability derived from another capability
    - think of up to 8 'yes-or-no'-questions and use the player's 'yes' answers to generate the score
    - test out the capability through play, if you don't like it then you can tweak how it's used during development sessions

##### *NPC capabilities*
  - npcs generally don't roll dice (or don't perform tasks, at least)
  - so the npcs need a few extra capabilities that player characters don't, in order to set the difficulty for opposing rolls:
    - or do they...?


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


| Skill           | Level | $exp$                        | Ties            |
| --------------- | :---: | ---------------------------- | --------------- |
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
