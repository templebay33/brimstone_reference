# Shadows of Brimstone AI Generation Guidelines
This reference contains guidance for an AI in generating Shadows of Brimstone content during play. Each section has its own details to help guide an AI in generating fun and interesting content for the game, depending on the type of content it is asked to generate. It should be used in tandem with the other data about the game such as the rules, details of Hero Classes, Missions, Map Tiles, Lore, etc. Ideally, all of this information will be either loaded into a temporary context window for the AI to use or be a part of an AI's training data during fine-tuning.  

## Hero Character Creation
An AI generating a Hero characer should follow this procedure step-by-step, outputting the result of each step along the way. Each step is numbered and has a name. 

1. Select Class:   
  When asked to create a Hero character, the AI should start by picking the Hero Class/Sub-Class of the character. If a specific Class/Sub-Class is not requested, then the AI can pick randomly or however it likes among those it knows about and has all of the data for. The AI should NOT pick a Hero Class/Sub-Class that has missing or incomplete data in the "Shadows of Brimstone - Hero Reference". If the request to generate a character is within the context of a campaign or role-playing session, it would make sense to pick a Hero Class/Sub-Class that is native to the world/setting being played. The AI may choose pick a Hero Class/Sub-Class that is not native to the same world as other Heroes in the campaign, but should develop a narrative reason for how such foreign/alien characters ended up joining the party of Heroes when they are from a different world. If the AI is asked to create a Hero character within the context of a role-playing campaign, the most important factor should be a Class/Sub-Class that thematically ties in with the rest of the current context as far as story, setting, narrative, etc.

2. Select Starting Upgrade:  
Once a Class/Sub-Class is created, the AI should follow the rest of the game rules in creating the Hero. The AI should pick a starting upgrade of its own choosing or pick randomly. The AI may want to pick a starting upgrade that compliments other Heroes in the campaign if that is relevent, but that is not necessary as it can be fun to go for non-obvious choices sometimes.

3. Draw Personal Item:  
A Personal Item should be picked randomly from the appropriate Personal Item deck according to the rules. Ensure you are not picking a Personal Item card that you want. If necessary, create a table with one entry per Personal Item and roll a die on the table to pick.

4. Select Side Bag Token:  
A side bag token can be picked from among those available for starting Heroes (the restricted list of available side bag tokens is covered in the Rules Compliation) according to whatever seems thematically or strategically appropriate to the AI.

Once all the standard steps from the game rules have been followed to create a new Hero, now comes the fun part that AI's are particularly adept at: adding narrative and role-playing flavor!

Throughout the rest of this process, the AI should make use of the "Shadows of Brimstone - Lore Reference" where possible to interweave as much of the characters generated narrative elements into the rest of the lore already present in the game. Making use of any snippest of lore related to the Hero Class itself and the native world/setting they come from are especially recommended.

5. Name the Hero:  
Next the AI should name their Hero. Remember that ANY Hero Class/Subclass in the game can be either Male or Female gendered. When picking a name, use the format: <First Name> <Nickname> <Last Name> with the nickname in quotes. This should be the full name of the character. An exception are tribal and alien characters, that can follow whatever seems thematically appropriate. But if a tribal or alien name is likely to be difficult to pronounce for the players, the AI should also add nickname to the tribal/alien Hero so the player can use it as a short-hand if desired.

Next its time for backstory and character personality development.

6. Create Nickname Origin:  
First create a short backstory of why they have the nickname that was chosen. That backstory should be a short paragraph and reflect the thematic tone of the character.

7. Generate Connection to Personal Item:  
Next create a short paragraph explaining the emotional/sentimental connection the character has to their randomly drawn Personal Item card. Keywords on the Personal Item and the thematic flavor of the game effects are good inspirations to explain how the Hero acquired the item and why it is important to him/her.

8. Generate Adventurer Origin Story:  
Next create a short paragraph explaining how or why the Hero became an adventurer. This can be considered a short "origin" story. If there are other Heroes already in the party, include how they met one or more other Heroes in the party to form a narrative chain of how the party formed.

9. Generate Adventuring Motivations:  
Next create a short paragraph describing the Hero's motivations during the campaign. Are they trying to hunt down a particular enemy and get revenge? Are they trying to get rich? Maybe the seek ancient and forbidden knowledge? Some kind of motivation that keeps the Hero willing to keep putting themselves in harms way and answer the call of adventure!

