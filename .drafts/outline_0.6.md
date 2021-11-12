---
Last updated: Monday 2021-07-19 @ 20:01:06 (UTC+01:00)

---

# Contents

-   [[#design goals|design goals]]
-   [[#0. concept|0. concept]]
-   [[#1. circumstances|1. circumstances]]
    -   [[#_names_|_names_]]
    -   [[#tier|tier]]
    -   [[#background|background]]
    -   [[#size|size]]
    -   [[#foreground|foreground]]
    -   [[#age|age]]
-   [[#2. Life-Paths and $caps$|2. Life-Paths and $caps$]]
-   [[#3. abilties|3. abilties]]
    -   [[#grade vs. Score|grade vs. Score]]
-   [[#4. features (traits & gambits)|4. features (traits & gambits)]]
    -   [[#traits = 2 $caps$|traits = 2 $caps$]]
    -   [[#gambits = 4 $caps$|gambits = 4 $caps$]]
        -   [[#special feature|special feature]]
        -   [[#innate features|innate features]]
        -   [[#earning new features|earning new features]]
-   [[#5. kith & kin|5. kith & kin]]
-   [[#6. jobs and skills|6. jobs and skills]]
    -   [[#levelling up jobs (failure bookeeping = $exp$)|levelling up jobs (failure bookeeping = $exp$)]]
        -   [[#learning new jobs|learning new jobs]]
    -   [[#$Sp:$ skills — 2 $caps$|$Sp:$ skills — 2 $caps$]]
-   [[#7. Assets|7. Assets]]
    -   [[#worth|worth]]
-   [[#8. principles — goals, habits, & creeds|8. principles — goals, habits, & creeds]]
    -   [[#Kismet (metacurrencies)|Kismet (metacurrencies)]]
-   [[#9. Modular Character Aspects [UNFINISHED]|9. Modular Character Aspects [UNFINISHED]]]
    -   [[#capabilities (optional abilities)|capabilities (optional abilities)]]
    -   [[#_examples_|_examples_]]
    -   [[#custom capabilities|custom capabilities]]
    -   [[#_NPC capabilities_|_NPC capabilities_]]
    -   [[#(mars)|(mars)]]

<!--GOALS-->

## design goals

-   make a game that I want to play
    -   versatile and scalable to most settings / situations (but especially my own worldbuilding project)
        -   will require frontloading the character assembly process
        -   but then the crunch for actual gameplay should be relatively low
    -   focus on different types of conflict resolution or presenting actions with interesting choices resulting in memorable storytelling / narrative experiences
    -   modular subsystems
        -   modular character assembly sections
        -   even the enire 'tasks' system may be modular (playtest this first!)
    -   free and open source! anyone can contribute
-   avoid making direct references to other ttrpg games and / or buzzwords
    -   or at least the proprietary ones
    -   linking to other creative commons resources is probably fine
-   play-test often, every two weeks if possible
    -   and get the first public release out within a month or two
    -   05/06/21 update: this goal has so-far failed, public interest in the game is currently _low_
-   stream parts of the creation process at least once per week
    -   (and make the VODs creative commons too)
    -   update: streaming is unlikely to happen because it makes me too anxious, but I will try to keep making update videos / devlogs
-   core mechanics, in one sentence each:
    -   narrative / descriptive focus
    -   two resolution mechanics:
        -   {standard d20 + bonus + choose highest d6 of advantages} > target = binary success
        -   {D6 dice pool} count successes and spend them on consequences = variable resolution
    -   path character generation, implicitly tells story of characters life and setting
    -   six abilities, each with two stats that separately determine skill and talent
        -   _optional:_ up to three sub-abilities (ie. capabilities) that can be theme / setting / tone specific and which can be interchaged and re-derived at any time
    -   point-buy score and feature distribution during character creation (determined by paths)
    -   qualitative character aspects (ie. features) which are not easily comparable to one another
    -   quantitative advancement system (ie. jobs) which level up with use, counting failed tasks as exp
    -   tag-based gear and items system, again focusing on qualitative aspects over quantitative stats
    -   players can wager metacurrencies during play for bonuses, and earn them back via good roleplaying
    -   potential for future development of subsystems

---

# game structure stuff / core philosophies:

<!-- parts of the markdown files should be commented in FULL CAPS for ease of Ctrl+F searching -->

-   section titles are shorthands for the rules themselves
    -   general game terms are first introduced in **bold**, but aren't capitalized
        -   specific game terms are Capitalized
            -   FC and Peer are also capitalized
        -   some terms are also shortened, with most vowels removed and using a $spcl$ $fnt$ to make them easier to pick out
            -   this font is also used for mathematical expressions and calculations
            -   (though this LaTeX font doesn't display on some markdown printouts)
        -   a `monospace font` is used for changable game figures, indicating when to roll dice and what modifiers to add
            -   small case `d` is used for Checks (roll-above) and rolling on random tables
            -   upper case `D` is used for Tasks (pool-based successes) and only refers to D6s
        -   use American spellings and use natural (or even casual) language
        -   _this document_ is written in an outlining style
            -   where sub-bullets add additional thoughts to the main bullet
                -   and sub-sub-bullets add more clarity
                    -   and so on...
-   speak to the reader: always use second person pronoun, 'you'
    -   let context determine whether 'you' means the FC, a player, or their character
-   **campaign** structure terms:
    -   campaigns (1-3 major arcs = 30-100 sessions)
    -   major arcs (1-3 minor arcs = 10-30 sessions)
    -   minor arcs (1-3 chapters = 3-9 sessions)
    -   chapters (1-3 sessions)
-   **session** structure terms:
    -   normal session segments
        -   preamble
        -   (game)play
        -   meta(game)
        -   debriefing
    -   downtime sessions
        -   used to pass in-game time quickly (weeks, months, years)
        -   spend lots to have brief role-play scenes and earn $exp$ in a related skill
    -   solo sessions
    -   development sessions
        -   "session 0"
        -   character assembly / development
            -   allows for re-jigging your character, changing some $caps$ or advancing to a new tier
        -   worldbuilding
    -   anyone can ask for any kind of session in advance, but the assumed default is a normal session
-   **scene** structure terms:
    -   scene types
        -   encounters
        -   interludes
        -   vingnettes
    -   rounds start with the FC's turn and then always progress clockwise
        -   (or left-to-right / top-to-bottom if playing online)
    -   once a round passes where no one has anything else to add (or skips their turn) then the scene ends
    -   any player (including the FC) can also use [script change tools](https://briebeau.com/thoughty/script-change/) to pause, speedup, slowdown, or _even rewind_ play
        -   other consent tools will also be provided, such as a checklist of content warnings
   
-   two types of **roll**:
    -   **checks** (simple verbs / actions)
        -   straight-forward, quick and dirty, binary outcomes
        -   target number based success criteria, roll with `1d20 + X + h(Yd6)`
            -   **target** = absolute difficulty (0-5) $\times$ 5 + relative difficulty factors, up to +4 (ie. target spreads are 0-4, 5-9, 10-14, 15-19, 20-24, or 25-29)
            -   **result** = `1d20` die roll + appropriate ability score `+X` (chosen by the FC) + the highest roll `+h()` of `Yd6`, where `Y` is the sum of any appropriate (ie. Peer reviewed) bonus factors from your features, spent lots, or aid.
                -   no autopass for Bronze, 20s for Silver, and 19-20s for Gold and Platinum
                    -   but also Platinum can't autofail on a 1.
            -   check success = get result equal to or higher than target
                -   margin of success or failure does not matter
                -   there is no inherent notion of a 'critial'
                -   you will not automatically fail on a natural 1
    -   **tasks** (complex verbs / skills)
        -   complicated, slow but clean, potential for marginal outcomes
        -   pool based success criterions, roll with `(X+Y)D6 > W`
            -   primary threshold = 1 + up to 4 relative difficulty factors (ie. threshold spread = 1-5)
            -   pool size = job level `X` + up to 2 aiding dice `Y`
                -   (aiding dice are rolled by the allies themselves, because their grade counts separatately)
            -   total successes = pass target per die depends on ability grade (chosen by the FC):
                -   Bronze = 5s and 6s only, Silver = 4-6, Gold = 3-6, Platinum = 2-6
            -   KISS individual dice to reroll them: using kismet, insight, stunts, or skills.
                -   use ego to double-count all 6s rolled (ie. each 6 counts as a pass twice)
            -   task success = spend successes on primary threshold
                -   spend other successes on secondary or tertiary consequences
                    -   secondary things prevent the FC from invoking their opposite against you
                    -   tertiary things modify an already bought primary or secondary consequence, or a failure consequence
                        -   but grant addition rewards such as exp, lots, or items
    -   this means players only need a handful of D6's and a d20 to play — which most ttrpg people _already have_
        -   so the proprietary elements / barriers to entry are kept reletively low
        -   theoretically you could even drop the d20 and use `3d6`
            -   but you'd get a more bell-shaped spread
            -   and I don't want to cause confusion as to the distinction between checks and tasks
-   it's easier to do addition than it is to subtract
    -   bonuses should always add to your dice or roll
    -   penalties should always add to the difficulty
        -   only _execptional_ features or subsystems, should break these heuristics
-   similarly, division is hard, so no all numbers used should be integers
    -   if a calculation results in a fractional amount then _always round down_
-   a target is what you aim for, don't shoot blind
    -   always tell the players what the target / difficulty is before rolling
-   always set stakes, and be clear about failure conditions
    -   set narrative stakes
    -   failing better (not always failing forward)
    -   players can offer potential failure solutions
        -   and can narrate both their successes and their failings, if they want to
-   _"Say 'yes' or roll the dice"_ ~ Vincent Baker
    -   avoid re-rolling without changing the stakes
-   your **FC** refers to the Facilitator ('referee' and 'game manager' are also acceptable)
    -   the FC is not necessarily in a position of power over the other players
        -   it should even be possible to play without a FC, but this will not be covered
-   your **Peers** refers to all the other players at the table except you
    -   the Peer is a relative term, each player's Peer is different
        -   and the FC's Peers are all the other players
    -   _all_ players are expected to adjudicate the game rules, not just the FC
    -   rules can be changed, broken, or removed by _any_ player (including the FC) at any time
        -   but only with permission from that player's Peer
    -   if something is said to require 'Peer review' then it offers a a moment to open the discussion up to the whole table
-   let players direct/frame scenes!
    -   and reward them with Ego
-   the FC never rolls (or at least never performs tasks)
    -   players roll to attack to strike their enemies, and roll to dodge to avoid them
-   the FC has princicples too
    -   similar to the player characters, the FC may write 'meta-goals', 'meta-habits', and 'meta-creeds'
    -   these are tools to help them structure the game and keep a level head
-   all mechanics are abstract representations of reality
-   common sense vs. suspension of disbelief
    -   there's probably a discussion here, but let's ignore that for now
-   rulings not rules
-   everything is relative
    -   time, distances, difficulties
-   no half measures, no sitting in the middle of the road
    -   when categorising things, there is no 'medium' option, all indexes are from 1 to 4 (or 0 to 5), and we try to use natural language that explains them without needing to look anything up. eg:
        -   playable sizes are 1 Small, 2 Modest, 3 Ample, 4 Large
        -   adult ages are 1 Young, 2 Mature, 3 Seasoned, 4 Old
        -   distances are close, near, far, and remote
-   (nearly) everything is modular
    -   core game engine [venus] will be `CC BY 4.0` (free cultural work)
    -   everything else [evening_star] will be `CC0` (public domain)
        -   this means anyone who wants to make content for the game can do so, and sell it if they want
        -   but they must reference the venus engine in some way, and probably use it's branding, to bring a bit of unity to all the projects and to improve discoverability
    -   though both will be `All Rights Reserved` until the first major release
        -   just while I make sure I get the game I want to play before anyone else run off with it and does their own thing

---

<!--MVP-->

# minimum viable product / first play-test version

-   pre-made characters for the players, consisting of
    -   name, circumstances, path choices
    -   age, abilities, features, jobs
    -   VINPCs and essential items
    -   no capabilities (at least not for the first playtest)
-   checks _only_, no tasks? (not sure about this)
-   a roleplay heavy scenario
    -   potentially even PvP oriented
    -   current plan is to play a bunch of bronze age pirates (cf. sea peoples) undergoing a mutiny on their trireme
        -   this means players can't really escape from the situation anywhere, they have to deal with the problem at hand
        -   not sure whether to write it so that players vy for the captaincy, or whether it's framed so that they put their support behind different npcs?

---

<!--ASSEMBLY-->

# character assembly

## 0. concept

-   think about what kind of character you want to make given the setting and the tone of the game that your FC wants to run
    -   in some cases, your FC may wish to run several development sessions where you collaboratively world-build with the other players before you even begin to think about what sort of characters you'll each play
        -   this can be done purely improvisationally, or with the guidance of a proprietary worldbuilding game
    -   in other cases, your FC will be using a preestablished or well-recognised setting
        -   either one that they've made up themselves or run games in before; a setting that you all know and love from popular culture; or a game set in a part of Earth's real or alternative world history, or a shared imagined future
-   a good character concept is a single sentence or picture that sums up your idea for them
    -   the concept might initially be very out-of-focus or loaded with stereotypes, references, and tropes
    -   but that's okay because you don't need to write it down anywhere, you just spitball your ideas at first and see how your Peers react to them
    -   plus the rest of the character assembly process will determine how your character differs from those touchstones — and perhaps how they are still the same — until they are slowly brought forth into enough mental clarity that you feel comfortable and confident to protray them in game

## 1. circumstances

##### _names_

-   your character's name, alias, or title (and optionally, their pronouns)
    -   you can come back to this later if you can't think of a character name right at the beginning of assembly
    -   or you may even decide to change your name during play, either because of some in-game revelation, or because you simply don't think their current one suits them any more
-   and your own name, as a player, so the FC can tell who's who

#### tier

-   tier sets the approximate 'power level' for play, it determines a few major character aspects according to the table below
-   all players should make characters of the same tier, unless they have their Peer's permission
-   tier can only change during development sessions, and must be unanimously voted on by all players

|                   TIER: | CIVIC (lowest) | HEROIC (low) | MYTHIC (high) | DEIFIC (highest) |
| ----------------------: | :------------: | :----------: | :-----------: | :--------------: |
| № free grade Increases: |        1       |       5      |       8       |        10        |
|       Starting № paths: |        1       |       2      |       3       |         4        |

-   The civic tier represents fairly historically accurate characters acting in an assumedly normal world. It represents people like you and I, most likely, and nearly everyone else who has lived and died on Earth.
    -   Pop culture examples:
-   Heroic tier is for playing out believable tales about people who quest for glory or struggle to leave their mark on the annals of history, culture, or legend whose efforts may not have been really possible without either a story-teller's embellishments or a true touch of magic. You may also want to refer to this as the 'cinematic' tier, if your setting is more modern.
    -   Pop culture examples: The Fellowship of the Ring
-   The mythic tier is the place of gifted-rogues, warrior-poets, adventurer-prophets, philosopher-engineers, sorcerer-monarchs; where paranormal events occur regularly and legendary deeds may be performed with few questions asked.
    -   Pop culture examples: Conan the Barbarian, Xena: Warrior Princess, The Pandava Brothers, Gilgamesh and Enkidu
-   Characters in the epic tier may be exalted mortals, superheroes, spirits, demigods, or even minor deities or shards of an even greater being given mortal form. They are not omnipotent beings though, their actions still have consequences, and there is still room for them to grow and learn from the world.
    -   Pop culture examples: Rama and Krishna, Moses and Jesus, Thor, Loki,

#### background

-   list aspects of your character's life circumstances that you think are improbable or impossible to ever change after character assembly
    -   e.g. stock, species, ancestry, kin, people, roots, culture, hues, tones, values, patterns, etc.
-   or use the space to declare which parts of your character's inward identity or personality you have pre-determined and aren't interested in ever changing
-   your setting or your FC may provide you with options to take here which may or may not have specific mechanical effects.
    -   For example, some settings may want to differentiate between different playable species or cultures by giving out free 'innate' features and/or jobs
    -   The core engine makes no assumptions here though, and leaves this open for others to decide

###### size

-   most typically determined by species, ethnicity, diet, and age; it represents an approximate combination of your height, length, and weight
    -   for example, most adult humans on Earth are between 5 and 6 feet (150-180 cm) tall, so this puts them at a modest size; but a human child would be considered small or tiny.
    -   Meanwhile, tigers and horses are of ample size, and hippos would be considered large; despite generally being shorter than most humans at the shoulder, they are simply more massive than us once they reach maturity.
-   size is indexed from 1 to 4 as follows (with approximate metrics for Earth-like settings)
    1.  Small ~ 2-5" (90-150 cm) & less than a quintal
    2.  Modest ~ 5-6" (150-180 cm) & 90-250 lbs (40-110 kg)
    3.  Ample ~ 6-7" (180-210 cm) & 250-2200 lbs (110-1000 kg)
    4.  Large ~ 7-10" (210-300 cm) & more than a tonne
-   size usually has very little mechanical effect, but sometimes a difference in size between you and someone else may added as a relative factor — either as a penalty or a bonus — to your actions depending on what you're trying to do
-   (there are also some other unplayable sizes, typically reserved for animals and monsters, and which would require FC permission to play as because their size differences compared to everything else can create some unexpected inconveniencies)
    -   These include: tiny or miniscule, and giant, enormous, colossal, or immense.

#### foreground

-   list aspects of your character's life circumstances that you think could be open to change over time (changable during development sessions, or after certain choices or realizations made in play)
    -   e.g. religion, community, class, gender, physique, colors, shapes, body modifications, etc.
-   or use the space to highlight parts of your character's outward identity or appearance
    -   As with backgrounds, there may be options presented here by your setting or your FC which grant free features, assets, or jobs, but the core engine makes no assumptions

###### age

-   influences your starting ability score spread, and directly determines how many additional paths you may take.
    -   age is indexed from 1 to 4, for adults (and a rough approximate in human years):
        1.  Young characters get +2 MAsp, +4 PAsp, and 1-2 additional paths (ages 18-25)
        2.  Mature characters get +3 MAsp, +3 PAsp, and 3-4 additional paths (ages 26-39)
        3.  Seasoned characters get +4 MAsp, +2 PAsp, and 5-7 additional paths (ages 40-59)
        4.  Old characters get +2 MAsp, +1 PAsp, and 8-10 additional paths (ages 60-89)
-   (there are also two other _typically unplayable_ ages, '0. junior' or '5. senior', usually reserved for NPCs. These require Peer permission to play as since they are quite vulnerable and likely to be difficult to roleplay respectfully):
    -   0.  junior characters (children) get +1 MAsp, +2 PAsp, and 0-1 additional paths
    -   5.  senior characters (elders) get +1 MAsp, +0 PAsp, and 10+ additional paths

## 2. Life-Paths and $caps$

-   Life-Paths (or simply just 'Paths') represent roles or vocations that your character has fulfilled or pursued at various points throughout their life
    -   be they full occupations, periods of studentship, service, incarceration, or exile, snippets from your upbringing, or other walks of life
    -   they are generic but personalized archetypes; and step by step they implicitly tell the story of both your character's life so far and the settings they've lived in
        -   that said, the order that you take paths in does not need to be chronological
        -   but you _cannot_ take the same path multiple times
    -   some paths have prerequisites; such as being a specific age or tier, having certain features, being a member of a given social or economic class, or requiring that you walk a different path first
-   the number of paths you can take is determined by your tier and your age (starting paths + additional paths)
    -   you'll notice that the number of extra paths from your age is variable, this is because you should try to only take as many paths as you need to fulfill your character concept
    -   but this limit can also be raised by the FC if they feel the default limit is too punitive
-   paths have a name or a title, which you should write at the top of your character sheet as you take them
-   a path adds +1 to your ability score pool (or $sp$) by presenting either an 'MA', a 'PA', or a pair of specific abilities 'X/Y', or the word 'Any':
    -   MA and PA mean you can add +1 to any mental or physical ability of your choice, respectively
    -   a pair of abilities, such as 'App/Res', means you must choose one of those two abilities to add +1 to
    -   and 'Any' means that you add +1 to any ability you like
-   every path you take grants you +X $caps$ (character assembly points), which you spend in steps 5-7 of character assembly
-   under each path heading will be two lists to spend those points on:
    -   a numbered list of up to 6 features that you can purchase with a 1 $cap$ discount in step 5
        -   when you take the path, you should also roll a `d6` on this list to choose a single feature that you get _for free_
            -   if there are less than 6 features on the LP and you roll a number that isn't listed, or you roll the same feature that you already rolled on a different LP, then simply re-roll or choose which one you want
            -   this randomness is injected to make your character a bit more unique and to force you think about what the circumstances may have that lead to you picking up that feature — be it positive, or negative
    -   a bulleted list of jobs that you are allowed to start and level up for one $cap$ each in step 6
        -   any listed jobs that overlap with the lists of other paths you've taken may be automatically learned and started at your minimum job level
            -   that is, if you notice two or more paths offer you the same job, you may start it _for free_
-   there is also be a third, comma-separated, list of a few essential assets that you aquire for taking the path. _These are all free_.
    -   If there's any other assets you want which aren't listed you must buy them with $caps$.
-   you can make up new paths, but since the list of all available paths sort of implicitly describes the larger setting that you're playing in, the creation of new paths is left to your FC, or the designers of whatever pre-written setting you're using
    -   though you can of course suggest ideas to your FC and see if they can come up with anything on the spot
    -   guidelines for FCs and designers to help them make new paths are given in their own chapter / section (not written yet)

## 3. abilties

-   Mental abilities (MA)
    -   **Appeal** (`App`)
        -   mental grace, charisma, social prowess, artistic sentiment, and emotional senses
        -   used for: feigning ignorance, making a good first impression, offering ideas or trading goods, and pleading for help
    -   **Resolve** (`Res`)
        -   mental resilience, wisdom, patience, determination, memory retention, and temporal senses
        -   used for: counting, finding, mending, and building things, remembering information you should already know, and working long hours
    -   **Wits** (`Wit`)
        -   mental speed, intelligence, shrewdness, logical reasoning, instinct, and spatial senses
        -   used for: aiming projectiles, problem solving, identifying and inspecting things and making connections, and watching, listening, or reading
-   Physical abilities (PA)
    -   **Endurance** (`End`)
        -   physical resilience, constitution, stamina, vigour, and regular movement upkeep (aerobics)
        -   used for: long-distance walking or jogging, holding your breath, treading water, wrestling, and eating or drinking strange things
    -   **Finesse** (`Fin`)
        -   physical grace, dexterity, flexibility, style, coordination, and making delicate or balanced movements
        -   used for: hitting things with most weapons, balancing and stretching, landing and rolling safely, crawling and sneaking around, and escaping binds
    -   **Swiftness** (`Swi`)
        -   physical speed, strength, reflexes, alacrity, and bursts of quick movement speed (anaerobics)
        -   used for: dodging or parrying, throwing and catching things, jumping, pushing or pulling things around, and quick sprints

#### Grade vs. Score

_grade_ represents your potential to succeed as raw talent and luck, whereas _score_ (sometimes abbreviated as '+', since it's always positive) represents your training and growth

-   your grade depend primarily on your tier (see above), as all your abilities start at Bronze grade and then you may assign 1-10 free grade increases according to your tier
    -   these free grade increases cannot take more than one ability to Platinum grade without your FC's permission
-   grade can also increase by buying special features with your $caps$
    -   but they are expensive and are rarely offered in paths
-   at the end of each major story arc (ie. about once every 15-30 sessions), your Peers may discuss whether you deserve a grade increase in recognition of your character's achievements thus far
    -   and if you do, then you may choose which ability to allocate it to
-   grade affects the natural success range of your d20 roll for Checks, and determines the pass range for all the D6's in your dicepool for Tasks, as per the following table:

| grade Rating                       | Bronze $(Br)$ | Silver $(Si)$ | Gold $(Gl)$ | Platinum $(Pt)$ |
| ---------------------------------- | :-----------: | :-----------: | :---------: | :-------------: |
| Natural Success Range _for Checks_ |       NA      |       20      |    19-20    |      18-20      |
| Natural Success Chance _per d20_   |       0%      |       5%      |     10%     |       15%       |
| Success Range _for Tasks_          |      5-6      |      4-6      |     3-6     |       2-6       |
| Success Chance _per D6_            |      33%      |      50%      |     67%     |       83%       |

-   scores all start at +0 and have no theoretical maximum, but they will probably sit in the 1-3 range for most characters starting out
    -   FCs should discourage 'min-maxing' players, who want to dump all their points into one ability, by putting a soft cap on the maximum starting ability score
    -   increase scores by distributing the score pool $sp$ generated by your age and path choices (see above)
    -   after character assembly, ability scores can only change during development sessions
        -   at the end of each minor story arc (ie. about once every 5-10 sessions) and after some discussion, your Peers may vote on which of your abilities should advance by 1, based on what they think you have most commonly been using
        -   or when so much time passes that your age increase, then some of your scores may go up or down, which you may allocate yourself
-   scores are added to your Checks as a flat bonus, and are used in Tasks to determine your starting dice pool size

## 4. features (traits & gambits)

### traits $:2\ caps$

-   traits represent parts of your character's personal or cognitive make-up:
    -   physical or cosmetic features that make them stand out from a crowd;
    -   their cultural expressions and idiosyncrasies, or a stereotype they've embraced;
    -   a fresh wound or an old scar, an obsession, or a phobia, or some other trauma.
-   each trait can be used once per session to either earn kismet _during play_ by bringing them to bear in dramatically appropriate ways:
    -   **Representation:** Take pride in a trait, or play it earnestly in the moment.
        -   Roleplay, show off, or express the trait at the right time to get what you want, or use the trait to your advantage in some other fashion.
        -   You earn a lot at the end of your turn if:
            -   the trait leads to a new situation that wouldn't have otherwise happened;
            -   if you refuse aid on a roll because of the trait, and succeed anyway;
            -   or if the trait avoids a roll entirely that would have ordinarily been necessary.
    -   **Limitation:** Allow a trait to limit an ability.
        -   Before rolling dice for a task, explain how the trait limits the ability you're using, and then reduce it's grade by one step _for the rest of the scene_ (affecting both tasks and checks).
            -   So Platinum drops down to Gold, Gold becomes Silver, and Silver goes to Bronze.
            -   And the grade below Bronze is called 'Copper' (Cp): it only gets successes on a 6 for tasks, and automatically fails checks on a natural 2 or below for checks.
        -   You earn a lot at the end of that scene, once the affected ability returns to it's normal grade.
    -   **Comedy:** Use a trait to do something funny or cause a scene.
        -   You earn Ego if this makes all the other players at the table burst out laughing, even if the characters in the game don't find it so amusing.
            -   It doesn't count if it's just an out-of-game joke.
            -   But it does keep counting every session you do it, as long as the majority of your Peers still find it funny.
        -   If you already have Ego then earn a Lot instead.
    -   **Tragedy:** Let a trait be the cause of your failure or refuse to even try.
        -   You earn Ego by failing a task willingly before rolling any dice and blaming the appropriate trait.
            -   _why would you do this?_
                -   because failing can be fun too sometimes, but being rewarded for it makes the consequences of failure string a little less.
                -   but whether this is a purely _meta_ consideration, or whether your character is genuinely sabotaging themselves is up to you.
            -   also, you may not "roll the dice anyway just to see what would have happened", because this can slow the game down and ruin the integrity of your commitment to the failure

it's possible that multiple of these criteria may be equally valid to invoke for a trait at a given moment, but in such cases still only one Lot or Ego is awarded.

### gambits $:4\ caps$

-   these are features which delibrately bend or break the normal rules of play:
    -   maybe via some supernatural potency;
    -   gifts or charms bestowed by genetic luck or a greater force;
    -   an innate knack for doing something, or a special trick that you learned over time;
    -   or social or cultural powers that go beyond mere wealth and prestige;
-   each gambit is somewhat unique, so you'll have to read their descriptions, but most have explicit conditions underwhich they can be used:
    -   usually when you do or say something specific, or when something happens that allows you respond in a certain way
    -   most can be used every turn, so long as all the conditions are met
    -   others can only be used once per session, but have less specific triggers
    -   some can raise your effective level for specifc jobs or abilties
    -   some can make your dice rolls explode
        -   meaning that for every 6 you roll, roll another die and add the result on top of what's already been rolled
            -   and any 6s they roll can explode too — potentially _ad infinitum!_
    -   some simply work with no dice rolls needed
    -   and a scarce few are passively _always active_ or grant you special access to a separate subsystem, like a spellcasting mechanic
        -   these are always written separately, and won't be included in the feature description itself to avoid bloating the features chapter
-   they often have a catchy phrase as their name or title, which helps to encapsulate or summarize them, along with their description and rules explanations
-   making up new gambit features is possible, but requires some careful thought and Peer review, so is harder to do on the fly than with traits or skills
-   all gambits cost 4 caps, but some are locked based on your tier.
    -   For example: If you are civic tier you can only buy civic gambits, but if you're mythic tier then you can buy mythic, heroic, and civic gambits.
    -   because they all cost the same amount though, there are no 'better versions' of the same gambits at higher tiers, just different powers and effects.

##### special feature

in addition to the free features you get from paths, you may take any one feature of any type _for free_ as your 'special' feature

-   all your other features are considered 'general' by contrast
-   no other other player character may take your special feature as a general feature
    -   and similarly, you may not take the special feature of another player character
-   if there is a disagreement about who gets to take which feature as their special, then each of you should make a pitch to your Peers based on your character concept as to _why_ the feature should be uniquely yours and yours alone
    -   and then put it to a vote, if you have to
-   your special feature cannot be lost or removed by any means, unless you willingly discard or swap it
-   if you can't decide which feature you want to be your special, then you may wait and see through play, or vote on one later (see below)
-   with your FCs permission, your Special ccould potentially be an Asset instead, like a rare artefact that you've inherited, or a piece of information you've sworn to secrecy, or some other plot device

##### innate features

as mentioned in step 1, some settings or FCs may offer you some free features or starting jobs because of your species or culture. Most commonly this would be language skills (see example above), but can be anything deemed appropriate really, for example, all humans in an assumedly Earth-like setting:

-   learn their native language almost without even trying, just by growing up around other native speakers and hearing them talk and trying to talk back
-   are generally furless, and thus have to make and wear clothes to keep warm; but can also sweat, which makes them better at running long distances
-   are seemingly better at throwing things than any other animal because of their specialized shoulder muscles and joints
-   have very dexterous fingers, allowing them to manipulate objects and craft tools more easily than other animals
-   and have well-developed social responses, including blushing, laughing, and crying, making macro-emotions easy to read

Some, all, _or none_ of the above may be things that you care to represent in humans with innate features. But contrast is the key. If there are no non-humanoid playable species in your setting, then it probably isn't worth trying to make differentiations like these. Focus on the differing cultures and subcultures instead.

#### earning new features

during development sessions _between_ arcs (about every 10-15 sessions) the FC may call for a round-table discussion of everyone's playstyles and accomplishments, where your Peers may vote for you to gain or lose new features:

-   they will each suggest a new feature for you to gain (based on how you've portrayed your character thus far or what you've discovered through play), then move on to the next person at the table
    -   once you each have a list of potential features you could gain and you've had some time to think, go round the table again, and one-by-one make a pitch to your Peers for each feature they've suggested as to why you should gain it
        -   you may veto any features that you _really don't like_ at this stage, by simply not pitching them
        -   then your Peers should vote 'yes' or 'no' to each feature they now think you should gain, based on your pitches
        -   and the feature with the most 'yes' votes is then gained, or if there is a tie then you can choose which one you like best between the tying options
-   afterwards, go around the table again and make a pitch for any features you think you should _drop_ entirely or _swap_ for something different because you have not been playing them or because you feel they have shifted into something new
    -   swapping features like this needs unianimous agreement to pass
    -   whereas dropping features only needs a majority win
-   such sessions are also when ability grade and score increases may be voted on

## 5. kith & kin

-   these are 'very important non-player characters' or VINPCs (pronounced `/vɪn:pi:si/`) that you have designated as being crucially interesting to your character or the story
    -   they may be your family members, a lifelong friend, a lover or rival, a mentor, an animal companion or loyal steed, a business associate, your guardian or an aide, or whoever else you may think of who's life and objectives could be relevant to your own
-   you are limited to a maximum of _three_ VINPCs in total, regardless of your tier
    -   only the FC may raise this limit, since they are the one that will most-likey have to design and portray them all
    -   therefore, you must also discuss each one in detail with your FC
    -   if you have no ideas about which characters may be important to you, don't worry
        -   you can ask for an NPC you've met ingame to be designated as a VINPC during downtime or development sessions
        -   similarly, a character whom you thought would be important may turn out not to be
            -   it's ok to downgrade them back to being normal NPCs
-   you can also use your paths and circumstances to guide which sorts of NPCs you are most likely have relationships with
-   VINPCs cannot randomly die or be killed by another NPC without it being dramatically appropriate and without the express permission of the player who has taken them as a VINPC
    -   but they are otherwise under complete control of the FC and will act like any other person in their world
        -   that is, from an in-game perspective, none of these characters are aware in any way that they are special
            -   it is a purely _meta_ consideration
-   you can ask a VINPC for aid, if they're present in a given scene, but they usually won't give it freely
    -   since their aid ties them to the consequences of your actions, VINPCs will most-likely try to trade favors with you over time
    -   in fact, every VINPC slot has a checkbox that you can use to determine whether they currently owe you a favor or not
        -   when this is not filled, you must help them in return for their favor again, or you must otherwise persuade them, before they will want to aid you again
            -   this doesn't always have to be a roll
                -   the FC may be explicit about what they think would give you their favor again
                -   but whenever you do something for them feel free to also ask the FC if this gives them favor again
        -   filp a coin, or roll a d6 and count evens or odds, to determine at the start of the game to find out whether you begin with favor with each of your VINPCs
            -   whether you do, or do not, tell us why?
                -   ie. make up a story, then and there
            -   this is just grist for roleplaying
                -   but may also help the FC to run these characters right at the start of the game

## 6. jobs and skills

-   jobs don't always have to be a literal professional position, or a trade that you ply, they can simply refer to roles or responsibilities that you are capable of undertaking or fulfilling (and may be closer to 'skill sets', in that sense, but 'jobs' is a more snappy moniker)
    -   making up new jobs is possible, usually by taking the verb you want to perform and converting it to it's noun form
        -   but sometimes there's a perfectly good noun that already exists that describes the job your thinking of, without needing to fiddle around with suffixes
        -   and although every job should come with a short definition for clarity, written in the present tense, the use-case of every job should be fairly self-explanatory
    -   still, it's a good idea to try to design new jobs that don't overlap too much with existing ones
        -   make sure you have a really clear idea about what each new job would do and what sorts of situations they might be used in
        -   and to always run a new job you've invented past your Peers before adding it to your sheet
    -   jobs have one or more labels, which help you to organize and search for them by category or sector
-   starting a job that's listed on any of your paths costs 1 $cap$
    -   starting any other job costs 2 $caps$
    -   and all of the jobs that you see _listed more than once across all the paths you've taken_ can be started for free
-   when you start a new job, it's starting level is equal your minimum job level (determined by your tier).
-   advancing any job level beyond it's starting value costs 1 $cap$ per level, regardless of whether it was listed on your paths or not
-   the maximum level a job can be advanced to is 6
    -   though some features can boost your level, and these boosts can bring the _effective level_ above an 8
        -   but be sure to only apply such features once all your $caps$ have been spent
-   from then on jobs gain $exp$ (experience points) as you use them in play (see tasks rules)
    -   and the level advances by 1 when you accumulate enough $exp$ equal to _twice_ the current level
-   if your tier raises through play, then your minimum job level will increase also
    -   thus all jobs that you had that were still at your previous minimum automatically raise to the new minimum, without needing to accumulate more exp for them

### levelling up jobs (failure bookeeping = $exp$)

-   twice the level of the job is the number of tasks you must _fail_ with that job to level it up
    -   ie. you only learn from your mistakes
-   levelling the job happens immediately after the last task is failed
    -   (or as soon as you notice that the exp bar has been filled sometime thereafter)
-   every time you level up a job, the $exp$ slate is wiped clean for that job
    -   e.g. level 4 job requires 8 failed tasks to become level 5, then it needs 10 new failures to reach level 6
-   6 is the soft level cap for all jobs
    -   the only way to advance above 6 in a job is with the aid of a gambit, supernatural training, or the used of advanced magics or technologies
-   you can also earn bonus exp by spending excess lots above 10 at the end of a chapter
    -   and from spending lots to generate scenes during downtime
-   abilities level up by faltering on your creeds and a vote by your Peers (see above)

#### learning new jobs

when enter a situation where you would need to perform a task but don't have the right job

-   add the new job to your sheet at 'level 0'
    -   then take the ability designated by the FC for the task and use it's grade, as per usual, but then take it's _score_ aswell instead of the job level to determine how many dice you roll
-   mark an additional $exp$ for _all_ tasks made at level 0 (regardless of success or failure)
-   once the exp bar is filled up completely (10 checks total), the newly learned job then advances to level 1
-   you cannot use a level 0 job to offer aid

### skills $:2\ caps$

fields of study, disciplines, subjects of particular interest to you, specialist training you've recieved, hobby projects, places or types of people you're overly familiar with, profficiencies and special methods, or just a certain aptitude or working knowledge you've garnered over time

-   skills are quite diverse and may each be used in up to four ways:
    -   you may KISS with them, to get bonus dice or rerolls
    -   they guarantee that you know how to safely interact with the creature, object, or place in question
        -   includes speaking other languages or understanding local dialects with relative proficiency
    -   they let you remember things your character should already know about the topic, using a Resolve check
    -   or they let you discover or establish new facts about the topic, using a Wits check
-   you will find that on every job description there is also a list of 'suggested skills'
    -   these are, as the name suggests, only suggestions
    -   but they should give you a better idea of how certain skills can overlap on multiple jobs
    -   the 'Berries' skill, for example, could be applicable the 'Baker', 'Forager', and 'Herbalist' jobs, or any other tasks that may need to draw on your special knowledge of different kinds of berries and their uses
-   skills are just words — usually pluralized nouns or proper nouns — with short explanations attached to remind you what they mean
    -   so making up new ones on the fly is pretty easy
-   if you see a generic noun listed as a skill in lower-case between square-brackets '[like this]', then you should replace that with a proper noun specific to your character and setting when you take it
    -   for example, the skill '[city]' should become 'London' when you add it to your sheet if your character lived or worked in or around London when they aquired that feature
        -   rather than interpreting that to mean a skill for _all_ cities
    -   or the skill '[language]' should turn into a named language of your choice, such as 'English', 'Malay', or 'Swahili', or whatever setting-appropriate language you like
        -   nb. a language skill can't be applied to every instance in which you speak or use that language, only the times when complex vocabulary is used or when the nature of the language itself is relevant in some way
-   you learn a new skill every time you learn a new job (ie. advancing from level 0 to 1)
    -   the skill you learn must be relevant to that job
-   during character creation you can also buy extra skills for 2 $caps$ per skill.
-   you can also learn new a new skill every time there's an extended period of downtime of at least one in-game season
    -   by spending Ego and having a miniature scene or montage about how you learned the new skill
    -   this is similar to spending Lots on $exp$ in downtime, but can effectively only be done once per downtime session because there's no way to regenerate Ego during downtime

## 7. Assets

assets come in three types: capital, reputable, and vendible. (the price listings in $caps$ are only for if you wish to buy an asset that isn't listed in a path, since all the assets listed in your paths are free).

-   $CA:$ Capital Assets — 4 $caps$
    -   property and real estate, great fortunes or inheritances, stocks and bonds, vehicles and machines, fine art and furniture, rare artefacts and treasures, livestock, or other large quantities of wealth or stores of value that are not easily transferable
    -   capital assets typically have a physical use: for example, buildings can be lived in, land can be worked, ships and trains can transport people or things, magical swords can slay monsters, and art can be used as tax write-offs
        -   in all of these cases, the usefulness of the item in question should be fairly implicit or else come with a description or explanation
            -   in the case of magical items, rare artefacts, and advanced technologies, they may _themselves_ have uses that effectively function as Gambits, but as possessions they still _also_ count as capital — very useful indeed
    -   other things like precious metals, company shares, or stockpiles of scarce resources are more obvious forms of wealth that can put you in a position of power over others, especially in a capitalistic or feudalistic society
        -   when appropriate, this grants a bonus factor to checks, or can be used to KISS dice for tasks
            -   or if you have the 'wealth' capability then your capital asssets help determine your starting level, by effectively using them as collateral to take out loans to secure funding when you need it, without ever having to sell directly
    -   in a post-scarcity setting, something like 'social credit' may replace traditional capital
    -   most capital assets are more-or-less unique and non-fungible
        -   so you can buy multiple houses, for example, but each house will be different
            -   (and one generally can't combine two houses together into a bigger more valuable house)
-   $RA:$ Reputable Assets — 2 $caps$
    -   the people you know, your inportance within an organization, a repuation for something that makes you in/famous (and any powers or privlages that you recieve because of that notoriety), your public image, or anything else that might bring you renown, influence, or clout
    -   these features most commonly grant you access to places or people than you would otherwise struggle to get, with no (or fewer) questions asked
        -   they make you important with a given culture or faction, and thus more likely to be listened to or taken seriously in the right settings
        -   or they might help you strike fear into your enemies if your repute makes you particularly domineering or dreadful
        -   or if you have the 'links' capability then these features help determine your starting score
-   $VA:$ Vendible Assets — 1 $caps$
    -   mundane gear, equipment, and kit, tools and weapons, special articles of clothing and outfits, armour and other panoply, supplies and sundry goods, personal effects, or simple cash money
    -   vendible assets exist to highlight the most important things you own, the belongings that you hold dearest or rely upon most regularly
    -   your character is assumed to have the bare necessities to adequately fulfill their job roles, to fit into their society, and to have generally gotten as far as they have in life
        -   so there is no need to specify every single bit of kit, trinket, and possession
    -   your items can be lost, traded, or stolen, but equally new assets can be aquired by finding, buying, or stealing them in kind.
    -   some items are consumable, disposable, or otherwise _finite_ — like medicines and poisons, alchemical reagents, certain tools, special ammunitions, or magical / technological gizmos — they can grant you a temporary bonus effect or power, equivalent to a Gambit, but may also have a Limiting side-effect or two
        -   if the item is something that should have an obviously finite number uses, then roll `2d6` when you aquire it and count the total as the amount of times you can use it before it runs out
        -   if the item is more like a tool or gadget that could break with use, then roll `1d20` after each use and if you roll a 1 then it's breaks and needs repairing or gets completely destroyed.
    -   venible assets can include just about any object not already covered by capital assets, so making up new ones is fairly simple

most vendible assets have tags, which are qualititative properties or descriptive lables that have no strict mechanical effect, but act more as a way to flag how they should or can be used, or how those uses could be interpreted by your Peers. Certain tags may also make an item more or less attractive to certain buyers.

Examples tags include: tool, weapon, armor, shield, great, magic, high-tech, complex, reputed, heavy, bulky, consumable, delicate, disposable, cursed, ancient, cute, ugly, fungible, living, misc, etc.

#### value

The main difference between venible and capital assets when it comes to trying to sell them is in finding a buyer. Most traders will accept vendible goods, but capital assets require specialist traders or brokers to liquidate into cash.

asset has an evaluation in dice called it's 'worth'

-   out of game, each asset's worth is evalutated by a number of dice and their grade (eg. 1Br, 2Si, 3Gl, 1Pl, 5Cp, etc.)
    -   here, the use of grade is mainly meant to be representative of an order of magnitude of greater value
        -   so a 5-Gl asset is equivalent in worth to a 10$^S_l$ asset, for example
        -   but it also has a mechanical purpose if you use the optional monetary subsystem
-   in game, the worth represents the value of asset in whatever currency is appropriate or accepted as legal tender in your setting, if it were to be liquidated into cash
    -   or in the case of literal cash, it's the actual purchasing power of that money
-   if the asset is fungible then it's worth can be _multiplied-down_ into fewer dice of a higher grade, or _divided-up_ into more dice of a lower grade, as per the following table:

| Denomination |  Cp |  Br |  Si |  Gl |  Pt |
| :----------: | :-: | :-: | :-: | :-: | :-: |
|  $1Br = 2Cp$ |  2  |  1  |  —  |  —  |  —  |
|  $1Si = 2Br$ |  4  |  2  |  1  |  —  |  —  |
|  $1Gl = 2Si$ |  8  |  4  |  2  |  1  |  —  |
|  $1Pt = 2Gl$ |  16 |  8  |  4  |  2  |  1  |

nb. Copper (Cp) dice only strike a success on a 6.

## 8. principles — goals, habits, & creeds

write about your character in three paragraphs labeled 'goals', 'habits', and 'creeds':

-   **Goals**
    -   these are things that your character wants to achieve over the course of the next few game sessions (or before the end of the current arc)
    -   they should be fairly direct and promissory, not wishful, and are best written in first person with the future tense:
        -   "I _will_ get my revenge..." not, "I would like to get revenge..."
        -   "We _must_ escape..." rather than, "We should try to escape..."
    -   try to avoid adding qualifying statements unless they help you to clarify a general motive
    -   you can use the **SMART** mnemonic, if it helps you. that is:
        -   The best goals are **S**pecific, **M**easurable, and **A**ctionable, for which you are **R**esponsible, and are **T**ime-bounded.
    -   during the debrief at the end of each chapter (1-3 sessions), you should advocate to your Peers for any goals you have completed during that same chapter.
        -   For each that you think you have, and your Peers agree too, earn a Lot.
        -   Then write new goals for the next chapter, or keep any on that are still relevant
    -   you can only re-write your current goals mid-way through a chapter with your FCs permission
        -   because they have probably planned something for your current goals, and they may have to do extra planning now if you suddenly change your mind
-   **Habits**
    -   these are things that your character always or never does, or things that they do so regularly or as part of a routine that they do them without really thinking about them
    -   they can effectively function as character 'macro functions', but try not to write them like computer code
        -   "If I ever feel I'm in danger, I secure my sidearm and ready it." instead of, "If in danger, then draw weapon."
        -   "Whenever we set out on the road, I like to strike up a song and keep spirits high!" not, "While travelling: sing."
    -   the choice to invoke a habit is always yours and yours alone, they don't execute automatically, and you still have to roleplay out the consequences and roll any dice if they result in a check or a task
        -   a habit _can_ briefly slide back time though:
            -   if something happens, and you realize that one of your habits could have been triggered by it and that it would change the way that you'd behave
            -   this cannot cross back into previous scenes though, only the current one
            -   and only works with Peer approval
    -   once per session: when invoking a habit presents an unforeseen dilemma, puts you under duress, embarasses or disturbs someone else, or otherwise creates interesting drama, then you earn Ego back at the end of that scene.
        -   If you already have Ego, then take a Lot instead.
-   **Creeds**
    -   these are things that you think your character believes in absolutely, or oathes they have sworn, doctrines they adhere to, and motivations or morals that are unwavering.
    -   they are best written as unqualified statements of fact (even if they're not actually true) without a hint of doubt in the tone, even if that makes them sound righteous or arrogant
        -   "_Nothing_ can break my love" not, "My love won't falter unless..."
        -   "God will protect me from all evil!" instead of, "I hope my god is real..."
    -   part of the FC's duties includes testing and prodding at these convictions over the course of each campaign arc, to see how ironclad they really are, and to see how steadfastly your character defends them.
        -   therefore, if there is something that you think character _really does_ believe in without question, _and you don't want it to be questioned_, then consider adding it to your background circumstances or writing it as a Feature instead of a Creed.
            -   you can always change a Feature or a background into a Creed at a later date, by voting it off and or re-writing your backgrounds, but you can't so easily change a Creed without playing the game
        -   similarly though, try to avoid offering any advice to your FC on how your Creeds could be challenged.
            -   This is part of the fun of the game, for both of you.
            -   Though the relationship should not become antagonistic.
    -   at the end of each arc, during that chapter's debrief or during a development session between arcs, your FC must ask you "which of your Creeds have not faltered?"
        -   if your response is "none" then read them aloud and let the FC press further and point to times when they think they have
            -   it is then up to the _FC's Peers_ table to decided if you really have faltered, or not.
        -   if your response is "this one" or "these ones" then read them out loud and then point to the times when you think they faltered
            -   it is then up to _your Peers_ to decide if they really did falter, or not.
    -   if one or more of your Creeds were found to have faltered then you may increase the level of one of your abilities by 1 and then you must write new Creeds before the next session
    -   if none of your Creeds were found to have faltered then you earn back your Ego (or a Lot) and may fill your Fidelity meter by one step, under the Kismet section of your character sheet
        -   once your Fidelity is full (four steps total), then at any dramatically appropriate time during the next arc you may drain your fidelity to _permantently_ increase the grade of one of your abilities by one step
            -   if you get to the end of the next arc without using your Fidelity then use it during the debrief before you have a chance to earn more.
-   you can share your principles with your Peers if you like (and, in fact, this is _encouraged_), but you _must_ share them with your FC so they can plan to accomodate the game around your desires as both a player and a character
    -   your FC can veto any goals, habits, or creeds that you present to them that they think would either be too distruptive or which are too easy to complete, trigger, or uphold (respectively).
-   you can write as many of each that you feel is appropriate, but if you start running out of space on the character sheet then that's a good sign you should trim them down a bit
    -   the FC may allow you write longer principles on a spare character sheet, but this is their choice
    -   alternatively, you can keep a character diary and write spare principles to swap in and out between each chapter
-   you can almost think of your habits and creeds as 'proto-features' which could get voted on as _real_ features during a development session if you play them to the hilt enough, freeing up space for new habits and creeds in the future

#### Kismet (metacurrencies)

<!--META-->

'Kismet' is a Turkish word derived from the Arabic 'qisma', meaning one's share in destiny.

-   **Lots**
    -   you can have up to 10 Lots at a time
        -   Lots spent on chacks add `+1d6` to your pool of advantages
        -   Lots spent on tasks let you KISS and reroll a die of your choice
        -   one Lot can be spent per check to reroll too
        -   you can earn a portion of your Lots back in the debreif every session by advocating for your portrayal of your character's aesthetic features and reflecting their choices throughout the session expressed via goals, habits, &/or creeds
        -   Lots earned during the debreif that would bring you above the maximum, 10, are converted into $exp$ to help you level up any skills of your choice
    -   you start the game with `1d6` Lots

-   **Ego**
    -   you either have Ego at any given time, or you don't
        -   spending Ego counts all your 6s twice for tasks
        -   or lets your roll another d20, for checks, and choose the highest result
        -   earn back Ego from introducing your own scenes
    -   flip a coin, or roll a die and call even or odds, to see if you'll start the game with Ego or not

-   **Fidelity**
    -   this is a counter that ranges from 0 to 4
    -   you earn Fidelity by not faltering your Creeds (see above)
        -   it is a reward for establishing and upholding your truth — your version of reality — whatever that may be, and whatever good or ill that it brings others
    -   once your Fidelity is full, you may spend it (draining it back down to zero) to permantently raise the grade of one of your abilities by one step
        -   ie. Bronze -> Silver, Silver -> Gold, Gold -> Platinum
        -   this is supposed to be done at a 'dramatically appropriate' time, but it can be any time really
    -   thus, to take one ability all the way from Bronze to Platinum, you'd need to earn a total of 12 Fidelity
        -   and a total of 68 Fidelity to reach Platinum in all abilities
            -   which, assuming you earn 1 Fidelity every 15 sessions, would take approximately 400 sessions to max out
    -   you do not start the game with any Fidelity

---

## 9. Modular Character Aspects [UNFINISHED]

<!--MODULES-->

#### capabilities (optional abilities)

-   capabilities function almost identically to abilities, except that:
    -   they are _derived_ from your current abilities and the answers given during a questionnaire
        -   the grade of a capability is equal to the lowest grade of two other abilities
        -   the level of a capability is equal to the number of questions you answer 'yes' to
            -   answer the questions honestly, as they will be subject to Peer review
    -   they can only be used to perform checks, not tasks
        -   often, failing a capability check takes a certain amount of agency away from your character for a brief time
        -   that is, failing a capability check will always result in consequence that you or your Peers choose from a list and then you should react or roleplay appropriately
    -   they are also completely optional / modular, and which ones you should use are heavily based on your game's current tone or themes
    -   however, sticking to a theme is important so that the game doesn't get diluted, so you may only choose up to 3
        -   decide as a group which ones you feel would be necessary or useful for your game
        -   different PCs _can_ each have different capabilities, but only if it makes sense...
            -   that said, it's better to try to be consistent
        -   since they are all derived, you can change out capabilities in a development session for new ones if your game theme has shifted
        -   and re-derive them again when the theme shifts back
            -   you may find you have different or new answers to the questions asked in the derivation process, and that's okay (arguably intentional)

###### _examples_

-   _Grit_ or _Might_?
    -   use with themes of violence, war, and combat
    -   a measure of your general audacity and your readiness to injure others, your disposition
        -   governs instinctual reactions in a fight
    -   calculated by: Add Wits and Swiftness, divide by 4, + questionnaire answers
-   _Guts_
    -   use with themes of violence, combat, mystery, and horror
    -   a measure of your physical and mental tolerance for putting yourself in harms way and potentially being injured, your mettle
        -   governs how long you can keep up the fight (akin to HP)
    -   calculated by: Add Endurance and Resolve, divide by 4, + questionnaire answers
-   _Wealth_
    -   use with themes of capitalism or feudalism, commerce, intrigue, and politics
    -   represents money management, investments, access to funds, etc. not for games where you want to track every penny
        0. someone else's property; a vagrant; a fugative; an untouchable
        1.  living beneath the poverty line; an indentured servant; or just down on your luck
        2.  living within your means; free but poor; living a nomadic lifestyle; or caged in comfort
        3.  starting to turn a profit; an apprentice; a student; a hustler; or a seasonal-soldier
        4.  enough savings for emergencies an special occasions; a guild-member; an itinerant trader; or a mercenary
        5.  full records, insurance, and regular savings; a master artisan; a residential merchant; or a professional-soldier
        6.  an aristocrat living off inheritance, investments, or exploitation; a superintendent; a guild-master; a knight; or a criminal kingpin
        7.  one born into wealth and sworn to fealty; lesser nobility; a viceroy; a chancellor; or robber-baron
        8.  a true blue-blood; greater nobility; practically sovereign; a warlord or dictator; or the cheif executive of a merchantile empire
    -   calculated by: Peer decision based on circumstances, paths, and questionnaire answers
-   _Links_
    -   use with themes of politics, intrigue, factionalism, and war
    -   represents a 'social wealth' of sorts: your current contacts, patrons, factions you are affiliated with, past associates, rivals, or lovers, and any favors still owed or contracts you've entered into with them
    -   good for social games set in a single city or county, not great for world-hopping adventures (better to just use 'first-impessions' Appeal checks in that case when meeting new people)
    -   calculated by: half your Appeal level + questionnaire answers
-   _Vigilance_
    -   use with themes of exploration, mystery, survival, horror, and overcoming supernatural events
    -   mental resilience to abnormal events and existential dread, your spirit or temperance
    -   calculated by: age bracket (1-4) + questionnaire answers
-   _Honor_
    -   use with themes of feudalism, politics, and chivalry
    -   calculated by: questionnaire answers

###### custom capabilities

-   all of the above are just suggestions
-   if you don't like the names of some of the capabilities above you can, of course, change them for your group or your setting
    -   the capabilities section of the character sheet has 3 blank spaces, for this reason, so you can write-in whatever you like
    -   just so long as you're consistent
-   or if want to make your own to suit your game's specific themes you can do so easily:
    -   make sure that the capability is something you can only perform checks with, typically as a reaction or something for which there are only a limited number of responses if you fail
        -   otherwise it might be better suited to being a custom job with some special requirements or usage conditions
    -   list of an ability or two to base the grade of the derived capability on
        -   do not make a compound capability derived from another capability
    -   think of up to 8 'yes-or-no'-questions and use the player's 'yes' answers to generate the level
    -   test out the capability through play, if you don't like it then you can tweak how it's used during development sessions

##### _NPC capabilities_

-   npcs generally don't roll dice (or don't perform tasks, at least)
-   so the npcs need a few extra capabilities that player characters don't, in order to set the difficulty for opposing rolls:
    -   or do they...?

---

<!--OTHER-->

# additional / modular gameplay features [UNFINISHED]

ultimately, almost all mechanics can be abstracted into different kinds of conflicts. each kind may have it's own system of resolution

-   internal conflict resolutions
    -   healing / recovery
    -   changing your mind
    -   problems that cannot be solved with your character sheet
        -   i.e. player skill vs character skill
-   character conflict resolutions
    -   battles
        -   active-initiative battle system?
    -   chases
    -   debates
    -   duels
    -   sex, money, and violence
-   environmental conflict resolutions
    -   animals
    -   traps
    -   envrionmental penalties are grouped such that you only apply the highest if multiple are applicable:
        -   light / visibility levels
        -   terrain stability
    -   natural disasters
-   supernatural conflict resolutions
    -   religions
    -   summoning weird things
-   technological conflict resolutions
    -   vehicles
-   societal conflict resolutions
    -   politics
    -   wars

### (mars)

fully optional supplemental material for combat heavy / borderline weapons-fetishistic games where the capabilities of every minute detail are really important

-   (i may never actually write this, this is mostly a joke)
