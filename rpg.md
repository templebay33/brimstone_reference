# Brimstone Horizons RPG
Brimstone Horizons RPG is a fan-made expansion for Shadows of Brimstone (Flying Frog Productions) which introduces light-weight role-playing elements into the existing sandbox style adventure mechanics of the official game. While similar fan-made expansions have already been produced (HexCrawl, Alone in the Shadows of Brimstone, Brimstone Adventures, etc.), Horizons takes an approach using a "lighter touch", sticking much closer to the vanilla experience. New mechanics are introduced sparingly in an effort to prioritize simplicity, flow, flexibility, and pacing of a campaign. 

Another goal of designing Horizons was to keep the necessity and cost of printing additional components low. While fan-made, digitally distributed content is essentially "free", the costs often involved in large print-and-play projects can easily rival or exceed top-tier, "all-in" Kickstarter pledges of new official content. While some of the *optional* modules offered by Horizons do require printed components, an emphasis has been placed on reducing the need for this where possible. This rule book for example is maintained both in PDF and in Markdown formats for easier viewing and searching on portable devices. 

Aside from being composed of modular elements, features of Brimstone Horizons RPG include:

* An NPC Encounter system for generating NPC's during your adventure and engaging in short, thematic social encounters with them.
* A Companion system for generating your own Hero Companions, similar to Allies, but powerful enough to count as fully capable Heroes in your solo adventures. This allows you to reduce the book-keeping of solo campaigns by supplimenting a single vanilla Hero with Companions that are mechanically much simpler to manage and track.
* A system for generating and playing Fights on large custom tiles and battle-maps. 
* A modified "Open Adventure" system for generating and playing adventure missions that extend outside the boundaries of a confined dungeon-crawl structure, allowing missions to take you to more remote and varied locations anywhere in your game world.
* New Travel Events to expand and replace the existing Travel Events system.
* Mini-games which offer short divergent experiences from the normal skill-check system during some encounters.
* Heaps of oracle tables to help assist in role-playing, adventure creation, and campaign design.

Each of the above modular systems have been designed to be easily modified by you, rules-light, fast-playing, and as cheap to implement as possible without requiring much labor. I hope you find at least some of Brimstone Horizons as enjoyable to play as I have in creating it!

## Narrative Writing Style
You'll notice that the writing style used for narrative descriptons of encounters, missions, and other RPG elements is vague and simple. The reason for this is not laziness, but intentionally non-specific so that you can fill in the details yourself to make your world your own. Instead of describing the details of what happens during an encounter, simple nouns and verbs are given as keywords so that you can fill in the rest in such a way that it fits within the context of your story. I tend to use a combination of three different approaches when building narrative detail inspired by the random events of the game.

The first is to take charge of the narrative myself. If you are using Horizon, chances are you're playing Shadows of Brimstone more like a TTRPG than a strategy game. Especially if you are playing solo, it's important to remember that there is no such thing as cheating! Whenever you have an idea that excites you "...if THIS happened instead...", it's a sure sign that you are going to have more fun by temporarily borrowing the reigns of control from the dice and steering your story in a direction that makes it more fun. This includes not only filling in the details of vaguely written events, but completely changing the nature of the events themselves.

The second is to make use of the age old tool known as oracle tables. These are simply tables you can roll dice against to select random options from, decks of cards you can draw from for random options, and similar tools. Don't want to decide for yourself what kind of flora you encountered and decided to try eating? Create an "Edible Flora" table and let the dice decide. Horizons includes an entire chapter full of Narrative Oracle Tables that might be of interest specific to the settings of Shadows of Brimstone.

The third and newest kid on the block is generative AI. At the current time of writing in Auguest of 2023, AI models have already become impressively adept at role-playing. Simply asking an AI to act as a narrator during your campaign and feeding in the vague details of your gameplay is all that is needed for what is often creative and well-written material. The more information you provide an AI about the lore and settings of your world, the basic rules of the game, and the style of narration that you desire, the better the result. A lot of the content provided by Horizons was itself assisted by AI.
# NPC Encounters

