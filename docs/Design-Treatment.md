# Cohort

_Game Design Treatment_

**Designer:** James Cayetano

**Updated:** 10/26/26

<!--
Use this document to explain the game clearly enough for a reader to understand
its intended experience and discuss a first prototype. Expand the same concept
from your one-page treatment. Replace bracketed text with your own writing and
images; remove these drafting comments when the treatment is ready to share.
Write only as much as each section needs. Keep uncertain ideas identified as
proposals. A finished prototype or digital implementation is not needed here.
-->

## Game Concept

<!-- Explain why the working title fits. Mention alternative titles if useful. -->
I wanted the title of the game to represent the gameplay which revolves around controlling a squadron of soldiers that you personally chose. In this case, I went with the word "Cohort" instead of something like "Squad" (a game by that name already exists), "Platoon" seems too big a scale.

<!-- Describe the setting, theme, and story or premise. Identify the characters
or the role the player takes. A game without a story can describe its situation
and player roles instead; do not invent a narrative just to fill this section. -->
The player takes the role of a Mercenary Commander taking command of a squadron of units to fight against another player. The types of units that the player can select range from squads of Rifleman, Gun Emplacements, and even armored vehicles like tanks.

## Gameplay

<!-- Explain the player's objectives, the conflicts or challenges, and how play
succeeds, fails, or ends. Describe the recurring decisions and actions, the rules
that connect them, and what changes in the game as a result. Game state means the
current situation, such as positions, resources, score, or available choices.
Describe the intended experience through those interactions. -->
Each player controls a squadron of units that will be deployed onto a field consisting of 4 Spaces called [Ranks].
[Ranks] on the field are numbered 1-4, scaling upward depending on what side each player is on, visualized below:

- Player 1    4-3-2-1 |CENTER| 1-2-3-4    Player 2

Units will take 1-3 [Ranks], depending on Unit Type and strength. Players will choose as many Units that can fit onto their side of the field. For example, a player may choose four [Infantry] type Units that take up one [Rank] each, while another may choose a [Vehicle] that takes up 2 [Rank]s, along with two [Infantry] units.

### Setup And Start

<!-- Describe the starting state: how the play area and pieces are arranged,
what each player begins with, and how play starts. Refer to the pieces described
below rather than listing them twice. -->
Players will choose as many Units that can fit onto their side of the field. For example, a player may choose four [Infantry] type Units that take up one [Rank] each, while another may choose a [Vehicle] that takes up 2 [Rank]s, along with two [Infantry] units. Players will create a deck of 6 selected Equipment cards to place in a deck that will be drawn from throughout the match. At the beginning of each [Phase], players draw 1 Equipment Card from a created deck of 6 Equipment cards. A player can hold up to 3 Equipment cards in their hand at max, any more must either be discarded or exchanged with another Equipment card.

### Core Gameplay Loop

<!-- Describe the recurring player choices and actions, the rules that connect
them, and what changes as a result. Game state is the current situation, such as
positions, resources, score, or available choices. -->
Core Loop:
- Each unit can perform an action at least once per [Phase] depending on the specific Unit. 
- After a unit has acted, remove an [Action Token] from the Unit, and then the opponent gets to act with one of their Units.
- After a unit has no more [Action Tokens], it cannot act for the rest of the [Phase]. 
- A [Phase] ends when both players' units have no more action tokens. Upon [Phase] ending, both players' units regain all of their actions back.
- Units Types have access to a shared Action, as well as a unit specific Action, and a unit specific special Action that consumes a resource known as [Order]s.
- [Orders] are a form of Energy that are automatically gained at a rate of 2/Phase, with other sources of [Orders] being certain Unit actions or passives, and Equipment. These [Orders] allow units to perform certain actions and use certain pieces of Equipment. 

### Ending And Outcome

<!-- State when play ends and how the outcome is decided. Include win/lose
conditions where applicable, or another clear beginning/end structure. -->
Play ends when all of the units on one player's side are all defeated. A player loses if all of their units are defeated, and wins if at least one of their units survives when all of their opponents' units are down.

## First Physical Prototype

<!-- Describe the planned physical play area and its pieces or materials, such as
boards, cards, tokens, dice, or a score sheet. Use only what this game needs.
Explain what the pieces represent and how a player uses them to try the core
loop. This is a feasible plan, not a finished prototype or playtest result. -->
Planned Prototype would contain a simple board to represent the play field, marked with spots denoting [Rank] spaces. Cards to represent Units and Equipment, and Tokens to represent Actions Taken, Orders (Energy) in player's possession, Damage Taken, and Armor Shredded. Explanation can be found below in Pieces and Purposes.