10. Generate Personality Quirk:  
The next step is to create a personality quirk for the character. This can be described in just a single sentence or two. Are they afraid of Void Spiders? Allergic to fauna in the Swamps of Jargono? Maybe they are addicted to gambling and keep risking it all whenever visiting a Gambling Hall. Whatever the quirk is, it can be used for fun role-playing opportunities if the AI continues to make decisions and role-play on behalf of the Hero.

11. Render Full Character Sheet:  
The final and last step when the AI is creating a Hero is to take everything generated so far and output a well-formatted and human readable Markdown file of the character so that it can be stored by the player and easily referenced later. The markdown summary that is displayed should include the following elements displayed in the same order:
- The full name and Class/Sub-Class of the character
- A table containing ALL of the information in the Hero Sheet for that Class/Sub-Class (Initiative, Health, Sanity, 6 Skill Attribute Values, etc.)
- A table displaying the current amount of Grit, Dark Stone, Gold, XP, and the current experience Level of the character. The starting Level is 1 and all other resources should be zero except for Grit which starts at 1.
- If playing a Hero Class/Sub-Class that requires tracking current and/or maximum amounts of a special resource, that should be listed next. This could be things like Rage, Ambition, Discoveries, Fury, Faith, or other Class/Sub-Class specific resources. Refer to the "Shadows of Brimstone - Hero Reference" to determine of the chosen Hero Class/Sub-Classes makes use of any of these special resources. If not, move on to the next section
- A section to list all their current Side Bag tokens and starting Side Bag carry limit (which is almost always 5).
- The name and description of the chosen starting upgrade
- The name and description of the randomly drawn Personal Item
- The name and descriptions of each starting gear item the Hero begins with
- The names and descriptions of any Special cards that were required to be chosen for some Hero Classes/Sub-Classes that specifically call for them. This could be things like Samurai Battle Tactics for the Samurai or Gambling Tricks for the Gambler and there are several more examples. Refer to the "Shadows of Brimstone - Hero Reference" to determine of the chosen Hero Class/Sub-Classes makes use of any of these Special cards. If not, move on to the next section
- The backstory of the characters nickname previously generated
- The story of the Personal Item origins previously generated
- The origin story previously generated
- The heroes motiviations and goals previously generated
- The personality quirk previously generated

The final rendered character sheet should use this example sheet as a template:

# Lyle "Deadeye" Jenkins - U.S. Marshal

|  |  |  |  |  |
| :---: | :---: | :---: |  :---: | :---: |
| *Strength* | *Agility* | *Spirit* | Initiative | Level |
| 2 | 3 | 2 | 4 | 1 |
| *Cunning* | *Lore* | *Luck* | Health | Sanity |
| 4 | 1 | 3 | 10 | 10 |
| **Range To-Hit** | **Melee To-Hit**
| 4+ | 4+
| Combat | Max Grit | Defense | Willpower |
| 2 | 2 | 3+ | 4+ |

**Keywords:** *Law, Traveler*
### Abilities
**Double Shot (Shotgun):**  
Once per turn, when you kill an Enemy with a Shotgun, you gain +1 Shot with that Shotgun.

### Starting Upgrade
**Rolling Thunder:**  
Any time you kill an Enemy, you may Recover a Grit on the D6 roll of 4+.

### Personal Item
**Weathered Newspaper**  
*Personal, Paper, News*  
  
  - +1 Lore
  - Whenever the Hero Posse marker moves onto a Blood Spatter or Growing Dread space of the Depth Track, you may Recover a Grit.
### Gear
**Shotgun**  
*Gear, Gun, Shotgun*  
Range: 5  
Shots: 1  
Gold Sell Value: $300  
Weight: 1  
Upgrade Slots: 1  
Hand Slots: Double Handed  
Special Rules: Uses the D8 To Hit and for Damage (6, 7, or 8 count as a Critical Hit). 

**Marshal Badge**  
*Gear, Law, Icon*  
Special Rules: Uses the D8 To Hit and for Damage (6, 7, or 8 count as a Critical Hit).  
Restrictions: Law Only

### Side Bag
- Bandage

## Lyle's Story So Far
This paragraph describes Lyle's origin story.

This paragraph describes how Lyle got his nickname.

This paragraph describes why Lyle's Personal Item is important to him.

This paragraph describes Lyle's personality quirk.

This paragraph describes Lyle's goals and motivations.