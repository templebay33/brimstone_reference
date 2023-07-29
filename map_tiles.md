# Shadows of Brimstone - Map Tile Reference
This reference provides information on the Map Tiles throughout all the products in Shadows of Brimstone, including their physical layout. 

This reference is intended to be understood by large language AI models. Currently, such models lack reliable multi-modal capabilities, including the ability to understand data from within images. Because of this, the Map Tiles for the game have had their physical layout described in text format.  


## Visual Description of Physical Map Tiles
The physical Map Tiles are described in this section so they may assist an AI in understanding and tracking how they are placed on the table. By "physical" map tile, I'm referring to the "real" map tiles that this section is using language to describe.

The Map Tiles that are included in various Core, Adventure, and Expansion boxes are flat cardboard tiles that take on various 2D shapes and have artwork depicted on both sides of the 2D tile. The different art work on either side of a particular Map Tile correspond to two different World Locations (e.g., one side might be a tile for the Mines, while the other depicts a location in the Swamps of Jargono).

The borders of the map tiles are black lines representing impassable walls. Almost every Map Tile has at least two puzzle-cut edges for connecting to other randomly drawn Map Tiles. Entrance Map Tiles and End Caps only have a single puzzle-cut edge. 

The artwork depicted on the tile is from a top-down perspective and highly evocative to help visually represent the Heroes walking through the location when the game miniatures are placed on the tile. Layered on top of the artwork is a grid of squares, about 1.2 inches across both horizontally and vertically to form square spaces. These "spaces" regulate miniature movement across the tile. Each square on the Map Tile is called a space.  

Some of the black wall lines bordering the map tile cut off a space so that the area inside the space is smaller than normal. These "partial" spaces be at least 50% the size of a full square space in order to be considered a valid space for gameplay purposes. Spaces cut off by wall borders smaller than half of a full space are NOT considered valid spaces for gameplay and are ignored.

Puzzle-cut edges in the cardboard used for connecting to other map tiles always cut off exactly two spaces. These spaces cut off by puzzle-cut edges are considered valid spaces and may be occupied by models even if there is no other map tile connected to it. Every puzzle-cut connection on every Map Tile in Shadows of Brimstone is two spaces wide to ensure that all Map Tiles can be connected to one another.  


## Text Format of Map Tile Layout
The physical layout of spaces on Map Tiles can be approximated using text in an ASCII art style similar to those employed by text-based roguelike games such as NetHack. This helps an AI understand and evaluate the geometric layout of Map Tiles for gameplay purposes. We will refer to each ASCII art depiction of a Map Tile layout as a "Map Tile Diagram" or a "tile diagram". Within this Markdown document, each Map Tile Diagram will be displayed inside a codeblock element to preserve the whitespace needed to properly depict the map tile diagram. The rest of this section details the symbology used for representing map tiles with a diagram and how to interpret the diagrams. 

**No Whitespace in Diagrams**

Whitespace can cause problems with text character alignment in some displays and occasional issues with copy/paste operations of the text. For this reason, all whitespace in a diagram is replaced with a dot "." character. The dot character does not represent anything on a real physical map tile and should just be interpreted as blank space. When drawing a map tile diagram, an AI should ALWAYS replace any whitespace with "." characters.

**Basic Space Gridlines**

The basic horizontal and vertical lines that define a square space are represented by 3 characters:
- "|" represents a vertical line
- "-" represents a horizontal line
- "+" represents a corner where a vertical and horizontal line intersect

The internal dimensions of each space are 3 characters wide by 1 character tall (this does NOT include the grid line symbols on the edges and corners of the space). Thus, a single square space can be drawn like so:

```
.........
..+---+..
..|...|..
..+---+..
.........
```

Note that as previously stated, the "." character is treated as blank white space and is completely ignored for gameplay purposes.

Here is an example of a 2x2 grid of spaces:

```
..............
..+---+---+...
..|...|...|...
..+---+---+...
..|...|...|...
..+---+---+...
..............
```

Note that the map diagrams are ALWYAS placed within blockquotes in this markdown document.

**Space ID's**

Spaces have room for 3 characters inside them so that unique ID's can fit inside each space. Each ID is unique within the tile being shown. Each ID begins with a single uppewr-case letter which maps to rows and two numbers which together map to columns. Thus the space "C04" indicates the third row down from the top and the 4th column from the left.

If we were to add column and row labels in addition to space ID's to a diagram example, it would look like this:

```
......................
.......01..02..03.....
..,..+---+---+........
..A..|A01|A02|........
.....+---+---+---+....
..B..|B01|B02|B03|....
.....+---+---+---+....
..C......|C02|C03|....
.........+---+---+....
......................
```

Notice that even though space C02 is the first valid space in the C row, we still label it as "C02" instead of "C01" because it is part of column "02".

Normally, map diagrams will not include column and row headers like this example. 

