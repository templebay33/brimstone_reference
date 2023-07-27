# Cthulhu Wars - AI Game Reference
This is a compilation reference of rules, examples, and strategy for the board game "Cthulhu Wars" published by Petersen Games. It has been written in a way to be of maximal benefit to Large Language Models that are limited to understanding the game through text without the benefit of being able to see the visual elements of the game and understand it from that perspective.


The the rules in this reference are 100% correct according to the official game rules, they have been re-phrased in language and style more suitable to help an AI understand the game. Therefore, this may not be a good reference for a human to learn the game, since they would not benefit from visual aid's or text layouts that are more friendly to humans.


Game Summary:

Cthulhu Wars is a competitive strategy board game for 3-5 players where each player will control a Lovecraftian faction of supernatural creatures led by a Great Old One to dominate the Earth. Each Faction in the game has their own unique units, abilities, and play-style. The winner of the game is the player that has earned the most Doom Points when the game comes to an end. Key elements of the game include: area control, dice-based combat, resource management, and asymmetric faction abilities.


Theme:

While the theme of the game is Lovecraftian Horror and lore where the players get to play as the dark and evil Great Old Ones, the theme is not at all necessary to understanding how the game is played. Since Cthulhu Wars is purely a strategy game and not similar to a role-playing game, an AI would have little use for further narrative and thematic information about the game.


## The Board
The board is an abstract map of Earth split into two halves which are placed side-by-side when setting up the game table to form one large map. The half of the map featuring North America will be referred to as the "Western Board" and the half of the map featuring Asia will be referred to as the "Eastern Board". The term "board" refers to one of the two halfs, while the term "map" refers to both boards combined into a single large map. 

### Board Sides
Each of the two boards are double-sided and feature a 3-Player side and a 5-Plyer side. The board can be configured in one of 4 ways during game setup, depending on the number of players:
- 3 Players: Western Board on the 3-Player side, Eastern Board on the 3-Player side.
- 4 Players: Western Board on the 5-Player side, Eastern Board on the 3-Player side. 
- 4 Players Alternate: Western Board on the 3-Player side, Eastern Board on the 5-Player side.
- 5 Players: Western Board on the 5-player side, Eastern Board on the 5-Player side.

Note that either the "4 Players" or "4 Players Alternate" layout can be used when playing with 4 players and must be specified which layout is used during set up.

### Map Elements
There are 3 gameplay elements on the map:
- Areas: These are the locations on the map. Every unit, gate, and marker is located within a single area on the map. Each area has a unique name. The number of areas and their names change depending on the map layout used. Layouts for higher player counts feature more areas than those with lower player counts. Any single area is considered to be one of two possible types: Land and Ocean.
- Faction Symbols: Some areas contain a Faction Symbol which is used to determine the start location for that faction when the game is set up. The faction symbols rarely have gameplay purpose other than for initial setup of the game. The areas that these faction symbols are located in depend on the map layout used.
- Glyphs: Glyphs are symbols displayed in some areas. Glyphs have special meaning and purpose for the Yellow Sign faction and will be explained in futher detail in the rules for the Yellow Sign. The areas that these glyphs are located in depend on the map layout used. There are 3 different types of glyphs on the map and all that matters for gameplay purposes are there names and the area in which they are located. Their names are: Arrow Glyph, Snake Glyph, Claw Glyph.

### Map Layouts
Pictures and diagrams are not be necessary for an AI to understand the geometry and layout of the map. All that is necessary is a list of names each area on the map and for each of those area, a list of what other areas it is adjacent to and what Faction Symbols or Glphys are located in the area (if any). The type (either Land or Ocean) is also specified. This list will be different depending on the map layout used. Here is the descriptive list for each of the 4 possible map layouts:

**3-Player Layout:**  
(Western Board 3-Player side, Eastern Board 3-Player side)
- Arctic Ocean
  - Adjacent Areas: North Pacific, North America, North Atlantic, Europe, Asia
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Ocean
- North America
  - Adjacent Areas: North Pacific, Arctic Ocean, North Atlantic, South America
  - Faction Symbol: Sleeper
  - Glyph: Snake Glyph
  - Type: Land
- North Pacific
  - Adjacent Areas: Arctic Ocean, North America, South America, Indian Ocean, South Pacific, Asia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- North Atlantic
  - Adjacent Areas: Arctic Ocean, North America, South America, Europe, South Atlantic, Asia, Africa
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- South America
  - Adjacent Areas: North Atlantic, North America, North Pacific, South Pacific, South Atlantic
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- South Pacific
  - Adjacent Areas: South America, Australia, North Pacific, Indian Ocean, South Atlantic, Antarctica
  - Faction Symbol: Great Cthulhu
  - Glyph: N/A
  - Type: Ocean
