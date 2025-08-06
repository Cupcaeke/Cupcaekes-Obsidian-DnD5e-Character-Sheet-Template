---
level: 1
proficiency_bonus: 
hp: 7
ac: 9
speed: 30
cssclasses:
  - tag-bubble
CL: ""
RACE: 
BG: 
ALIGN: 
PN: 
EXP: 
HI: 
LBS: 
EYE: 
SKIN: 
HAIR: 
PERS: ""
IDEAL: 
BOND: 
FLAW: 
IMAGE: 
ammo1: 
ammo2: 
AC1: true
AC2: false
AC3: false
AC4: false
CP: 
SP: 
EP: 
GP: 
PP: 
TREASURE: 
CARRY: 
SP1-1: false
SP1-2: false
SP1-3: false
SP1-4: false
SP1-5: false
SP1-6: false
SP1-7: false
SP1-8: false
SP1-9: false
SP1-10: false
SP1-11: false
SP1-12: false
SP1-13: false
SP2-1: false
SP2-2: false
SP2-3: false
SP2-4: false
SP2-5: false
SP2-6: false
SP2-7: false
SP2-8: false
SP2-9: false
SP2-10: false
SP2-11: false
SP2-12: false
SP2-13: false
SP3-1: false
SP3-2: false
SP3-3: false
SP3-4: false
SP3-5: false
SP3-6: false
SP3-7: false
SP3-8: false
SP3-9: false
SP3-10: false
SP3-11: false
SP3-12: false
SP3-13: false
SP4-1: false
SP4-2: false
SP4-3: false
SP4-4: false
SP4-5: false
SP4-6: false
SP4-7: false
SP4-8: false
SP4-9: false
SP4-10: false
SP4-11: false
SP4-12: false
SP4-13: false
SP5-1: false
SP5-2: false
SP5-3: false
SP5-4: false
SP5-5: false
SP5-6: false
SP5-7: false
SP5-8: false
SP5-9: false
SP6-9: false
SP6-8: false
SP6-7: false
SP6-6: false
SP6-5: false
SP6-4: false
SP6-3: false
SP6-2: false
SP6-1: false
SP7-9: false
SP7-8: false
SP7-7: false
SP7-6: false
SP7-5: false
SP7-4: false
SP7-3: false
SP7-2: false
SP7-1: false
SP8-1: false
SP8-2: false
SP8-3: false
SP8-4: false
SP8-5: false
SP8-6: false
SP8-7: false
SP9-1: false
SP9-2: false
SP9-3: false
SP9-4: false
SP9-5: false
SP9-6: false
SP9-7: false
---

# **Character Name**