Space ID's make it easier to talk about map tiles and describe where models/miniatures and other game elements are placed on them because we can refer to the ID's in our descriptions.

We can conclude that because a space ID always begins with an upper-case letter and continues to use that letter across the same row, the maximum number of spaces this notation system supports is a 100x26 grid. That limitation is not a problem however since all map tiles within the game are much smaller than this.

**Walls**

Edges and corners of spaces that are covered by a thick black line (on the physical map tiles) are walls. It is important to understand which space edges and corners are marked as walls for gameplay purposes. Walls block adjacency, movement, and line of sight.

Generally, the edges and corners of spaces which make up the outer borders of a map tile are walls. But walls can also sometimes extend into the tile a bit, so it is important to mark where they are in the diagram.

Walls are represented by the "#" character. Walls can replace horizontal edges of spaces marked with "-", vertical edges of spaces marked with "|", and corners of spaces marked with "+". Any time "-", "|", or "+" is replaced with "#", that element is considered to be a wall in addition to being an edge or corner. These can be referred to as "walled edges", "walled corners", or just "walls". 

If we surround the borders of the previous example tile with walls it would look like this:

```
.................
#########........
#A01|A02#........
#---+---#####....
#B01|B02|B03#....
#####---+---#....
....#C02|C03#....
....#########....
.................
```

Note that in this example, only the outer edges of the spaces are walled. The internal edges have no walls. Spaces A02 and B02 share and edge without a wall. Spaces B01 and C02 only share a corner. Since that corner is marked with a "#", spaces B01 and C02 are separated by a wall.

**Cardinal Directions**  
Corners, sides/edges and other features can be described using a mix of direction and cardinal directional terms. The following directional terms are interchangeable when describing a tile and mean the same thing:

- Top = North (N)
- Top-Right = North East (NE)
- Right = East (E)
- Bottom-Right = South East (SE)
- Bottom = South (S)
- Bottom-Left = South West (SW)
- Left = West (W)
- Top-Left = North West (NW)

Additionally, the terms "up" and "above" when describing map tile elements mean north or top, and the terms "down" or "below" mean bottom or south.

The terms "edges" and "sides" are interchangeable within the context of map tile elements and both mean a horizontal or vertical line bordering one or more spaces.

The terms "gridlines" or "grid lines" refer to edges and corners surrounding spaces that are NOT walls.


**Doorways**
On the real-world physical tiles, "doorway" spaces have a puzzle-cut shape cutting in the edge of the spaces, cutting the spaces in half. These doorway spaces always come in pairs and are made to physically connect to the puzzle-cut doorway spaces on other tiles. When two map tiles are connected together, the half-sized spaces from the first tile and the half-sized spaces from the second combine to form full size spaces. For gameplay purposes, when a model occupies one of these doorway spaces when two tiles are connected, the model is considered to be located on both tiles simultaneously.

For the text based map diagrams, doorway spaces are easily identified because they do not have edges or walls fully surrounding the space.

Here is an example of a simple passage tile that features doorway spaces:

```
#A01|A02#
#---+---#
#B01|B02#
#---+---#
#C01|C02#
#---+---#
#D01|D02#
```
In the above examples, spaces A01 and A02 are doorway spaces. This is because the top edge of these spaces do not feature any "-", "|", or "#" characters. 

If ANY edge on a space does not have "-", "|", or "#" characters, but the space does have ID's, those spaces MUST be doorway spaces.

By this logic, D01 and D02 are also doorway spaces.