- Australia
  - Adjacent Areas: Indian Ocean, South Pacific
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- Indian Ocean
  - Adjacent Areas: Australia, North Pacific, South Pacific, Asia, Africa, South Atlantic, Antarctica
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Europe
  - Adjacent Areas: Asia, Arctic Ocean, North Atlantic
  - Faction Symbol: Yellow Sign
  - Glyph: Claw Glyph
  - Type: Land
- Asia
  - Adjacent Areas: Arctic Ocean, Europe, North Pacific, North Atlantic, Africa, Indian Ocean
  - Faction Symbol: Crawling Chaos
  - Glyph: Claw Glyph
  - Type: Land
- Africa
  - Adjacent Areas: North Atlantic, Asia, Indian Ocean, South Atlantic
  - Faction Symbol: Black Goat
  - Glyph: Arrow Glyph
  - Type: Land
- Antarctica
  - Adjacent Areas: South Pacific, South Atlantic, Indian Ocean
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Land
- South Atlantic
  - Adjacent Areas: Antarctica, South Pacific, South America, North Atlantic, Africa, Indian Ocean
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean


**4-Player Layout:**  
(Western Board 5-Player side, Eastern Board 3-Player side)
- Arctic Ocean
  - Adjacent Areas: North Pacific, North America East, North America West, North Atlantic, Europe, Asia
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Ocean
- North America East
  - Adjacent Areas: North Atlantic, North America West, Arctic Ocean
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- North America West
  - Adjacent Areas: North Atlantic, North America East, Arctic Ocean, North Pacific, Central America
  - Faction Symbol: Sleeper
  - Glyph: Snake Glyph
  - Type: Land
- Central America
  - Adjacent Areas: North Pacific, North America West, North Atlantic, South America West, South America East
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- North Pacific
  - Adjacent Areas: Arctic Ocean, North America West, Central America, South America West, Indian Ocean, South Pacific, Asia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- North Atlantic
  - Adjacent Areas: Arctic Ocean, North America East, North America West, Central America, South America East, Europe, South Atlantic, Asia, Africa
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- South Atlantic
  - Adjacent Areas: North Atlantic, South America East, South Pacific, Antarctica, Africa, Indian Ocean
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- South America West
  - Adjacent Areas: South America East, Central America, North Pacific, South Pacific, South Atlantic
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- South America East
  - Adjacent Areas: South America West, North Atlantic, Central America, South Atlantic
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- South Pacific
  - Adjacent Areas: South America West, Antarctica, South Atlantic, New Zealand, Indian Ocean, North Pacific
  - Faction Symbol: Great Cthulhu
  - Glyph: N/A
  - Type: Ocean
- New Zealand
  - Adjacent Areas: South Pacific, Australia, Indian Ocean
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- Australia
  - Adjacent Areas: Indian Ocean, New Zealand
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- Indian Ocean
  - Adjacent Areas: Australia, North Pacific, South Pacific, Asia, Africa, South Atlantic, Antarctica
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Europe
  - Adjacent Areas: Asia, Arctic Ocean, North Atlantic
  - Faction Symbol: Yellow Sign
  - Glyph: Claw Glyph
  - Type: Land
- Asia
  - Adjacent Areas: Arctic Ocean, Europe, North Pacific, North Atlantic, Africa, Indian Ocean
  - Faction Symbol: Crawling Chaos
  - Glyph: Claw Glyph
  - Type: Land
- Africa
  - Adjacent Areas: North Atlantic, Asia, Indian Ocean, South Atlantic
  - Faction Symbol: Black Goat
  - Glyph: Arrow Glyph
  - Type: Land
- Antarctica
  - Adjacent Areas: South Pacific, South Atlantic, Indian Ocean
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Land


**4-Player Layout Alternate:**  
(Western Board 3-Player side, Eastern Board 5-Player side)
- Arctic Ocean
  - Adjacent Areas: North Pacific, North America, North Atlantic, Scandinavia, North Asia
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Ocean
- North America
  - Adjacent Areas: Arctic Ocean, North Pacific, North Atlantic, South America
  - Faction Symbol: Sleeper
  - Glyph: Snake Glyph
  - Type: Land