~~~tabs
---General
![[#General|no-h1 full clean]]
---Description
![[#Description|no-h1 full clean]]
---Image Gallery
![[#Image Gallery|no-h1 full clean]]
---Config
![[#Config|no-h1 full clean]]
---Quick Ref.
![[#Quick Reference|no-h1 full clean]]
~~~

~~~tabs
---Abilities
![[#Abilities|no-h1 full clean]]
---Equipment
![[#Equipment|no-h1 full clean]]
---Inventory
![[#Inventory|no-h1 full clean]]
---Spellcasting
![[#Spellcasting|no-h1 full clean]]
---Features & Traits
![[#Features & Traits|no-h1 full clean]]
---Backstory
![[#Backstory|no-h1 full clean]]
---Misc.
![[#Misc.|no-h1 full clean]]
---Notes
![[#Notes|no-h1 full clean]]
~~~


---
---


# General
[[#General|🔗]] 

```event-btns
items:
  - name: Short Rest
    value: short-rest
  - name: Long Rest
    value: long-rest
```
```badges
items:
  - label: Level
    value: '{{ frontmatter.CL }}'
  - label: Prof. Bonus
    value: '+{{ frontmatter.proficiency_bonus }}'
  - label: AC
    value: '{{ frontmatter.ac }}'
  - label: Initiative
    value: '{{ modifier abilities.dexterity }}'
  - label: Speed
    value: '{{ frontmatter.speed }}'
  - label: Inspiration
    value: '[ ]'
```
```healthpoints
state_key: my_character_hp
health: '{{ frontmatter.hp }}'
death_saves: true
hitdice:
  dice: d8
  value: 3
```
> [!column|no-t]
> > [!recite] Consumable 1
> > ```consumable
> > items:
> >  - label: "SP-SD-BI-ETC"
> >    state_key: my_character_consum
> >    uses: 2
> >    reset_on: long-rest
> > ```
> 
> > [!recite] Consumable 2
> > ```consumable
> > items:
> >  - label: "SP-SD-BI-ETC"
> >    state_key: my_character_consum
> >    uses: 2
> >    reset_on: long-rest
> > ```
# Description
[[#Description|🔗]] 

> [!columns|no-t]
> 
> > [!recite|bg-white t-w] Character Info
> > | Info              | Description         |
> > | ----------------- | ------------------- |
> > | **Class & Level** | `INPUT[text(placeholder(Class & Level)):CL]`    |
> > | **Race**          | `INPUT[text(placeholder(Race)):RACE]`  |
> > | **Background**    | `INPUT[text(placeholder(Background)):BG]`    |
> > | **Alignment**     | `INPUT[text(placeholder(Alignment)):ALIGN]` |
> > | **Player Name**   | `INPUT[text(placeholder(Player)):PN]`    |
> > | **Experience**    | `INPUT[text(placeholder(EXP)):EXP]`   |
> 
> > [!recite|bg-white t-w] Character Appearance
> > | Info              | Description         |
> > | ----------------- | ------------------- |
> > | **Age** | `INPUT[text(placeholder(Age)):AGE]`    |
> > | **Height**          | `INPUT[text(placeholder(Height)):HI]`  |
> > | **Weight**    | `INPUT[text(placeholder(Weight)):LBS]`    |
> > | **Eyes**     | `INPUT[text(placeholder(Eyes)):EYE]` |
> > | **Skin**   | `INPUT[text(placeholder(Skin/Fur/Etc)):SKIN]`    |
> > | **Hair**    | `INPUT[text(placeholder(Hair)):HAIR]`   |
> 
> > [!recite|bg-white] Personality Traits
> > `INPUT[textArea(placeholder(Personality Traits or Quote)):PERS]`
> 
> > [!recite|bg-white] Ideals
> > `INPUT[textArea(placeholder(Ideals and Morals)):IDEAL]`
> 
> > [!recite|bg-white] Bonds
> > `INPUT[textArea(placeholder(Bonds and Boundaries)):BOND]`
> 
> > [!recite|bg-white] Flaws
> > `INPUT[textArea(placeholder(Flaws and Fears)):FLAW]`
# Image Gallery
[[#Image Gallery|🔗]]  

```meta-bind
INPUT[imageListSuggester:IMAGE]
```
# Config
[[#Config|🔗]]  

> [!columns|no-t]
> > [!recite|bg-white no-t t-w]
> > | Info                  | Description                       |
> > | --------------------- | --------------------------------- |
> > | **Total Level**       | `INPUT[number(placeholder(Level)):level]`             |
> > | **Proficiency Bonus** | `INPUT[number(placeholder(+X)):proficiency_bonus]` |
> > | **Max Hit Points**    | `INPUT[number(placeholder(Hit Die + CON)):hp]`                |
> > | **Armor Class**       | `INPUT[number(placeholder(Check Equipment for more)):ac]`                |
> > | **Speed**             | `INPUT[number(placeholder(Walking Speed)):speed]`             |
> > Leave **Proficiency Bonus** blank to automatically calculate based on **Total Level**.
> 
> > [!recite|bg-white] State Keys
> > Character sheets each need unique state keys in order to function wherever they appear. You can edit the code blocks where they appear, replacing `my_character` with your character name (Or whatever your preference is! Just *make sure* that the state key is unique across your entire vault). State keys tend to appear wherever there are checkboxes. Specifically, they appear in the `healthpoints` block and the `consumable` blocks.
> 
> > [!recite|bg-white] Ability Scores & Skills
> > Your character's ability scores need to be modified in the `ability` code block under the [[#Abilities]] section. You can also adjust your saving throws under the `proficiencies` section of that code block. Lastly, you can add bonuses (like from items and features) in the `bonuses` section of the code block following the structure provided. You can change your skill proficiencies within the `skills` code block right beneath.
> 
> > [!recite|bg-yellow] Tips and Credits
> > The DnD-UI Toolkit plugin has some bugs with showing abilities and skills in the main tab box as of July 2025. The Initiative badge and Skills block don't render properly at the moment, so you need to click the link button at the top of the General block and Abilities block to see them accurately.
> > If you are struggling with any of the formatting and syntax of this template, check out the docs from the following sources: [Obsidian](https://help.obsidian.md/syntax), [ITS Theme](https://publish.obsidian.md/slrvb-docs/ITS+Theme/ITS+Theme), [DND UI Toolkit](https://hay-kot.github.io/obsidian-dnd-ui-toolkit/), [MetaBind](https://www.moritzjung.dev/obsidian-meta-bind-plugin-docs/).
> > Additionally, if you need to add any new text boxes or in-table check boxes, check the MetaBind plugin documentation (listed above). You will need to add a new unique Property (at the top of the Note) and tie it to the INPUT field you created.
> > Lastly, this Vault comes with an alphabetical Spellbook folder. It is recommended to link your spells in [[#Spellcasting]] to those notes for easy access. Items placed in the Equipment section can also be linked in the [[#Inventory]] section for quick descriptions. Using tags on Features & Traits such as Action, Bonus Action, or Reaction can help sort abilities quicker.
> > This character sheet template was made lovingly by [Cupcaeke](https://cupcaeke.carrd.co). I made this to work as a sort of middle-ground between a good ole pdf/paper sheet and something like DNDBeyond or Orcpub. I hope you enjoy!
# Abilities
[[#Abilities|🔗]]  

```ability
abilities:
  strength: 8
  dexterity: 8
  constitution: 8
  intelligence: 8
  wisdom: 8
  charisma: 8

proficiencies:
  - 
  - 

bonuses:
  - name: 
    target: 
    value: 
    modifies: 
```

```skills
proficiencies:
  - acrobatics

expertise:
```
```badges
items:
  - label: Passive Perception
    value: '{{ add 10 (modifier abilities.wisdom) }}'
```

> [!recite|bg-white t-w ws-med] Other Proficiencies & Training
> | Proficiency Type          | Description         |
> | ----------------- | ------------------- |
> | **Armor** |     |
> | **Weapons**          |   |
> | **Tools**    |     |
> | **Languages**     |  |
> | **Other**   |     |

# Quick Reference
[[#Quick Reference|🔗]]  

**A quick reference for things you can do on your turn, as well as various conditions and effects**
<iframe
src="https://donjon.bin.sh/5e/quickref/"
width="150"
height="300"
style="overflow: auto; resize: both; aspect-ratio: 16 / 9; width: 100%; height: 100%;">
</iframe> 

# Equipment
[[#Equipment|🔗]]  

## Weapons #action

| Item | Range | ATK Bonus | Damage / Type | *Properties / Notes* |
| ---- | ----- | --------- | ------------- | -------------------- |
|      |       |           |               |                      |
|      |       |           |               |                      |
|      |       |           |               |                      |
|      |       |           |               |                      |
|      |       |           |               |                      |

| Ammunition Type | Count                                              |
| --------------- | -------------------------------------------------- |
|                 | `INPUT[number(class(wider),placeholder(0)):ammo1]` |
|                 | `INPUT[number(class(wider),placeholder(0)):ammo2]` |
## Armor

| Equip               | Item      | Type  | AC     | Stealth | *Properties / Notes* |
| ------------------- | --------- | ----- | ------ | ------- | -------------------- |
| `INPUT[toggle:AC1]` | Unarmored | Light | 10+DEX | ---     |                      |
| `INPUT[toggle:AC2]` |           |       |        |         |                      |
| `INPUT[toggle:AC3]` |           |       |        |         |                      |
| `INPUT[toggle:AC4]` |           |       |        |         |                      |
## Attunement Slots

| Slot  | Item | Body Part | Summary |
| ----- | ---- | --------- | ------- |
| **1** |      |           |         |
| **2** |      |           |         |
| **3** |      |           |         |
# Inventory
[[#Inventory|🔗]]  

- **Current Encumbrance**
	- `INPUT[number(class(wider),placeholder(Held)):CARRY]`**lbs**
```badges
items:
  - label: Capacity
    value: '{{ multiply 15 abilities.strength }}lbs'
```

## Coin-purse

> [!recite|wm-sm txt-c t-w table-cell-top] Treasure
> | CP | SP | EP | GP | PP |
> | --- | --- | --- | --- | --- |
> | `INPUT[number(class(wider),placeholder(0)):CP]` | `INPUT[number(class(wider),placeholder(0)):SP]` | `INPUT[number(class(wider),placeholder(0)):EP]` | `INPUT[number(class(wider),placeholder(0)):GP]` | `INPUT[number(class(wider),placeholder(0)):PP]` |
> `INPUT[textArea(placeholder(Treasure)):TREASURE]`

## Carried Items
 - **Tip!** You can *Insert Template* here and select *Item Card Template* to quickly add items. Make sure each item has a unique \^block-id so you can link it later! Items with charges also need unique *state keys*.
 
> [!recite|alt-line txt-s nmg clean collapse nbrd clear bg-yellow]- Item Example
> **Quantity:** 1x
> **Weight:** 0 lbs
> **Item Type:** Weapon, Tool, etc
> ---
**Description.** Here is where you can place your item description.
> ```consumable
> items:
>   - label: "Charges"
>     state_key: my_character_example_item
>     uses: 1
>     reset_on: long-rest
> ```
> ^unique-item-ID


## Other Storage (Bag Of Holding, etc)
- **Capacity:** X lbs
# Spellcasting
[[#Spellcasting|🔗]]  

```stats
items:
  - label: Spellcasting Class
    value: 
  - label: Spellcasting Ability
    value: 
  - label: Spell Save DC
    value: '{{ add 8 frontmatter.proficiency_bonus (modifier abilities.intelligence) }}'
  - label: Spell Attack Bonus
    value: '+{{ add frontmatter.proficiency_bonus (modifier abilities.intelligence) }}'

grid:
  columns: 4

dense: true
```

> [!recite|t-w]- Spellcasting Focus
> | Name | Type | Properties & Notes |
> | ------ | ----- | -------------------- |
> |  |  |
> |  |  |
> |  |  |

> [!columns|no-t nmg] Spell List
> > [!recite|t-w] Cantrips
> > | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ------------- | ------- | --------- | ------------- |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
> > |  |  |  |  |  |
>
> > [!recite|t-w txt-s nmg] 1st Level
> > > [!recite|txt-s alt-line] LV1 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV1"
> > >     state_key: my_character_SPL1
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP1-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-9]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-10]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-11]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-12]` |  |  |  |  |  |
> > | `INPUT[toggle:SP1-13]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 2nd Level
> > > [!recite|txt-s alt-line] LV2 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV2"
> > >     state_key: my_character_SPL2
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP2-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-9]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-10]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-11]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-12]` |  |  |  |  |  |
> > | `INPUT[toggle:SP2-13]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 3rd Level
> > > [!recite|txt-s alt-line] LV3 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV3"
> > >     state_key: my_character_SPL3
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP3-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-9]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-10]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-11]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-12]` |  |  |  |  |  |
> > | `INPUT[toggle:SP3-13]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 4th Level
> > > [!recite|txt-s alt-line] LV4 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV4"
> > >     state_key: my_character_SPL4
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP4-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-9]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-10]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-11]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-12]` |  |  |  |  |  |
> > | `INPUT[toggle:SP4-13]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 5th Level
> > > [!recite|txt-s alt-line] LV5 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV5"
> > >     state_key: my_character_SPL5
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP5-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP5-9]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 6th Level
> > > [!recite|txt-s alt-line] LV6 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV6"
> > >     state_key: my_character_SPL6
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP6-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP6-9]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 7th Level
> > > [!recite|txt-s alt-line] LV7 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV7"
> > >     state_key: my_character_SPL7
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP7-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-7]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-8]` |  |  |  |  |  |
> > | `INPUT[toggle:SP7-9]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 8th Level
> > > [!recite|txt-s alt-line] LV8 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV8"
> > >     state_key: my_character_SPL8
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP8-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP8-7]` |  |  |  |  |  |
> 
> > [!recite|t-w txt-s nmg] 9th Level
> > > [!recite|txt-s alt-line] LV9 Spell Slots
> > > ```consumable
> > > items:
> > >   - label: "Spell Slots LV9"
> > >     state_key: my_character_SPL9
> > >     reset_on: long-rest
> > >     uses: 0
> > > ```
> > 
> > | Prep. | Spell | Casting Time | Range | Duration | Components |
> > | ----- | ----- |------------- | ------- | --------- | ------------- |
> > | `INPUT[toggle:SP9-1]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-2]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-3]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-4]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-5]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-6]` |  |  |  |  |  |
> > | `INPUT[toggle:SP9-7]` |  |  |  |  |  |


# Features & Traits
[[#Features & Traits|🔗]]  
 - **Tip!** You can *Insert Template* here and select *Feature Card Template* to quickly add a feature. Features with consumables need unique *state keys*.
> [!recite]- Search Action/Bonus Action/Reaction
> > [!recite|alt-line txt-s]- Actions
> > ```query
> > line:#action
> > title: A C T I O N S
> > ```
> 
> > [!recite|alt-line txt-s]- Bonus Actions
> > ```query
> > line:#bonus-action
> > title: B O N U S - A C T I O N S
> > ```
> 
> > [!recite|alt-line txt-s]- Reactions
> > ```query
> > line:#reaction
> > title: R E A C T I O N S
> > ```
> 

#### Senses & Vulnerabilities
**Senses:** 
**Resistances:** 
**Vulnerabilities:** 
**Immunities:** 

## Actions #action 


## Bonus Actions #bonus-action


## Other Features

> [!recite|nmg]+ Feature Example
> # Feature
> *Source: Lvl 10 Class Feature / PHB / Race / ETC*
> \--
> ```consumable
> items:
>   - label: "Charges"
>     state_key: my_character_feature
>     uses: 3
>     reset_on: long-rest
> ```
> Description of feature.
> 


# Backstory
[[#Backstory|🔗]]  

---

---
# Misc.
[[#Misc.|🔗]]  

---

---
# Notes
[[#Notes|🔗]]  

---