This example only showed doorway spaces pointing along a vertical axis but they can also appear on a horizontal axis as in this example of another passage tile:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```

This T-Junction tile features doorway spaces open in both horizontal and verical directions. Spaces A01, B01, A06, B06, D03, and D04 are all doorway spaces and for the same reason in the previous example (one of the edges of a space with an ID lacks "#", "-", or "|")

As previously stated, doorway spaces are always in pairs. While each of the two spaces can be referred to as "doorway spaces", as a pair they form a single "doorway". In gameplay terms, a "doorway" can be defined as a pair of adjacent "doorway spaces". 

The text notation we will use when referring to a doorway as opposed to individual doorway spaces, is simply the letter or number that is common to both doorway spaces.

In the above example, spaces A01 and B01 are adjacent spaces that together form a doorway. Since the digits 01 are common to the ID's of spaces A01 and B01, we will refer to the doorway as "doorway 01" or simply "doorway 1".

On the vertical axis, spaces D03 and D04 together for a doorway. Since the letter "D" is what is common to both ID's, we will refer to that doorway as doorway D. 



### Basic Map Tile Diagram Examples
Let's take a look at a few examples of a basic Map Tile Diagram using the symbology that was just defined.

Here is a map tile diagram of a basic corner passage map tile:

```
.###############
A01|A02|A03|A04#
.--+---+---+---#
B01|B02|B03|B04#
.#######---+---#
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```

The following statements are TRUE about the above map tile diagram:
- The top-most and right-most edges of the tile are walls because they are designated with "#".
- Spaces A02 and V03 share a corner marked with "+".
- There are two doorways on this tile, doorway 1 and doorway D
- The distance between A01 and C04 is 3 spaces.

Here are some statements that are FALSE about the above map tile diagram with reasons why they are false:
- False Statement: Space B04 is surrounded by walls on all sides.
  Why it's False: For space B04 to be surrounded by walls on all sides, each edge must be marked with a "#". Only the right side of space B04 is marked with "#" so it is not surrounded by walls on all sides.
- False Statement: Space A04 is part of a doorway.
  Why it's False: If space A04 were a doorway space, it would have at least one edge which lacks a "|", "#", or "-". Space A04 does not lack such an edge as all edges are defined.

**Map Tile Diagram Conventions**  
As you see more map tile diagram examples, you may notice a few conventions that should always be followed when creating, rendering, or drawing map tile diagrams.

The southern or bottom most doorway spaces of each map diagram area always the "entrance" doorway spaces of a map tile. This is because the orientation of how a map tile is rotated when it is placed during gameplay is marked with an arrow on the related Map Tile Card which shows the "entrance spaces". This arrow designating the "entrance space" tells the player which doorway spaces to use when connecting the newly drawn map tile to the current map tile that the Heroes are standing when taking an explore action. This ensures that the newly drawn map tile is oriented/rotated in the intended orientation when it is placed on the table. As a shorthand, the map tile diagrams in this document are always oriented so that the entrance spaces are on the bottom for consistency and clarity.

You'll also notice that two of the edges of doorway spaces are only half the length of a normal space edge. This helps to visually indicate that these are puzzle-cut spaces in the diagram and that they are half the size of a normal space until they are connected to another Map Tile.

Additionally, map diagrams are also drawn to minimize the unnecessary amount of "." characters to show whitespace. This is simply done by making sure that the left most characters representing the map tile (characters that are NOT a ".") are on the left most edge of the diagram.

In other words, this simple diagram of a map would NOT be following convention:

```
...#A01|A02#
...#---+---#
...#B01|B02#
...#---+---#
...#C01|C02#
...#---+---#
...#D01|D02#
```

This is because it is unnecessary to include the whitespace on the left side. Instead, the same map tile drawn using a diagram the DOES follow convention would looke like this:

```
#A01|A02#
#---+---#
#B01|B02#
#---+---#
#C01|C02#
#---+---#
#D01|D02#
```

This does not mean that it is not sometimes necessary to have whitespace in a diagram. This T-Junction diagram which DOES follow the convention also contains necessary "." characters:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```

In the above diagram, the left-most characters that are NOT "." characters are the "A" and "B" characters necessary for the space ID's used for doorway 1. Since these spaces are doorway spaces, they are only half-sized spaces and do not have walls or edges ("#", "-", or "|") that extend the full length of the square. So "." characters are used to ensure the rest of the diagram is aligned properly.

Hopefully, these examples as well as the rest of the map diagrams in this reference are sufficient to help the AI represent, understand, describe, and reason about the map tiles in the game.


### Advanced Map Tile Diagram Features
Some Map Tiles in Shadows of Brimstone feature special terrain features that effect gameplay. This, and other advanced rules elements will be discussed here.

**Barriers**
Barriers represent edges and corners of spaces that are impassabale like a wall, but do NOT block line of sight like a way. Two spaces that share an edge marked as a barrier ARE considered to be adjacent, but models may not move across the barrier unless they have an abilities which allows them to do so. Barriers can be on edges or corners.

The "=" character represents a barrier on the horizontal axis and the "!" character represents a barrier on the vertical axis. The "=" character is also used for barriers that extend into corners and replace where a "+" or a "#" would normally be.

Here is a simple diagram that includes a barrier:

```
....#A02|A03#
#####---+---#####
#B01|B02|B03|B04#
#---+---+---+---#
#C01|C02|C03!C04#
#---+---+====---#
#D01|D02!D03|D04#
#####---+---#####
....#E02|E03#
```

This example shows:
- A barrier on the edge between C03 and C04
- A barrier on the corner shared by C03 and D04
- A barrier on the edge between C03 and D03

In gameplay terms, the following statements would be true about the map tile depicted above:
- A model would not be allowed to move from space C03 into space C04 unless it had a special ability allowing it to do so. This is because even though spaces C03 and C04 are adjacent, they are separated by a barrier.
- A model would be allowed to move from space B03 into C04. Those two spaces are adjacent and they share a corner "+". The corner shared by spaces B03 and C04 is NOT a barrier.
- A model in space C04 does have line of sight to a model in space C02. Even though drawing a line of sight from the center of space C04 to the center of space C02 would cross a barrier, barriers do NOT block line of sight.
- A model would NOT be allowed to move from C04 into space D03 without a special ability allowing it to do so. That's because spaces C04 and D03 are diagnally adjacent and share a corner that is a barrier "=".