- South America
  - Adjacent Areas: North America, North Atlantic, North Pacific, South Atlantic, South Pacific
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- Australia
  - Adjacent Areas: Indian Ocean, South Pacific
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- North Atlantic
  - Adjacent Areas: Arctic Ocean, North America, Europe, Scandinavia, West Africa, Arabia, South Atlantic, South America, North Pacific
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- North Pacific
  - Adjacent Areas: Arctic Ocean, North America, North Atlantic, Indian Ocean, South Pacific, North Asia, South Asia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Indian Ocean
  - Adjacent Areas: North Pacific, South Pacific, Australia, South Asia, Arabia, East Africa, South Atlantic, Antarctica
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- South Pacific
  - Adjacent Areas: South America, South Atlantic, Antarctica, North Pacific, Indian Ocean, Australia
  - Faction Symbol: Great Cthulhu
  - Glyph: N/A
  - Type: Ocean
- South Atlantic
  - Adjacent Areas: North Atlantic, West Africa, East Africa, Indian Ocean, Antarctica, South Pacific, South America
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Antarctica
  - Adjacent Areas: South Pacific, South Atlantic, Indian Ocean
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Land
- East Africa
  - Adjacent Areas: Indian Ocean, South Atlantic, West Africa, Arabia
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- West Africa
  - Adjacent Areas: North Atlantic, Arabia, East Africa, South Pacific
  - Faction Symbol: Black Goat
  - Glyph: Arrow Glyph
  - Type: Land
- Arabia
  - Adjacent Areas: North Atlantic, Europe, North Asia, South Asia, Indian Ocean, East Africa, West Africa
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- South Asia
  - Adjacent Areas: Arabia, North Asia, North Pacific, Indian Ocean
  - Faction Symbol: Crawling Chaos
  - Glyph: Claw Glyph
  - Type: Land
- North Asia
  - Adjacent Areas: Arctic Ocean, North Pacific, South Asia, Arabia, Europe, Scandinavia
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- Scandinavia
  - Adjacent Areas: Arctic Ocean, North Asia, Europe, North Atlantic
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- Europe
  - Adjacent Areas: North Atlantic, Scandinavia, North Asia, Arabia
  - Faction Symbol: Yellow Sign
  - Glyph: Claw Glyph
  - Type: Land

**5-Player Layout:**  
(Western Board 5-Player side, Eastern Board 5-Player side)
- Arctic Ocean:
  - Adjacent Areas: North America East, North Atlantic, North America West, North Pacific, Scandinavia, North Asia
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Ocean
- North America East
  - Adjacent Areas: Arcitc Ocean, North America West, North Atlantic
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- North America West
  - Adjacent Areas: Arctic Ocean, North America East, Central America, North Pacific, North Atlantic
  - Faction Symbol: Sleeper
  - Glyph: Snake Glyph
  - Type: Land
- Central America
  - Adjacent Areas: North America West, North Pacific, North Atlantic, South America East, South America West
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- South America West
  - Adjacent Areas: Central America, South America East, South Atlantic, South Pacific, North Pacific
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- South America East
  - Adjacent Areas: North Atlantic, South Atlantic, South America West, Central America
  - Faction Symbol: N/A
  - Glyph: Snake Glyph
  - Type: Land
- New Zealand
  - Adjacent Areas: Australia, Indian Ocean, South Pacific
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- Australia
  - Adjacent Areas: Indian Ocean, New Zealand
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- North Atlantic
  - Adjacent Areas: Arctic Ocean, North America East, North America West, Central America, South America East, South Atlantic, West Africa, Arabia, Europe, Scandinavia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- North Pacific
  - Adjacent Areas: Arctic Ocean, North America West, Central America, South America West, South Pacific, Indian Ocean, North Asia, South Asia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Indian Ocean
  - Adjacent Areas: North Pacific, South Pacific, New Zealand, Australia, Antarctica, East Africa, Arabia, South Asia
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- South Pacific
  - Adjacent Areas: South America West, North Pacific, New Zealand, Indian Ocean, South Atlantic, Antarctica
  - Faction Symbol: Great Cthulhu
  - Glyph: N/A
  - Type: Ocean
- South Atlantic
  - Adjacent Areas: North Atlantic, West Africa, East Africa, Indian Ocean, Antarctica, South Pacific, South America East, South America West
  - Faction Symbol: N/A
  - Glyph: N/A
  - Type: Ocean