## Elements
- Event Card
  - Can be found on Encounters during an Adventure, Daily Events during a Town Stay, or drawn from the NPC Encounters deck when directed to do so via a Travel Event. 
  - Contains a Title, Flavor Text, and Event.
  - The Event is usually a Skill Check, but could also be a Mini-Game.
- Persona Card
  - The identity of an NPC in the world.
  - Title of the card is their name.
  - Contains Keywords, and possible modifiers during an Encounter.
- Disposition Dice
  - Used to roll for the starting Disposition of the NPC.
  - Disposition can be Low, Neutral, or High.
  - [1-3]: Low, [4,5]: Neutral, [6]: High.
  - Disposition can be raised or lowered as a result of the Encounter.
  - Disposition after resolving the Encounter determins the Consequence.
  - Some Persona Cards may modify or statically set the starting Disposition.
- Consequence Card
  - Represents how the NPC respond to you after the Encounter.
  - Each card maps to a different Disposition level.

## Integrating Into the Game
- NPC Encounters are special types of Adventure Encounters, Daily Events, and Travel Events. So they seamlessesly integrate with the gameplay loop.
- Optional: Can choose to have 1 random NPC Encounter per day in Town.
- Optional: Can choose to resolve an NPC Encounter whenever a "No Event" is rolled on a Town Location Chart.

## Example Encounter

1. The Heroes draw/roll a Daily Event during their Town Stay:  
**Title:** You Ain't One of Us!  
**Flavor:** *Someone has noticed you are an outsider in town. This could be a problem...*  
**Event:** One Hero makes a Cunning 5+ test and raises the Disposition by one if successful, lowers by one if failed. If any Heroes in the party are not native to the current world setting (Old West, Fedual Japan, etc.) instead make a Cunning 6+ test and set the starting Disposition to Low.

2. There are no non-native Heroes in the party, so next they roll a D6 to determine starting disposition and roll a 3 (Low).

3. Next a Persona card is drawn, identifying the NPC the Heroes are interacting with:  
**Name:** William Curtis  
**Keywords:** *Companion, Doctor, Old West*  
**Traits:**   
  Flirtatious: Any Female gendered Hero may add 1D6 to any skill tests when encountering William Curtis.  
  Companion: After resolving Consequences, you may add William Curtis to your party as a Frontier Doctor Companion if Disposition is High.

4. The Hero party does have a female gendered Hero in the party. She has a Cunning of 3, which is modified to a 4. She makes a skill check and passes. As stated om the Event, this raises William's Disposition to Neutral.

5. Next, the Heroes draw Consequence cards until they draw a Neutral Consequence. They draw the following card:  
**Title:** Feeling Generous  
**Disposition:** Neutral  
**Consequence:** One Hero may gain a Whiskey Side Bag Token.

6. Finally, since the Disposition was not raised to High, the Hero's do not have the option of adding William to their party as a Companion.


# Companions
Companions are generated by picking a class, rolling for their two abilities, and then rolling on a level-up chart whenever they gain a level. During the campaign, they do not equip new gear or acquire new abilities, keeping them simple to manage in comparison to the Hero. Of course as with anything in your campaign, you should feel free to modify as you see fit. But the design principle behind Companions was **not** to build adventuring partners that are as deep and interesting mechanically as Heroes, but rather partners that feel roughly equivalent to Heroes in their capabilities, while drastically simplifying the cost in "fiddlyness" to manage them during play. 

Companions are designed to be treated like Heroes for purposes of difficulty scaling. So if your campaign consists of a single Hero and 2 Companions, you would draw from the Medium Threat deck during play and be given a single Revive Token. This is the same as if you were playing with 3 Heroes. Companions are always counted as Heroes in terms of difficulty scaling.

While Companions are designed to be mechanically simple, they don't need to be limited at all in terms of role-playing and narrative during your adventures. A primary goal of the Companion system is to free up the players' mental focus from being spent on book-keeping to leave more room for role-playing.

While Companions were always intended to be used more for solo play, there is no mechanical reason why they cannot be used for multiplayer adventures or campaigns.

## Companion Restrictions
Companions have some of the same gameplay restrictions as Allies and there are many things they can do which Allies cannot. Here is the list of their restrictions, and a separate list of things they can do in comparison to Allies:

### Companion Restricitons
- May not earn XP
- May not equip new Items, Gear, or Artifacts
- May not visit Town Locations
- Does not participate in Town Events
- Does not participate in Town Location Events
- Does not participate in Town Hazard Events
- Does not gain Injuries, Madnesses, or Mutations

### Companion Differences Compared to Allies
- Rolls to Move like Heroes
- May get Critical Hits like Heroes
- May use Grit like Heroes
- May Draw Loot Cards like Heroes
- May Explore like Heroes (Scavenge and Look through Doors)
- Included in Random Hero Encounters
- Treated as Heroes during Travel Events
- May carry a default of 5 Side Bag Tokens

## Injury, Madness, and Mutations

For simplicity sake, Companions do not gain Injuries, Madness conditions, or Mutations. Instead, they accrue *Scars*, *Trauma*, and *Blight*. Whenever a Companion would gain an Injury, Madness, or Mutation like a Hero, they simply increase their current number of equivalent Scars, Traumas, or Blights on the Companion Sheet and follow the normal rules for Recovery if they were KO'd, or returning their Corruption to zero after gaining a Blight.

Each time a Companion increases their Scars, Traumas, or Blights, they then check for permanent death. This is done by first rolling 1D6. If the result is *below* the current level of Scars/Traumas/Blights, they are in the grip of death. The companion must then make one final Willpower roll on a 1D6 (no Grit). If they fail, they die. If the first roll is equal to or above the current number of Scars/Traumas/Blights, no final Willpower roll is required.

Scars, Traumas, and Blights can be healed by any game effect that would normally heal an Injuries, Madnesses, or Mutations. When this is done, decrease their current number of Scars/Traumas/Blights by one, to a minimum of zero.

## Companion Creation
Creating a new Companion is simple:

1. Select the Companion Class
2. Randomly select two Abilities from their Ability Chart, re-rolling duplicates.
3. Create a Companion Sheet copying their starting Level 1 information and their two abilities.
4. Give them their starting Side Bag Token(s).
5. Name your Companion!

A printable PDF has also been provided with a blank Companion Sheet if you would like to use it. I like to keep a handful of them laminated and use dry-erase markers.
## Companions Leveling Up
Companions do not earn XP. Any XP gained by a Companion is ignored. Companions "Level-Up" whenever the Hero in the Posse does. If there are multiple Heroes in the Posse, all Companions will Level-Up at the same time as the lowest level Hero. If Leveling Up during an Adventure, Companions reset their Wounds, Sanity, and Grit just as a Hero does.

When gaining a Level, make a 2D6 roll and consult the table below, updating the Companion Sheet with their new benefits:

**Companion Level Up Chart - 2D6**
| Roll | Benefit |
| :----: | ------- |
| 2 | +1 To Hit Melee or Ranged (your choice, To Hit 3+ max). If both already max, re-roll.|
| 3 | +1 Defense or Willpower (your choice, 3+ max). If both already max, re-roll. |
| 4, 5 | +1 Move. Increase Health AND Sanity by D3 (roll for each). |
| 6 - 8 | +1 random Attribute. Increase Health/Sanity (any mix) by D6. |
| 9, 10 | +1 Max Grit. Increase Health AND Sanity by D3 (roll for each). |
| 11, 12 | +1 Combat/Shots (your choice, max 5 each), or +1 Initiative. |

When determining a random Attribute to improve, use the following table:

**Random Attribute Table - D6**
| Roll | Attribute |
| ---- | --------- |
| 1 | Agility |
| 2 | Cunning |
| 3 | Spirit |
| 4 | Strength |
| 5 | Lore |
| 6 | Luck |

All Companions use the same table above when gaining a level. Companions **do not** earn new class abilities when leveling up.
## Companions Gaining Resources
Unlike Allies, Companions *may* Scavenge, Explore, participate in Encounters, draw Loot Cards, and earn Gold, Dark Stone, Gear and Artifacts during an Adventure. Companions may also earn other resources from some expansions such as Scrap and Tech in the Blasted Wastes. XP gained by Companions is ignored.