**Terrain Anchors**  
Map Tiles in some expansions have icons on the map tiles to indicate possible positions where special terrain features are placed. These are usually placed either on space edges or on space corners. Map Tiles that have these icons will use numbers in the map tile diagram to represent this, placed along the edge or corner where they are located on the real map tile. Outside the diagram, a description will accompany the diagram in the "Special Notes" section to describe what special terrain features are in use and which numbered Terrain Anchors they correspond to.

Here is a simple tile diagram with various terrain anchors added:

```
##############
#A01|A02|A03|A04
#-3-+---+---|-
#B01|B021B03|B04
#---+---######
#C01|C02#
#---2---#
#D01|D02#
```

In this modified version of a corner passage tile there are three terrain anchors. Terrain anchor 1 is located on the vertical edge between spaces B02 and B03. You can tell that this is a terrain anchor because it is a number being placed on the border of a space as opposed to "|" or "#" or "!".

Terrain anchor 2 is placed on a corner shared by spaces C01, C02, D01, and D02. You can tell that this is a terrain anchor because a number is placed in a corner of one or more spaces as opposed to a "+" or "#" or "=". 

Terrain anchor 3 is on the horizontal edge between spaces A01 and B01. You can tell that this is a terrain anchor because it is a number being placed on the border of a space as opposed to "-" or "#" or "=". 

This diagram does NOT represent a real map tile from Shadows of Brimstone and is simply to illustrate the example.

Terrain anchors are most commonly used with the special Cover Terrain game mechanic in the Trederra expansion and the Decayed Trees terrain in the Forest of the Dead expansion. The rules for how Cover Terrain and Decayed Trees work are described elsewhere.

The term "terrain anchor" does not exist in any of the official Shadows of Brimstone rules and was only created for aiding in describing map tiles without the use of images.

This terrain anchor notation is general enough to describe any future special terrain features created for the game. 

Special terrain features that do not need to be marked on space edges or corners can simply be described in a separate Special Notes section following the map tile diagram and reference the space ID's as necessary.

**Tracking Model Positions**  
We can also use map diagrams do display and track the position of models on a map tile. This is done by replacing the space ID inside a space with a model ID. 

Model ID's always start with lower-case letters and are then followed by a two-digit number. Model ID's for Hero and Ally models always start with "@" to distinguish them from Enemy models more easily.

A "Model Key" is then listed after the tile diagram to map the model ID's in the diagram to their names used in game. These are the names of the Heroes, Allies, or Enemies in play.

Here is an example of a map diagram with some models placed on it:

```
.#####################
A01|v02|@02|v03|A05|A06
.--+---+---+---+---+--
v04|@01|v01|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#      
.......#D03|h01#
```

Model Key:
- @01: Ellie (Rancher Hero)
- @02: Curtis (Prospector Hero)
- v01: Void Spider (Ellie)
- v02: Void Spider (Curtis)
- v03: Void Spider (Curtis)
- v04: Void Spider (Ellie)
- h01: Hell Bat (N/A)

In this diagram we can see that there are 7 models on the T-Junction tile. The model key tells us which model maps to which unit. We can see that there are two hero models named Ellie and Curtis and they are being surrounded by a total of 4 Void Spider enemies. Doorway D has a Hell Bat ready ready to join the fight as well.

The Model Key lists the Name of the Hero and then the Hero Class in paranthesis for each hero. This convention should always be followed. 

The conventions used for Enemies are as follows:
- Enemies always start with a lower-case letter, followed by two digits.
- All Enemies of the same TYPE (e.g. "Void Spider", "Hell Bat" "Bandit", etc.) share the same lower-case letter.
- The letter used in the ID for each Enemy type should match the first letter of the Enemy Type (e.g. "v" for "Void Spider") as it can be a helpful mnemonic for humans. If assigning the first letter of the Enemy Type is not possible because another Enemy Type is also on the tile using that letter, then any other available letter can be used.
- In parentheses, each enemy listed should list which Hero/Ally they are currently "targeting" for gameplay purposes. The rules for targeting are not described in this section. Enemies that do not currently have a target should just put (N/A) as their target.

In the above example, you can see that Ellie and Curties each are being targeted by two Void Spiders, while the Hell Bat has not yet chosen a hero to target.

Note that even though the space ID's for some spaces have been replaced by model ID's, we still know what the space ID's are because they are determined by counting columns and rows in the diagram. We know that Curtis is in space A03 because he is positioned in the top most row ("A") and the 3rd column to the right ("03"). When discussing this situation in a gameplay session, we can refer to this as space A03 or "Curtis' space" or the "position of @02", etc.

**Extra Large Models**
XL and XXL models (Extra Large) stand on bases that are too large to fit in a single space. XL models occupy a 2x2 area of spaces and XXL models occupy 3x3 spaces. Tracking these models in a map diagram is simply done by using the same model ID within each space the model occupies. 

