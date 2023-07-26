# Shadows of Brimstone - Map Tile Reference
This reference provides information on the Map Tiles throughout all the products in Shadows of Brimstone, including their physical layout. 

This reference is intended to be understood by large language AI models. Currently, such models lack reliable multi-modal capabilities, including the ability to understand data from within images. Because of this, the Map Tiles for the game have had their physical layout described in text format.  


## Visual Description of Map Tiles
The physical Map Tile components are described in this section so they may assist an AI in understanding and tracking how they are physically placed on the table. Using a shorthand text description to describe a particular Map Tile may even help an AI be able to track where models are placed within the squares of the tile during a Fight so as to assist in playing the game.  

The Map Tiles that are included in various Core, Adventure, and Expansion boxes are flat cardboard tiles that take on various 2D shapes and have artwork depicted on both sides of the 2D tile. The different art work on either side of a particular Map Tile correspond to two different World Locations (e.g., one side might be a tile for the Mines, while the other depicts a location in the Swampsof Jargono).

The edges of the map tiles are black bordered walls and almost every Map Tile has at least two puzzle-cut spaces for connecting to other randomly drawn Map Tiles. Entrance Map Tiles and End Caps only have a single puzzle-cut connector space. 

The artwork depicted on the tile is from a top-down perspective and highly evocative to help visually represent the Heroes walking through the location when the Hero miniatures are placed on the tile. The artwork is split up into a square grid, about 1" square, to regulate miniature movement across the tile. Each square on the Map Tile is called a space.  

Some of the black bordered walls and edges of the map tile will bleed into some of the edges on the Map Tile, creates spaces that are partially filled with artwork depicting the location and partially depicting the black bordered wall. Spaces with at least 50% of the square covered by artwork is still considered a valid space for models to occupy.  

Spaces occupied by puzzle-cut edges are also considered valid spaces and may be occupied by models wither there is another Map Tile connected or not. Every puzzle-cut connection on ever Map Tile in Shadows of Brimstone is two spaces wide to ensure that all Map Tiles can be connected to one another.  


## Text Format of Map Tile Layout
The physical layout of Map Tiles can be approximated using text in an ASCII art style similar to those employed by text-based roguelike games such as NetHack. This helps an AI understand and evaluate the physical layout of Map Tiles for gameplay purposes. We will refer to each ASCII art depiction of a Map Tile layout as a Map Tile Diagram. Within this Markdown formatted document, each Map Tile Diagram will be displayed inside a codeblock element to preserve the whitespace needed to properly depict the map tile diagram. 

The following ASCII text characters are used to represent elements of the Map Tile within each Map Tile Diagram:  
- Dashes ("-"): Represent edges of spaces along a horizontal axis. These are normal edges of spaces and two spaces sharing an edge are considered to be adjacent. These space edges do NOT block Line of Sight. These will be referred to a "space edges" or "edges".
- Pipes ("|"): Represent edges of spaces along a vertical axis. These are normal edges of spaces and two spaces sharing an edge are considered to be adjacent. These space edges do NOT block Line of Sight. These will also be referred to a "space edges" or "edges".
- Plus ("+"): Represents corners of spaces where both a vertical and horizontal line intersect.
- Hash/Pound ("#"): These represent walls and correspond to the thich black borders on the real Map Tiles. Two spaces separated by a wall on an edge are NOT considered adjacent. Two spaces that share a corner marked with "#" instead of "+", but do NOT share an edge are NOT adjacent. Walls block Line of Sight.
- Equals ("="): These represent special Barrier terrain on the horizontal axis and replace normal space edges (represented by dashes) when present. Barriers are only found on some Map Tiles. Spaces separated by a barrier are considered to be adjacent but barriers have special rules restricting movement that are explained elsewhere. Barriers do NOT block Line of Sight.
- Exclamation ("!"): These represent barrier edges on the vertical axis and work just like barrier edges on the horizontal axis.
- ID's ("A1", "A2", "B1", etc.): These are located in the center of each space and are not represented on the real Map Tiles in any way. They are added to spaces on the Map Tile Diagrams so that specific spaces can be referred to more easily using text. These are referred to here as "space ID's" or simply "ID's".
- At Sign ("@"): The @ is used for ID's on open door spaces. Each open door space starts with "@" and is combined with either an upper-case or lower-case letter. The two doorway spaces that are adjacent to each other and together define an "open door" use the same letter, one in upper-case and the other in lower-case. This allows both of the two spaces to be referred to individually as spaces based on their case, but we can also refer to the doorway as just a letter. For example, spaces "@A" and "@a" are both separate spaces adjacent to one another that are both part of "Doorway A". 

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