### Companion Resource Usage
Companions will "spend" **all** the resources (Gold, Dark Stone, etc.) they have accrued during each Town Stay. How this is performed is detailed later. Any additional resources that were not spent during the Town Stay or given to a Hero character via *persuasion* (explained later) are permanently removed from the Companion and considered to have been stashed in their "retirement fund".

### Companion Side Bag Token Usage
Companions may also carry Side Bag Tokens and the players may decide how they are used at any time just like a normal Hero. Companions will spend their time during a Town Stay replenishing their Side Bag Tokens using the Gold, Dark Stone, and other Loot they accrued during the previous Adventure. More on this below. 

Whenever a Companion would gain an additional Side Bag Token but has already reached their max token limit, the players may decide which tokens are kept and which are discarded. In addition, the player may decide other Companions or Heroes (with available capacity) to be given the dropped Side Bag Tokens. If there is nobody in the Posse able to pick up the dropped token, the token is lost/discarded.

### Companion Gear and Artifact Usage
Companions **never** equip Items such as Gear or Artifacts, preferring the comfort and familiarity of their own valuables. Such Items gained by a Companion are sold for their Sell Value during a Town Stay. The resulting Gold is then used by the Companion to purchase Side Bag Tokens as described later on.

* Any Gear or Artifact with no Sell Value is sold for D3x$25 by the Companion during their Town Stay. 
* Gear that is immediately discarded for Side Bag Tokens are used the normal way and the Companion will keep the resulting Side Bag Tokens if they have available capacity.


## Companions During Town Stay
After all Town Events and other events are resolved during the **first day** of a Town Stay, each Companion will sell everything they have gained while adventuring except for Side Bag Tokens. The Gold amount Companions gain from each item sold is:

* Dark Stone: $50/token
* Gear: Sell Value (D3x$25 if none)
* Artifact: Sell Value (D3x$25 if none)
* Scrap: $10/token
* Tech: $50/token

The resulting pool of Gold is then spent on the following list of priorities. The Companion will always start at the top item in the list and purchase it if enough Gold still remains in their pool, or move to the next item below if they cannot afford it. The Companion will continue this process until they have spent as much Gold as possible or if they have no additional capacity to purchase more.


| Cost | Item | Notes |
| ---- | ---- | ----- |
$200 | Heal Scar Attempt | 1D6: 1-3: Fail, 4-6 Success. Reduce Scars by 1. Skip if no Scars.
$200 | Heal Trauma Attempt | 1D6: 1-3: Fail, 4-6 Success. Reduce Trauma by 1. Skip if no Trauma.
$250 | Heal Blight Attempt | 1D6: 1-3: Fail, 4-6 Success. Reduce Blights by 1. Skip if no Blights.
| $ ? | Side Bag Token | See Companion Class Side Bag Priorities.

Each Companion class has a unique priority list of Side Bag Tokens specific to their class which they will purchase. When Companions purchase anything on these priority lists, there is no need for any specific Location to be available in Town. It is assumed that the Companion has found someone willing to sell them the good or provide the healing service no matter what the Town Location offerings are.

You'll notice that some of the Side Bag Token priority lists for each class specify a max number of tokens. When going through the priority list from top to bottom, the Companion will skip a line item if they already have the listed max number of the specific token in their Side Bag.

All remaining Gold the Companion has left is discarded after purchasing. 

After spending their Gold, Companions no longer participate in the rest of the Town Stay. They do not visit Town Locations or participate in Town Events. For gameplay purposes, Companions are considered to have "left Town" once they are done spending their Gold.

## Persuading Companions to Share
While your Companions have their own self-interests and desires for what to do with all that adventuring loot, it is possible for Hero's to persuade them to hand some of it over, considering the shared trials and dangers across your adventures.

A Companion in your Posse may be attempt to be persuaded by a Hero in your Posse to give them an item once per Adventure, and once per Town Stay. A persuasion attempt may be made during an Adventure at any point, except during a Fight. A persuasion attempt during Town Stay may be made before the Companion sells their acquired loot for Gold.

Before rolling dice for a persuasion attempt, the Hero **must** declare beforehand what kind of Item is being requested. The Hero can request **one** type of item per persuasion attempt from the following list:

* Dark Stone
* Scrap
* Tech
* Any single Gear Card
* Any single Artifact Card

When a persuasion attempt is made, the Hero picks any of their 6 skill attributes (Agility, Luck, etc.) to use for the test. The Companion being persuaded will also use the same attribute during the test. 

Both the Hero and Companion then make a 4+ skill check using the chosen attribute. Every success rolled by the Companion is used to cancel out one success of the Hero. The Hero may use Grit if desired, the Companion will never use Grit for this roll. 

If the Hero has any successes remaining after those that were canceled by the Companion, the Hero may "spend" those successes to take items from the Companion. The number of successes required to take a particular item is shown below:

| # of Successes | Item |
| --------------: | ---- |
| 1 | x2 Dark Stone Tokens |
| 1 | x3 Scrap Tokens |
| 1 | x1 Tech Token |
| 1 | 1 Gear/Artifact with Sell Value = $0 - $395
| 2 | 1 Gear/Artifact with Sell Value = $400 - $795
| 3 | 1 Gear/Artifact with Sell Value = $800+

If a persuasion attempt fails to procure at least one of the item requested (any amount of Dark Stone, etc.), the Companion has decided not to give away the item under any circumstances or future persuasion attempts, and the item will be sold during the next Town Stay.

# Persistent Towns
Horizons offers an alternative way to enhance the sense of "time and place" within the worlds of Shadows of Brimstone compared to some other systems. It's a simple approach that uses the concept of "persistent" Towns, but skips overworld movement, traveling, and tracking mechanics. 

Instead of offering a hex, grid, area, or point-to-point overworld map and then creating rules for the Posse to traverse the map, Horizons suggests giving each of the Towns you visit a name and recording the Town Size, Locations, and Type so that it can be re-created for future visits.

From a rules-light roleplaying perspective, I've found it sufficient to reference the hand drawn sketches of the Old West and Feudal Japan maps that are included within the Adventure Books of the game as a visual prop, and then simply record the Town names and their layouts.

While this is trivial to do on scrap paper, index cards, etc., PDF charts have also been made to help track the Towns in your campaign and how to re-create them.

No new rules are provided here for resolving the Travel Phase in the game. Players still roll for Travel Events based on the size of the Town they are visiting and resolve each event in the same way.

The only slight rules modifications are as follows:

1. When completing a mission *successfully*, the Hero Posse may choose which Town to visit. This can be a new Town not yet dynamically constructed according to the vanilla rules, or it can be a previous Town already visited which has not yet been destroyed by the Darkness.
2. When a mission ends in *failure*, the Hero Posse must limp to the nearest Town possible, which is determined by picking a Town randomly. 

Other than the above two recommended changes, no other rules changes to the vanilla game experience are made. The Travel Phase still only happens when traveling back to Town from an Adventure (Travel Events are not drawn when traveling **to** an Adventure), and no additional rules for tracking movement, distance, weather, terrain, etc., are introduced.

The Persistent Town charts provided, have a few convenient features which make them ideal for printing and lamination so they can be used/re-used for campaigns:

- A list of Town names taken from the official Adventure Book maps are already pre-populated.
- The Town names are numbered, making it easy to pick a random Town with a D20 roll.
- A small 2D6 chart for randomly determining Town Size is included, with Medium sized Towns being the most common result.
- Each possible Town Location and Type is listed on the chart, making it faster to simply check-mark the Type and various Locations found at each Town.

While it can be tempting to gloss over an approach this simple, you might be pleasantly surprised how easily this one small change can increase the immersiveness of your campaign. Instead of adding new gameplay systems, rules, and components for increased immersion, I've found that this can all be achieved through the Travel Events themselves. For example, instead of adding a survival system requiring your Posse to eat food while traveling the region, a simple Travel Event can be shuffled into the mix which requires the Hero Posse to test their hunting/gathering skills or risk penalties due to malnourishment. Combining the expanded Travel Events module suggested by Horizons with the Persistent Town module, should provide increased immersion into your campaigns without much additional rules overhead.
# Travel Encounters
The addition of new Travel Encounters which expand the ones found in the core game has been explored in several fan expansions of Shadows of Brimstone to date. It's an obvious way to expand the variety in the game that has not yet been done officially by Flying Frog Productions for one reason or another. 