For example, placing the XL sized "Living Statue" enemy on the T-Juction square might look like this:

```
.#####################
A01|l01|l01|A04|A05|A06
.--+---+---+---+---+--
B01|l01|l01|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#      
.......#D03|D04#
```

Model Key:
- l01: Living Statue (N/A)

In the above diagram, you can see that the Living Statue occupies spaces A02, A03, B02, and B03.

The game rules allow Extra Large models to "OverFlow" the game board so that it part of the base hangs off the edge of a map tile. If at the end of its movement, and extra large enemy can fit at least half of its base onto valid spaces on the tile that are not occupied by other models, the rest of the model is allowed to "OverFlow" off the edge of the tile. For 2x2 XL Enemies, this means that it is allowed to fit into just 2 spaces, and for 3x3 enemies, it must fit into at least 5 spaces. 

When representing Extra Large Enemies on a diagram that are OverFlowing the board, it is unnecessary to notate any of the OverFlow parts of the model in the diagram. Simply notate in the Model Key that it is currently "OverFlowing" it's current position. 

Here is an example of an XXL Enemy OverFlowing on the T-Junction Tile:

```
.#####################
A01|o01|o01|o01|A05|A06
.--+---+---+---+---+--
B01|o01|o01|o01|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#      
.......#D03|D04#
```

Model Key:
- o01: Oni Warlord (N/A, OverFlowing)

In the above example we have the Oni Warlord position on the T-Junction tile. The Oni Warlord is an XXL sized enemy, that normally takes up 9 spaces in a 3x3 area. However, there is no area large enough to fit the Oni Warlord on this tile, so it can only occupy spaces on the tile if it can fit at least 5 of its normal 9 spaces somewhere on the tile. In this case, the Oni Warlord occupies 6 spaces which are A02, A03, A04, B02, B03, and B04. The enemy is marked in the model key section that it is OverFlowing, and presumably the rest of the models base is sticking out past the walls to the north of spaces A02, A03, and A04.

**Tracking Facing for Models**
Some XXL sized Enemies have special rules for "Arcs" which require knowledge of which direction the Enemy is facing. The rules for Arcs are not described here, but for the rare cases that it is necessary to notate in a diagram the direction that a model is facing, it can be done most easily by adding a cardinal direction within the parenthesis in the Model Key.

In the previous example with the Oni Warlord, if we wanted to describe the Oni Warlord as "facing" spaces C03 and C04, we would modify the Model Key to read:

Model Key:
- o01: Oni Warlord (N/A, OverFlowing, Facing: S)

This would indicate the the "front" of the model is facing South. This would put spaces C03 and C04 in it's "front" arc, and spaces A05 and B05 in its "left" arc. 


## Combining Map Tiles in a Diagram
We can also represent two separate map tiles combined together when the doorway spaces of both tiles are connected. This could allow us to play the game purely within a text based conversation with an AI randomly picking map tiles as the Heroes explore and updating the diagram.

To illustrate how to connect a new map tile to an existing one, we will go through the process step by step. 

First, we start with the Entrance tile, which usually the first tile placed at the beginning of a new adventure:

```
....#A02|A03#
....#---+---#
....#B02|B03#
....#---+---#
....#C02|C03#
#####---+---#####
#D01|D02|D03|D04#
#---+---+---+---#
#E01|E02|E03|E04#
#---+---+---+---#
#F01|@01|@02|F04#
#---+---+---+---#
#G01|G02|G03|G04#
#################
```

Model Key:
- @01: Ellie (Rancher Hero)
- @02: Curtis (Prospector Hero)

You can see that I have placed the two heroes from a previous example (Ellie and Curtis) onto one of the 8 valid starting spaces of the map entrance tile. We will add these heroes to our diagrams in this step-by-step example as we simulate them exploring the Mines.

Elle and Curtis take a few turns moving, and in a later turn, end their activations with Curtis "looking through the door" out of Doorway A during the exploration step. 

Their update positions look like this:

```
....#@02|A03#
....#---+---#
....#B02|@01#
....#---+---#
....#C02|C03#
#####---+---#####
#D01|D02|D03|D04#
#---+---+---+---#
#E01|E02|E03|E04#
#---+---+---+---#
#F01|F02|F03|F04#
#---+---+---+---#
#G01|G02|G03|G04#
#################
```

Model Key:
- @01: Ellie (Rancher Hero)
- @02: Curtis (Prospector Hero)

You can see that when we re-drew the map tile to show the updated positions of Curtis and Ellie, we set the space ID's of the spaces they occupied in the previous version of the diagram back to the normal space ID's of F02 and F03. Curtis now occupies space A01 in the doorway and Ellie is straggling behind just a little in space B03. 