- Antarctica
  - Adjacent Areas: South Pacific,. South Atlantic, Indian Ocean
  - Faction Symbol: Windwalker
  - Glyph: N/A
  - Type: Land
- East Africa
  - Adjacent Areas: South Atlantic, West Africa, Arabia, Indian Ocean
  - Faction Symbol: N/A
  - Glyph: Arrow Glyph
  - Type: Land
- West Africa
  - Adjacent Areas: South Atlantic, North Atlantic, Arabia, East Africa
  - Faction Symbol: Black Goat
  - Glyph: Arrow Glyph
  - Type: Land
- Arabia
  - Adjacent Areas: Indian Ocean, East Africa, West Africa, North Atlantic, Europe, North Asia, South Asia
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- South Asia
  - Adjacent Areas: North Asia, North Pacific, Indian Ocean, Arabia
  - Faction Symbol: Crawling Chaos
  - Glyph: Claw Glyph
  - Type: Land
- North Asia
  - Adjacent Areas: Arctic Ocean, North Pacific, South Asia, Arabia, Scandinavia, Europe
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- Scandinavia
  - Adjacent Areas: Arctic Ocean, North Asia, Europe, North Atlantic
  - Faction Symbol: N/A
  - Glyph: Claw Glyph
  - Type: Land
- Europe
  - Adjacent Areas: North Atlantic, Scandinavia, North Asia, Arabia
  - Faction Symbol: Yellow Sign
  - Glyph: Claw Glyph
  - Type: Land


### AI Understanding Map Movement
An AI should keep the following in mind when reasoning about map adjacency: 

Area adjacency works in both directions. For example, if South Pacific is adjacent to Antarctica, then Antarctica MUST be adjacent to South Pacific. 

## Acton Phase

### Move Action
- Action Name: Move
- Cost: 1 Power per Unit Moved
- Type: Common
- Procedure:  
  1. Spend 1 Power for each unit you wish to move.
  2. For each Power spent, pick 1 unit to move. You may choose any of your units on the map that have not yet moved this turn. Each unit may only be moved once per turn.
  3. For each unit chosen, move that unit into an adjacent area. Use the appropriate Map Layout chart corresponding to the current map layout in use to determine which areas are adjacent to the unit you are moving.
- Gameplay Example:  
A game is being played on the 3-Player map layout. The Great Cthulhu player has two acolyte units he wishes to move that are both currently located in the South Pacific area, as well as a Deep One unit he wants to move that is currently in the North Atlantic area. He wants to move all 3 units in a single turn. He first spends 3 Power because he will be moving 3 units. If he did not have at least 3 Power still available, he could not move 3 units. After spending 3 Power, he moves each unit one at a time to an adjacent area from the area they are currently located in. He does this one by one in any order he chooses. He decides to first move one of his acolyte units from the South Pacific area to the South America area. He then wants to keep that Acolyte safe from being captured, so he moves his Deep One unit from the North Atlantic area to the South America area. The Acolyte in South America is now protected from capture by other monsters due to the presence of the Deep One also in South America. Finally, he moves one of his other Acolyte units in South Pacific that has not yet moved this turn into the North Pacific area where he plans to build a Gate on a future turn.
- Move Action Rule Clarifications:  
  - Since the movement action only allows a unit to move into an adjacent area and each unit may only be moved once per turn, it is not possible to move a unit into a space that is not adjacent in a single turn, no matter how much Power is spent.  
  - Since the Crawling Chaos faction has the Flight ability, which allows all of their units to move up to two areas away, playing as Crawling Chaos is one of the few circumstances in which a player can move a single unit to a non-adjacent space in a single turn. This is because the Crawling Chaos Flight ability is a faction ability, and faction abilities take precedence over the basic rules of the game when they conflict. 


## Special Abilities
There are 3 types of special abilities in the game:  
- Faction Abilities: Each faction has a special faction ability that always applies as long as the faction is present in the game.
- Unit Abilities: Some units (Cultists, Monsters, Terrors, and Great Old Ones) have unique unit abilities which apply to that unit in some way. 
- Spellbook Abilities: Most spellbooks provide the player that owns them a new ability when it is unlocked during the game. Many spellbooks provide a new ability to a unit when unlocked and can therefore be considered both a spellbook ability AND a unit ability.

The term "ability" or "special ability" can refer to any of the three types of special abilities and can be terms that are used freely by players and AI's. For example, the spellbook "Passion" can be considered a spellbook ability, a unit ability, a special ability, or just referred to as an ability. 