Horizons uses Travel Encounters as a kind of "glue" to bring all of the other concepts together. Instead of introducing new core game mechanics, Horizons relies on new random events peppered throughout the game as a vehicle to express new gameplay elements. 

One example ais the addition of outdoor random combat encounters. Instead of procedurally making checks as you progress across the map to determine if your heroes find themselves in an outdoor confrontation, a few random Travel Events are added into the mix which trigger a Fight when rolled. The same technique is used to trigger other gameplay elements like NPC Encounters and Mini-Games. 


# Open Adventure Missions

## Open Adventure Missions - Components

### Environment Exploration Cards
Environment Exploration Cards work just like normal 

### Environment Cards
Environment 
### Environment Map Tiles
Every Environment Card should have at least one corresponding Environment Map Tile. Environment Map Tiles do not have puzzle-cut edges, and are not generally inteded to combine with other Map Tiles. Environment Map Tiles can be of any size or shape, but it is generally much easier from a "homebrew" perspective to stick to rectangular shapes. 

Environment Map Tiles can be sourced from anywhere: other games, commercially produced battle-maps and tiles sold by publishers intended for RPG's or skirmish games, hand-drawn tiles on paper, AI-generated tiles printed at home, etc. One of the primary goals of Open Adventure Missions is to provide a simple framework for fans to get creative with their own Shadows of Brimstone collection. The only general requirement is for the size of the squares/spaces on the tile to approximately fit the Shadows of Brimstone bases.

**Fights on Environment Map Tiles**  
The only real gameplay need for an Environment Map Tile is during a Fight. While players are welcome to still place Environment Map Tiles on the table during non-combat Encounters for increased immersion, they only have a practical use during Fights.

Setting up for Fights on the tiles can be done mostly according to vanilla rules, placing Enemies by Initiative order in a checkboard pattern on the opposite edge of the tile from the Heroes. Sticking to rectangular tiles is helpful so that you can simply use a D8 roll to randomly pick one of the four edges the heroes will start on.

Larger tiles and battle-maps are interesting in that you have more options on where to initially place models for a Fight. I like to use the black numbered square tokens provided with the core sets to place possible spawn points at interesting locations spread out across a larger map, and then randomly pick spawn locations for Heroes and Enemies. If some artwork element of the tile you are playing on makes narrative sense as a location for model placement, go for it!

There is no need for a strict set of rules to govern how to intially place models on a tile for a Fight. Get creative, have fun, and do what feels right.

**Environment Map Tile Sets**  
If you have the resources, you can add a lot of variety to your adventures by compiling a set of multiple Environment Map Tiles to match a single Environment Card. This works especially well with "Wilderness" Keyword tiles. If you have a set of 6 different tiles appropriate for representing a "Riverbank" Environment, roll a D6 when the "Riverbank" Environment Card is drawn to pick one randomly from your set.

**Environment "Furniture"**  
A classic, tried-and-true method for increasing the variety of Environment layouts is to rely on modular "Furniture" tiles or 3D "scatter terrain". Instead of relying on static 2D artwork featured on your Environment Tiles, it can be helpful to have some tiles representing generic rooms and outdoor patches of land. With a big enough library of furiniture or scatter terrain to place on top of the tile, you can create just about any kind of environment you want with nearly infinite variation. If you plan to print most of your tiles at home, I recommend considering this approach as it can save quite a bit of ink in the long-run!

## Set-Piece Map Tiles

A large map tile that has is abrubtly cut off on one side with puzzle-cut connectors. It can either be connect to another set-piece map tile to make one large "battle map", or it can be connected to its "map tile adapter" piece, which shrinks the "open edge" down to a standard 2-space wide puzzle-cut edge so that it can be used in your normal adventures.

### Environment Encounters
Environment Encounters work just like normal Encounter cards in Shadows of Brimstone. The only difference is in how they are split into different categories/settings. Each Environment Card and Tile combination, lists as its first Keyword the narrative "tone" of the location. These are Keywords such as:

- **Mundane:** *Every day Environments inhabited by some form of civilization (Library, Ranch, Well, City Street, etc.).*
- **Dread:** *Unsettling Environments with a sense of foreboding and despair (Graveyard, Ritual Altar, Battlefield, etc.)*
- **Wild:** *Environments un-touched by cilivization (Forest Clearing, Creek Bank, Dense Jungle, etc.)*

The back of each Environment Encounter Card matches one of these Keywords, so that the narrative description of the Encounter can better match the "tone" of the Environment. Whenever an Environment Encounter is drawn, it is drawn from the deck of Environment Encounters which match the corresponding Keyword on the Environment Card.


### Environment Depth Charts

# Mini-Games
# Campaign Generation
- Choose main world
  - old west
- Choose rival faction in main world
  - assemble card sets for rival missions (darkness, growing dread, threat, etc.)
  - werewolves
- create enemy pool for main world (5 normal and 2 XL?)
- create card pool for main world missions  (darkness, growing dread, threat, etc.)
- Choose a single OtherWorld (trederra)
  - assemble enemy sets for OtherWorld
  - assemble card pools for OtherWorld
- Choose Big Boss XXL Enemy (either main or OtherWorld)
  - assemble card sets for xxl enemy missions
  - can go for challege pack instead
- create mission pool for campaign:
  - 5 main world basic missions
  - all faction missions
  - all OtherWorld missions
  - Town missions
  - XXL/Challenge missions
- Select starting and finale missions from the pool.
- Select campaign goal & length
- Create hero party
  - Optional: Hero backstory, personality, personal goal, and personal rival (Hero Rivals)
- roll for starting mission!

# Companion Classes
The rules for Companions are in a previous section. This section lists the various Companion Classes (facsimiles of Hero classes) available when creating one. A few tables are provided to help you pick Companion Classes randomly if you prefer.

## Frontier Doc

| Agility | Cunning | Spirit | Strength | Lore | Luck |
| :-----: | :-----: | :----: | :------: | :--: | :--: |
| 2 | 4 | 2 | 2 | 3 | 1 |

| Initiative | Max Grit | Move | Corruption Limit |
| :--------: | :------: | :--: | :--------------: |
| 4 | 2 | +0 | 5 |

| Health | Sanity | Defense | Willpower |
| :-----: | :-----: | :----: | :------: |
| 12 | 12 | 5+ | 3+ |

| To Hit (Range) | To Hit (Melee) | Combat |
| :------------: | :------------: | :----: |
| 5+ | 4+ | 2 |



- **Keywords:** Frontier, Medical  
- **Pistol:** Shots 2, Range 6  
- **Surgeon's Saw:** Melee To Hit rolls of 6+ do +2 Damage each.
- **Starting Side Bag Token:** 3x Bandage Tokens



| Roll | Ability |
| :--: | --------- |
| 1    | Medical Training: *Add +5 to all rolls when using Bandage Tokens.* |
| 2 | Surgeon: *Once per Town Stay, roll to Heal a single Injury or Mutaton on a 4+.* |
| 3 | Wild Remedies: *At the end of your turn, remove one Status Effect Marker (Burning, Poison, etc.) from yourself or an ally. Then make a Lore 5+ test. If failed, lose 1 Grit.*
| 4 | Anatomical Analysis: *+X Damage on Combat Hits to all Enemy Types (Hell Bat, Void Spider, etc.) that has had at least 1 model killed by the Posse this Adventure. X is equal to your Level.* 
| 5 | Agile: *+1 Move. You may move through other models during your movement and automatically pass all Escape tests.*
| 6 | Improvisation: *You may spend Grit as Bandage Tokens.*

**Side Bag Priorities**
| Cost | Token |
| ---- | ---- |
| $25 | Bandage (Max 3, skip with *Improvisation*) |
| $25 | Potion (Max 2)|
| $50 | Whiskey (Max 2)|
| $100 | Dynamite |
| $50 | Tonic |


# Narrative Oracle Tables

## Narrative Event Hooks
Narrative flavor text in *italics* that are used in Encounters and Events will make use of nouns that are displayed in <u><font color="green">*underlined green*</font></u> text. These are narrative hooks for ehanced role-playing and can be completely ignored if desired as they have no gameplay purpose.