During the exploration step when Curtis looks through the door, a random map card is drawn from the Mines Map Card Deck. The card is revealed to be the T-Juction passage tile, which looks like this:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```

So in order to show an updated diagram, we need to connect the T-Juction tile to the Entrance tile. 

First, we determine which doorway the new T-Juction tile should be connected to on the Entrance tile. The correct doorway is always the doorway that the Hero who took the "look through the door" action is currently standing on. In this case, Curtis took the "look through the door" action and he is standing on Doorway A of the entrance tile. 

Next, we need to determine which doorway on the newly drawn map tile (the T-Junction tile in this case) should be connected to doorway A of the entrance tile. The correct doorway on the T-Junction tile is doorway D. We know this is true because as previously discussed, doorway D is the "entrance" doorway on the T-Juction tile. We know doorway D is the entrance doorway instead of doorway 1 and doorway 6 because doorway D is the southern most doorway depicted in the map tile diagram.

Next we need to determine if the depiction of the new map tile (in this case the T-Junction tile) needs to be rotated 90 degrees to the left or right before connecting it to the previous tile. In this case, we know we do NOT need to rotate the T-Junction tile, because the direction of the entrance doorway on the new map tile (T-Junction doorway D) already aligns with the tile that the Hero who is exploring is standing on (Entrance tile doorway A). They are both on a vertical axis. If the Hero who took the explore action were instead standing on a doorway that points along the horizontal axis (east or west), we would need to rotate the T-Junction tile so that the doorway D spaces align properly. But in this case, we do not need to rotate the T-Junction tile.

The next step is to ensure that none of the elements on the newly drawn map tile would overlap or not fit when connected to the previous tile due to the geometry of the tiles. If this were the case, we would need to evaluate if the new tile would fit by being rotated and connected using one of the other doorways on the new tile. If there are no possible ways to rotate the new tile and connect it to the existing tile by rotating it, then the new tile is discarded and a different map tile is randomly drawn instead. This processes repeats until a valid map tile which fits is found.

In this case, I know that if I were to connect the T-Juction tile doorway D to the Entrance tile doorway A, there would be no overlapping non-"." characters with any other tiles. I am not aware of an algorithm to determine if this is true ahead of time, but if an AI can discover and create an algorithm it would be helpful.

In the meantime, since I know that there are no overlapping elements from either of the two tiles when connected, I can now draw a new diagram showing the two tiles connected:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
....#@02|A03#
....#---+---#
....#B02|@01#
....#---+---#
....#C02|C03#
#####---+---#####
#D01|D02|D03|D04#
#---+---+---+---#
#E01|E02|E03|E04#
#---+---+---+---#
#F01|F02|F03|F04#
#---+---+---+---#
#G01|G02|G03|G04#
#################
```