<!-- Describe the planned or current physical play area. Mark pieces that have
not been made as planned, and update this section as the prototype develops.
A plan can be described before the prototype is built. -->
Pieces that haven't been made yet:
- Extra Unit Cards
- Dice to track Health instead of Tokens(?)

### Pieces And Their Purpose

<!-- Add a row for each type of piece or material the game actually needs.
Examples include boards, cards, tokens, dice, counters, or a score sheet.
Explain what each represents and how a player uses it; give a quantity when
needed for setup. Repeated copies of the same piece can share one row. -->

| Piece or material | Quantity for setup | What it represents | How it is used |
| --- | --- | --- | --- |
| Green Token | 14 | Action Token | Marks how many ACTIONs a Unit has left in the current [Phase]. Minimum 1 per Unit unless stated other wise (ex. Main Battle Tank gets 2 Actions per phase) |
| Gold Token | 16 | Orders | Gained at a Rate of 2 ORDERs per [Phase]. Can hold up to a MAX of 6 ORDER Tokens, any further ones are discarded. |
| Red Token | Fifteen 1's, Fifteen 2's, Ten 5's, Ten 10's | Damage Token (1/2/5/10) | These tokens represent how much Damage a Unit has taken, rather than their current health. For example: Unit with 8 HP has a 1 and 2 [DAMAGE Token], then that means they have taken 3 total damage, and their current health is: 8 - (1 + 2) = 5 HP. If a Unit has [ARMOR], Damage taken is reduced by the amount of [ARMOR] the unit has, but cannot be reduced below 1. For example: Unit with 30 HP + 5 Armor gets hit with an attack dealing 4 Damage, damage taken is reduced by armor to a minimum of 1. So damage becomes: 30 - (5 Armor - 4) = 30 - 1 = 29 HP left. When restoring health/removing [DAMAGE Token]s, if a Unit has a 5 [DAMAGE Token], and a Medic heals for 2, swap the 5 token for a 1 and 2 Token, becoming 3 Damage taken. |
| Grey Token | 10 | Armor Shred Token | Some Units and Equipment have the ability to [SHRED] Unit armor. Similar to DAMAGE Tokens, these tokens represent how much damage a Unit's armor has taken. For example: Unit with 2 armor has a 2 [SHRED] token, meaning their current armor is now: 2 - 2, meaning the Unit is now unarmored. |
| Unit Card | 28 [2 Copies of 14 Cards] | Unit Card | Used to denote the Unit a player has chosen to deploy on the field, displaying their Health Points, Armor (if applicable), and Unit Specific Actions |
| Equipment Card | 20 [2 Copies of 10 Cards] | Equipment Card | Used to show the Equipment card drawn by a player and held in hand, displaying their effects and cost to use. |
| Marked Board | 1 | Game Field | To help players organize their cards on the field and how movement works. |

### Materials And Mechanic Adjustments

<!-- Explain which materials are created, adapted, or reused and why they work
for this prototype. Describe how rules, values, layouts, or pieces can be changed
between playthroughs without rebuilding the whole prototype. Focus on usable,
readable materials and actual design choices. -->
Most of the materials with be printed on paper, tokens may be replaced with Poker Chips in the future. Unit and Equipment Cards will eventually be replaced from regular printer paper to photo paper.

## Intended Players

<!-- Identify the intended audience's relevant interests and play habits.
Explain why this game's decisions, theme, or intended experience would appeal
to those players. Connect the audience to specific design choices. -->
This is designed for players who like strategic TCG style games, RTS games as well as deckbuilders who enjoy theorycrafting. It would appeal to them as they could experiment with teams and strategies on what they think they will enjoy, be it related to a theme or trying to build the most effective team.

## Accessibility And Inclusivity

<!-- Explain concrete ways people with different abilities can perceive,
understand, and use the game's actual interactions. Explain how these choices
preserve the intended gameplay and can carry into the later digital version.
Choose considerations relevant to this game; a generic feature list is not enough. -->
Unit Actions will be displayed on their card for readability, health and armor being clearly denoted. The Damage Tokens will have a Heart around the Number, with Shred Tokens having a Broken Shield as a decal. Action Tokens will have a Lightning Bolt decal, and Orders will look like a Medal. And to ensure that there is no confusion, a Legend sheet will also be provided for players to look for for reference. This allows for players to distinguish tokens even if color differences are difficult to perceive. The game's play field consists of only four ranks per side and uses simple numerical positioning, reducing the amount of complexity players must track. Players may freely inspect cards, unit information, and public game states at any time, ensuring that information is not hidden behind memory requirements.