When some narrative text includes such a narrative hook, such as:

"*As you make your way through the murky swamps, you come across a <u><font color="green">*mysterious plant*</font></u>...*"

It is an opportunity for players interested to roll on a "Mysterious Plant" Oracle table:

# Quick Notes/Ideas

### Overhauled Injury/Madness/Mutation Conditions
Players can now only have 1 of each type. Whenever they would gain a 2nd of the same type, the existing condition worsens and becomes more severe. Intended to reduce tracking complexity.

### Growing Dread Removal
Growing Dread mechanic is completely removed from the game. I just don't like it.

### No XP Earning
Earning XP is removed. Instead, players level-up at specific points in a campaign all together.

### No Roll-to-Move (Earn Grit via Combat)
Completely replace the need to roll dice for move/grit. Grit is now earned as a reward similar to how XP used to be rewarded during combat: whenever a certain amount of damage is done to particular enemy types. For very weak enemies it could be eliminating more than one of that type of enemy in a single attack (2+ Void Spiders), for average enemies, it could be each model, for big bosses it could be doing larger amounts of damage in a single attack or hit.

### Static Hero Attributes
Hero Attributes (Agility, Cunning, etc.) do not change during a campaign or as the result of leveling up. They can be modified up or down, but can never exceed 6 or below 1. This makes temporarily modified attributes easy to track with a D6 placed on top of the attribute on the player sheet.

### De-Emphasis on Volume of Loot
To keep player-tracking more reasonable over a campaign. Heroes can have items currently "weilded" in their hand. Side-bag tokens are still the same. Heroes have 1-3 storage slots of more wieldable items that can be changed out, but that is the limit of "stuff" that a Hero can have in their face-up play area. See "Combat Deck" for how clothing/armor/abilities are handled.

### Combat Deck
Deck of action cards drawn from and played during combat encounteres. New abilities earned via leveling up are added as cards to this deck. Clothing/equipment/armor type items are also added as cards to this deck. Armor is represented as a card that can be played in response to taking damage during combat. At the beginning of an Adventure, a Hero shuffles their combat deck and draws 3. Those are the only 3 cards they have available during the entire adventure. Additional cards are earned during an Adventure when damage/sanity thresholds are reached (see Health/Sanity/Corruption tracks).

### Health/Sanity/Corruption Tracks
Each Hero has a track for each instead of using tokens. Max Health/Sanity/Corruption does NOT change as heroes level up (the 2d6 level chart goes away). Each track has thresholds where that Hero earns additional combat cards during an adventure as they lose Health/Sanity/Corruption, getting them back into the fight as things get more tense. This is the "Desparation" mechanic. Health is reset after each Fight.

### Leveling Up
Leveling up is now done by all Heroes at certain points along the campaign without any tracking of XP. This only consists of earning a new Perk. Each Hero class has a Perk tree that spans out in a web-like fashion where you can only earn a new Perk that is connected to one that you already have. Some Perks add combat cards, some Perks change or upgrade your single Class Ability card (see Class Ability cards). 

### Simplified Combat Stats
The following stats are removed: Max Grit, Combat, Melee To-Hit, Range To-Hit, Defense, Willpower, Initative. The combat system is modified to no longer require tracking these.

### Fate Track
A track used throughout the campaign. As "good" things happen to the Heroes (successfully completel mission, level up, earn rare artifacts) Fate decreases. As bad things happen (fail mission, injury/madness conditions, losing rare artifact) Fate increases. Darkness, Encounters, and Fights have things that get modified or triggered by the current level on the Fate track so that difficulty is dynamically adjusted/equialized during a campaign. The better you do, things get harder for a while, the worse you do, things get easier for a while.

### Monolith Style Battle-Maps

### Alternating Combat Activations

### More hand-crafted guidance on Adventures, Encounters, Events, etc., to create more consistent experiences.
Also emphasis on pacing.

### Re-tooled Epic Fights
No longer a long slog of slowly draining life from very tough bosses. Epic fights should not last much longer than normal fights, but rather just be more challenging.