Notice that when I connect the two doorways, the walls no longer align properly. This is because the T-Junction tile extends farther left than the Entrance tile. So I'll Need to add a little bit more whitespace around the Entrance tile using the "." so that the doorway spaces align properly. Here is the result:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
.......#@02|A03#
.......#---+---#
.......#B02|@01#
.......#---+---#
.......#C02|C03#
...#####---+---#####
...#D01|D02|D03|D04#
...#---+---+---+---#
...#E01|E02|E03|E04#
...#---+---+---+---#
...#F01|F02|F03|F04#
...#---+---+---+---#
...#G01|G02|G03|G04#
...#################
```

That alignment looks much better. You'll notice that the doorway spaces where the two tiles connected however are larger than standard size. This does not happen with the real life physical copy of the game, but is caused because of the way we translate the visual information to text. 

So the last thing we need to do to clean up the tile is to resize the connected doorway spaces to the correct size. So the connected tiles would look like this now:

```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#@02|A03#
.......#---+---#
.......#B02|@01#
.......#---+---#
.......#C02|C03#
...#####---+---#####
...#D01|D02|D03|D04#
...#---+---+---+---#
...#E01|E02|E03|E04#
...#---+---+---+---#
...#F01|F02|F03|F04#
...#---+---+---+---#
...#G01|G02|G03|G04#
...#################
```

You'll notice that the space ID's from the previous tile (the entrance tile) were kept, but the space ID's for the new tile were removed. This convention should always be followed for consistency. Note that even though we used the space ID's from the entrance tile, spaces A02 and A03 are considered to be a part of BOTH the entrance tile and the T-Junction tile for gameplay purposes. In the above example, Curtis is standing on space A02. If an Encounter card were drawn that affected all heroes on the T-Juction tile, only Curtis would be affected because he is currently standing on both tiles. If the event affected the Entrance tile, BOTH Curtis AND Ellie would be affected because Ellie is ONLY standing on the entrance tile and Curtis is standing on BOTH the entrance tile AND the T-Junction tile.

Notice that we also do not change the space ID's on the entrance tile due to the fact that all of the spaces have shifted one space to the right so that the two tiles are properly aligned. Even though space D01 is not the left most space on the entire diagram (normally 01 would be part of the left-most column), space D01 is still the left most space *on the Entrance map tile*. When depicting multiple map tiles connected together in a diagram, the space ID's are always determined in relation to the *tile* it appears on, NOT the entire diagram.

Also note that we can still infer that spaces A01 and A02 on the entrance tile are also spaces on the T-Junction tile due to the way the space ID's jump from row C on the T-Juction tile to row A. 

Finally, you should note that the diagram now has multiple spaces with the same space ID. So when we have multiple tiles displayed in the diagram, we will now have to specify which of the two tiles we mean whenever we use space ID's.

**Example of Rotating A Tile**
This section has yet to be written.

**Cleaning Up Previously Explored Tiles**
This section has yet to be written.


## Map Tile Metadata
The following additional meta data is included with each Map Tile entry:

### Name
This is the thematic name of the tile as listed on the Map Deck card corresponding to the tile.

### Advanced
Some Map Tiles are considered "Unique" and have a corresponding Advanced Encounter card which corresponds to the unique Map Tile. This is a unique Encounter card that thematically links to the artwork on the tile itself, creating an event that is more thematically grounded to the artwork. Using Advanced Encounters is an optional rule in the game rules. The title of the advanced Encounter card will be listed here.

### Description
This is a text description of the artwork depicted on the tile. It is intended to be useful to an AI when acting as a Game Master and Story Teller than can reference the artwork on Map Tiles to generate narrative during an adventure, and also help to generate custom Encounters which match the tile.

Note that any description of terrain, objects or other elements in this section has no gameplay effects but are purely thematic. Any special gameplay effects will be described in the Special Notes section if necessary.

### ID
The physical Map Tiles were not manufactured with any ID markings on them across the entire product line of the game. This can make storing and organizing large amounts of tiles difficult for a large collection. It is common for fans of the game to create their own ID system and give each tile a unique ID written by hand onto the tile itself, as well as the Map Deck card which corresponds to it. This can make the physical tile much easier to quickly locate in a file cabinet during gameplay. I have created my own ID system for this purpose. 

I have labeled each related Map Tile, Map Deck card, and Advanced Encounter card with the same ID for easier location. Both sides of the Map Tile are labeled with the same ID, and so the corresponding Map Deck card and Advanced Encounter card (if any) for both sides all share the same ID. Because of this, two entries will be listed with the same ID, but they will be listed in different sections (one in Belly of the Beast and the other in Forbidden Fortress section for example), they will have different diagrams due to the tile likely being rotated/oriented differently, and they will have different advanced encounters and names.

Entrance, passage, corner, cross, and t-junction tiles do not have IDs.

The ID is a simple two-digit number with a 3-letter prefix. The 3-letter prefix helps me identify the World/Setting/Expansion that the tile belongs to. My 3-letter prefixes correspond to settings as follows, with the setting on the reverse side of the tile in parentheses:

- BOB: Belly of the Beast (Forbidden Fortress)
- FOD: Forest of the Dead (Forbidden Fortress)
- TAR: Targa Plateau (Mines)
- JAR: Swamps of Jargono (Mines)
- BLA: Blasted Wastes (Mines)
- TRE: Trederra (Mines)
- CYN: Caverns of Cynder (Mines)
- DER: Derelict Ship (Mines)
- PRO: Promo Tiles not sold in retail, can come from any setting.

Unique Map Tiles included in Mission Packs do not have an ID.

Including the information on how I organize my Map Tiles may make an AI better able to assist me during gameplay, but this ID system is not part of the official product and is something that I have done to modify my own game.

### Special Notes
A small number of Map Tiles may have unique gameplay elements, such as areas that may provide Cover in Trederra and Forest of the Dead. Any additional special gameplay notes that the tile may have will be added to this section.

### Entrance and Passage Tiles
Entrance and passage tiles are largely the exact same layout across all Core Sets, Adventure Sets, and Expansions, and have no gameplay differences. Therefore, these tiles will only be described once even though a set of Entrance and passage tiles are included in most sets. If any set does come with unique passage tiles that either have a unique layout or gameplay elements printed on the tile (Barriers, Cover, etc.), they will be listed as their own entry.

## Entrance, Passages, and End Cap Tiles

### Entrance

```
....#A02|A03#
....#---+---#
....#B02|B03#
....#---+---#
....#C02|C03#
#####---+---#####
#D01|D02|D03|D04#
#---+---+---+---#
#E01|E02|E03|E04#
#---+---+---+---#
#F01|F02|F03|F04#
#---+---+---+---#
#G01|G02|G03|G04#
#################
```


**Special Notes**  
Entrance tiles only have one puzzle-cut door since it is usually placed as the first tile on the table during a mission. Therefore, there are no Entrance spaces oriented on the bottom/south of the Map Tile. For cardinal orientation in this diagram, consider spaces G01-G04 to be along the "south" wall of the Map Tile.

As a general rule (unless Mission rules specify otherwise), the Heroes always begin placed in the space of their choice anywhere in the south-most 8 spaces of the tile. In this case, spaces F01-F04 and G01-G04 are valid choices to initially place a Hero model at the start of a Mission. 


### Corner Passage
**[1-3]:**

```
..##############
A01|A02|A03|A04#
..-+---+---+---#
B01|B02|B03|B04#
..######---+---#
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```

**[4-6]:**
```
##################
# A1 | A2 | A3 | @B
#----+----+----+--
# B1 | B2 | B3 | @b
#----+----########
# C1 | C2 #
#----+----#
# @A | @a #
```

**Special Notes**  
When a corner passage is drawn, a D6 is rolled to determine which direction the corner turns. Diagrams for both directions are shown along with the D6 values to determine the direction randomly. 


### Short Passage
```
          # @B | @b #
          #----+----#
          # A1 | A2 #
          #----+----#
          # A3 | A4 #
          #----+----#
          # @A | @a #