Additionally, the terms "up" and "above" when describing map tile elements mean north or top, which the terms "down" or "below" mean bottom or south.

The terms "edges" and "sides" are interchangeable within the context of map tile elements and both mean a horizontal or vertical line bordering one or more spaces.

The terms "gridlines" or "grid lines" refer to border edges and corners surrounding spaces that are NOT walls.

### Basic Map Tile Diagram Examples
Let's take a look at a few examples of a basic Map Tile Diagram using the symbology that was just defined.

Here is a map tile diagram of a basic corner passage map tile:

```
   ##################
  @B | A2 | A3 | A4 #
   --+----+----+----#
  @b | B2 | B3 | B4 #
   ########----+----#
          # C1 | C2 #
          #----+----#
          # @A | @a #
```

The following statements are TRUE about the above map tile diagram:
- The top-most and right-most edges of the tile are walls because they are designated with "#".
- Spaces C1 and B4 share a corner marked with "+".
- There are two doorways on this tile, doorway A and doorway B
- The distance between @B and C2 is 3 spaces.

Here are some statements that are FALSE aboyut the above map tile diagram with reasons why they are false:
- False Statement: Space B4 is surrounded by walls on all sides.
  Why it's False: For space B4 to be surrounded by walls on all sides, each edge must be marked with a "#". Only the right side of space B4 is marked with "#" so it is not surrounded by walls on all sides.
- False Statement: Space A4 is part of a doorway.
  Why it's False: If space A4 were a doorway, the ID of that space would start with an "@" and it does not. There is a chance the ID could be a mistake or typo, but we can also see that space A4 has either a gridline or wall border on all sides. Puzzle-cut spaces that belong to doorways are always missing borders around half of the space.

**Map Tile Diagram Conventions**  
As you see more map tile diagram examples, you may notice a few conventions that should always be followed when creating, rendering, or drawing map tile diagrams.

The first convention is that the doorway spaces that are further south/bottom in the diagram are always labeled as doorway A. This is because the orientation of how a map tile is rotated when it is placed during gameplay is marked with an arrow on the related Map Tile Card which shows the "entrance spaces". As a shorthand, the map tile diagrams in this document are always oriented so that the entrance spaces are on the bottom for consistency and clarity.

Additionally, always labeling the entrance doorway as doorway A helps with consistency and clarity.

You'll also notice that the ID's for doorway spaces will always use an upper-case letter for the left or top half of the doorway, and a lower-case letter for the right or bottom half of the doorway. This is also for consistency.

You'll also notice that two of the edges of doorway spaces are only half the length of a normal space edge. This helps to visually indicate that these are puzzle-cut spaces in the diagram and that they are half the size of a normal space until they are connected to another Map Tile.

Finally, you should notice that the ID's for spaces always start with A on the north most row and end with 1 on the left most column. Doorway spaces are not counted for this convention as they have their own special ID's starting with @. The numbers in each space ID increase within spaces in an east direction and the letters in each ID go up in alphabetical order as the spaces move in a south direction. This is a very standard convention to notate grids and it is used here so that the correct space ID's can be assumed even when they are not written in the diagram. This convention allows us to make smaller, simpler map tile diagrams which take up less space by removing the need to add space ID's (more on simple map tile diagrams later).

### Advanced Map Tile Diagram Features
Some Map Tiles in Shadows of Brimstone feature special terrain features that effect gameplay. This, and other advanced rules elements will be discussed here.

**Barriers**

This section has yet to be written.

**Terrain Anchors**  
Map Tiles in some expansions have icons on the map tiles to indicate possible positions where special terrain features are placed. These are usually place either on space edges or on space corners. Map Tiles that have these icons will use numbers in the map tile diagram to represent this, placed along the edge or corner where they are located on the real map tile. Outside the diagram, a description will accompany the diagram to describe what special terrain features are in use and which numbered Terrain Anchors they correspond to.

Here is a simple tile diagram with various terrain anchors added:

```
##################
# A1 | A2 | A3 | @B
#-3--+----+----|--
# B1 | B2 1 B3 | @b
#----+----########
# C1 | C2 #
#----2----#
# @A | @a #
```