## Unique Selling Points (USP)

<!-- Unique selling points are the distinctive design choices that give intended
players a reason to choose this game. Explain those choices through a relevant
comparison with an existing game. Connect the differences to the intended
players' experience; support the comparison with concrete design details.
Explain why the difference would make play more interesting to those players. -->
Cohort uses the tactical positioning of units in a military setting, similar to the dungeon crawler game "Darkest Dungeon". In comparison however, players must decide how to position Infantry, Vehicles, and Emplacements within only four battlefield ranks while managing limited Actions, Orders, and Equipment Cards. This creates meaningful tactical decisions without requiring a large play area or complex setup.

## Concept Pitch

<!-- Bring together the concept, theme, intended audience, player experience,
and strongest USP in a concise pitch. Summarize the earlier sections rather
than repeating their full details. -->
Cohort is a competitive PvP military strategy game where two players command squads of Infantry, Vehicles, and Emplacements across a four-rank battlefield. Designed for players who enjoy tactical combat and resource management, the game emphasizes positioning, unit synergies, and command decisions rather than luck alone. Through a combination of Order generation, Equipment Cards, and unique unit abilities, players must adapt their battle plan to overcome their opponent.

## Visual Direction

### First Sketch Or Storyboard Panel

<!-- Embed a readable sketch or storyboard image showing an important part of
the concept, style, space, or player interaction. Use Markdown image syntax with
your image's actual path. The caption explains what the image represents and how
its visual choices support the theme or intended player experience. -->
<img width="1024" height="768" alt="RanksSystem" src="https://github.com/user-attachments/assets/92b08f1d-6746-426e-b7f0-fdf6203a79bb" />

**Caption:** This Image displays how the [Rank] positioning System works. Here, Player 1 has a Tank Unit that takes up [Ranks 2-4], leaving only 1 free [Rank] space left, which is filled by an Infantry Unit. Player 2 has an Emplacement in [Rank 4] , with a Vehicle taking up two [Ranks], those being [Ranks 2 - 3]

### Second Sketch Or Storyboard Panel

<!-- Use a different image that adds information, such as another interaction,
space, or moment. A second view should help the reader understand another part
of the design. Connect its visual choices to the theme or player experience. -->
[Insert the second sketch or storyboard image.]

**Caption:** [Explain the distinct information this image adds and why its visual choices fit the game.]

## Feedback And Revisions

<!-- Record feedback from three different people, preferably intended players.
Use initials or a first name and the person's relationship to you; omit private
contact details. Each entry identifies a specific observation about the concept,
mechanics, or style and the revision or next test it prompted. Record feedback
that actually occurred, and distinguish a proposed change from a completed one. 
Give actionable observations about the concept, mechanics, or
style. Explain the change or next test each observation prompted and its effect
if tried. If a suggestion is not adopted, explain the design reason and how the
underlying concern is addressed. Distinguish planned changes from completed ones;
record only feedback and outcomes that actually occurred. -->

| Reviewer and relationship | Specific observation | Revision or next test |
| Reviewer and relationship | Specific observation | Response and effect on the design |
| --- | --- | --- |
| Avery C. - Best Friend | [Observation] | [Revision or next test] |
| Derek P. - TTRPG Friend | "Looks simple enough to understand at first, just needs some clarifications in some places." | Ensure that Rules are thoroughly explained and understandable. |
| Rus S. - TTRPG Friend | "Seems fairly balanced at a glance." | Playtest combat to adjust HP, Damage, and economy. |
| [Person 1] | [Observation] | [Change or next test, reason, and effect if observed] |
| [Person 2] | [Observation] | [Change or next test, reason, and effect if observed] |
| [Person 3] | [Observation] | [Change or next test, reason, and effect if observed] |

## Physical Prototype Demo Plan

<!-- Plan a concise demonstration using the presentation's assigned time cap.
Show the actual pieces, a representative interaction, and how the game ends or
reaches its outcome. Make the strongest USP and a concrete feedback-driven change
clear. Keep this as planning notes, not a second treatment or a full script. -->

**Presentation time cap:** 5 Minutes

| Segment | What to show or explain | Planned time |
| --- | --- | --- |
| Introduction | Core concept and strongest USP | 1 Minute |
| Prototype | Pieces, their meaning, and how players use them | 1 1/2 Minutes |
| Gameplay | A representative interaction and the ending or outcome | 2 Minutes |
| Feedback | A concrete design change and why it was made | 30 Seconds |

**Planned total:** 5 Minutes