```

### Mid Passage
```
          # @B | @b #
          #----+----#
          # A1 | A2 #
          #----+----#
          # B1 | B2 #
          #----+----#
          # C1 | C2 #
          #----+----#
          # @A | @a #
```

### Long Passage
```
          # @B | @b #
          #----+----#
          # A1 | A2 #
          #----+----#
          # B1 | B2 #
          #----+----#
          # C1 | C2 #
          #----+----#
          # D1 | D2 #
          #----+----#
          # @A | @a #
```

### T-Junction Passage
```
.#####################
A01|A02|A03|A04|A05|A06
.--+---+---+---+---+--
B01|B02|B03|B04|B05|B06
.#######---+---#######
.......#C03|C04#
.......#---+---#
.......#D03|D04#
```


### Cross Passage
```
          #.01.| 02 |
          #----|----|
          # 03 | 04 |
   -------#----|----#-------
  05 | 06 | 07 | 08 | 09 | 10
   --|----|----|----|----|--
  11 | 12 | 13 | 14 | 15 | 16
   -------#----|----#-------
          | 17 | 18 |
          |----|----|
          | 19 | 20 |
```

### End Cap

## Forbidden Fortress

### Burning Room
```
        [1-3]       ----------------
     |*01*|*02*|    | XX | XX | XX |
-----|----|----#----|----|----|----|
| XX | 03 | 04 | 05 | 06 | 07 | 08 |
|----|----|----|----|----|----|----#--
| 09 | 10 | 11 | 12 | 13 | 14 | 15 |*16*
|----|----|----|----|----|----|----|--   [4-6]
| 17 | 18 | 19 | 20 | 21 | 22 | 23 |*24*
|----|----|----|----|----|----|----#--
| 25 | 26 | 27 | 28 | 29 | 30 | 31 |
|----|----|----|----|----|----|----|
| XX | 32 | 33 | 34 | 35 | 36 | 37 |
-----|----|----|----#----|----#-----
                    |*38*|*39*|
```

- **ID:** BOB07
- **Advanced:** Blazing Inferno

**Description**

A rectangular dojo room with no furniture, padded floors, and a floating shelf on the west wall. A folding privacy screen has fallen over in the center of the room, is torn, and splattered with blood. A few blood splatters are scattered on the floor and a long spear is lying on the floor. The northeast corner of the room features a sliding screen door on the north edge of spaces 06, 06, and 08, filled with a blazing fire just outside the threshold into the XX spaces. A burning ceiling rafter has partially collapsed in the northeast corner of the room in spaces 07, 08, and 14. 

## Belly of the Beast

### Synapse Chamber
``` 
         --------------------------
         | XX | 01 | 02 | 03 | XX |
       --|----|----|----|----|----|
      04 | 05 | 06 | 07 | 08 | 09 |
[1-3]  --|----|----|----|----|----|
      10 | 11 | 12 | 13 | 14 | 15 |
       --|----|----|----|----|----|
         | 16 | 17 | 18 | 19 | 20 |
    -----|----|----|----|----|----|--
    | XX | 21 | 22 | 23 | 24 | 25 | 26
    |----|----|----|----|----|----|-- [4-6]
    | XX | 27 | 28 | 29 | 30 | 31 | 32
    |----|----|----|----|----|----|--
    | XX | 33 | 34 | 35 | 36 | 37 |
    ----------#----|----#----------
              | 38 | 39 |
```

- **ID:** BOB07
- **Advanced:** Nerve Bundles

**Description**  
A large open chamber with the usually pink, wet, organic tissue as the walls and floor. There are four large, purple nerve bundles here connected to each other by nerve synapses. Electric pulses vibrate across the nerve bundles and synapses. The large bundles are about the size of a space and are located at the SW corner of space 06, the SW corner of space 13, space 22, and the edge between spaces 30 and 36.