In this modified version of a corner passage tile there are three terrain anchors. Terrain anchor 1 is located on the vertical edge between spaces B2 and B3. You can tell that this is a terrain anchor because it is a number being placed on the border of a space as opposed to "|" or "#". Terrain anchor 2 is placed on a corner shared by spaces C1, C2, @A, and @a. You can tell that this is a terrain anchor because a number is placed in a corner of one or more spaces as opposed to a "+" or "#". Terrain anchor 3 is on the horizontal edge between spaces A1 and B1. You can tell that this is a terrain anchor because it is a number being placed on the border of a space as opposed to "-" or "#". This diagram does NOT represent a real map tile from Shadows of Brimstone and is simply to illustrate the example.

Terrain anchors are most commonly used with the special Cover Terrain in the Trederra expansion and the Decayed Trees terrain in the Forest of the Dead expansion. The rules for how Cover Terrain and Decayed Trees work are described elsewhere.

The term "terrain anchor" does not exist in any of the official Shadows of Brimstone rules and was only created for aiding in describing map tiles without the use of images.

This terrain anchor notation is general enough to describe any future special terrain features created for the game. Special terrain features that do not need to be marked on space edges or corners can simply be described in a separate text description from the map tile diagram and reference the space ID's as necessary.

**Tracking Model Positions**  
This section has yet to be written.

**Tracking Facing for Models**
This section has yet to be written.


### Simple Map Tile Diagrams
This section has yet to be written.



## Combining Map Tiles in a Diagram
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
     | 01 | 02 |
     |----|----|
     | 03 | 04 |
     |----|----|
     | 05 | 06 |
-----#---------#-----
| 07 | 08 | 09 | 10 |
|----|----|----|----|
| 11 | 12 | 13 | 14 |
|----|----|----|----|
| 15 | 16 | 17 | 18 |
|----|----|----|----|
| 19 | 20 | 21 | 22 |
---------------------
```

**Special Notes**  
Entrance tiles only have one puzzle-cut door since it is usually placed as the first tile on the table during a mission. Therefore, there are no Entrance spaces oriented on the bottom/south of the Map Tile. For cardinal orientation in this diagram, consider spaces 19-22 to be along the "south" wall of the Map Tile.

As a general rule (unless Mission rules specify otherwise), the Heroes always begin placed in the space of their choice anywhere in the south most 8 spaces of the tile. In this case, spaces 15-22 are valid choices to initially place a Hero model at the start of a Mission. 


### Corner Passage
**[1-3]:**
```
   ------------------
  01 | 02 | 03 | 04 |
   --|----|----|----|
  05 | 06 | 07 | 08 |
   -------#----|----|
          | 09 | 10 |
          |----|----|
          | 11 | 12 |
```

**[4-6]:**
```
------------------
| 01 | 02 | 03 | 04
|----|----|----|--
| 05 | 06 | 07 | 08
|----|----#-------
| 09 | 10 |
|----|----|
| 11 | 12 |
```

**Special Notes**  
When a corner passage is drawn, a D6 is rolled to determine which direction the corner turns. Diagrams for both directions are shown along with the D6 values to determine the direction randomly. 


### Short Passage
```
          | 01 | 02 |
          |----|----|
          | 03 | 04 |
          |----|----|
          | 05 | 06 |
          |----|----|
          | 07 | 08 |
```

### Mid Passage
```
          | 01 | 02 |
          |----|----|
          | 03 | 04 |
          |----|----|
          | 05 | 06 |
          |----|----|
          | 07 | 08 |
          |----|----|
          | 09 | 10 |
```

### Long Passage
```
          | 01 | 02 |
          |----|----|
          | 03 | 04 |
          |----|----|
          | 05 | 06 |
          |----|----|
          | 07 | 08 |
          |----|----|
          | 09 | 10 |
          |----|----|
          | 11 | 12 |
```

### T-Junction Passage
```
   -------------------------
  01 | 02 | 03 | 04 | 05 | 06
   --|----|----|----|----|--
  07 | 08 | 09 | 10 | 11 | 12
   -------#----|----#-------
          | 13 | 14 |
          |----|----|
          | 15 | 16 |
```

### Cross Passage
```
          | 01 | 02 |
          |----|----|
          | 03 | 04 |
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