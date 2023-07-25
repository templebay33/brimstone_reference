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
Map Tiles can be displayed as a grid of spaces forming colums and rows. The grid for each tile will be displayed in a code block element. Each space will be assigned a unique two digit ID number so that it can be referred to via text descriptions. 

Since each Map Tile has a designated edge of puzzle-cut spaces that are considered the Entrance spaces of the tile when placing them on the table, all Map Tile diagrams will be oriented with the Entrance spaces on the bottom/south of the diagram. This will allow cardinal directions to be used in text descriptions since south will always point to the bottom of the diagram.

Puzzle-cut spaces that are used for connecting to additional Map Tiles and represent open doorways during gameplay will have their ID number displayed in *italics*.

Map Tile cards designate which results on a D6 roll correspond to which puzzle-cut spaces on the tile so that doors and gates can be randomly determined. The puzzle-cut spaces will have a range of numbers within [square brackets] adjacent to them, indicating which values on a D6 roll correspond to that doorway.

Dashes and vertical pipes will represent black bordered walls and grid edges of spaces.

Spaces that have less than 50% of their volume covered in artwork are not considered valid gameplay spaces. Knowing where this spaces are is still useful for knowing where the walls are. These spaces do not require a unique ID and will be shown as "XX".

Some spaces have black wall borders that cover one or more of their edges or corners. This can block Line of Sight to some other spaces and is important to know. Spaces that have one or more of their corners blocked will have the corresponding wall corner marked with a pound/hash # in place of a dash where the corner is that is blocked.

Barriers are thick white lines that block most movement across them but not Line of Sight. Each side/edge of a space that contains a Barrier will use equal signs = instead of dashes to indicate a Barrier horizontally, and use exclamation marks ! instead of vertical pipes to indicate Barrier lines vertically.

Any additional unique elements on a Map Tile that are important for gameplay purposes will be described outside of the diagram.

Note that Entrance spaces on either side of the same Map Tile usually do not share the same edge. Therefore each side of the same Map Tile will be listed as a completely separate Map Tile with its own diagram.

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