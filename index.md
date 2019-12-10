<!-- title>Crystalis Randomizer</title>
<link rel="stylesheet" href="css/main.css">

<nav>
  <a class="img if-not-permalink" href="/"><img src="images/crystalis-sword.png"></a>
  <a href="index">Play</a>
  <a class="if-not-permalink" href="track">Track</a>
  <a href="help">Help</a>
  <!-- TODO: better process for stable version numbers. -->
  <span id="version"></span>
</nav>
<div></div -->

# Introduction

Welcome to Crystalis Randomizer.  This project seeks to
provide fresh gameplay experiences through the classic NES game
Crystalis, while remaining as faithful as possible to the
aspects of the original game that made it fun in the first place.

# Getting Started

 * **Start with a casual flagset**, even if you're super-familiar
   with the original game!  Many of the flags, especially the "hard-mode"
   flags, are simply not suited to beginning players, and will most likely
   lead to frustraton.
 * A good way to get started is to turn on some casual flags and to use
   a tracker (such as the one provided here, or else the emotracker pack).
   Clicking on "Track" in the top menu will automatically
   use the currently selected flag set to determine availability of each
   item on the mini map.  Availability is indicated by colors, from red
   (completely blocked) to orange and yellow (available via hard mode
   strat or glitch, respectively) to greenish yellow (available but not
   considered by the current flag's logic) to green (available and probably
   expected).  Locations may be marked as "checked" by clicking on them,
   or by right-clicking on the major item that's usually there.
 * Learn the [dungeon maps] to the main key item locations.
 * Do not shuffle minor items in with the major ones, and then do not
   worry about the minor item chests.
 * Expect to spend 2-4 hours the first time.  With some practice it's
   not too difficult to get down to the 1-2 hour range.
 * Grinding is not as time-consuming in the randomizer as in vanilla,
   but levels are a huge help to scale down the difficulty.  Pay attention
   to the EXP from different enemies and grind out a level or two if things
   get too difficult.
 * <span class="item">Medical herbs</span> (especially buffed) are often
   more valuable than <span class="item">magic rings</span>.
   <span class="item">Warp boots</span> are also very helpful, both for fast
   travel and for getting out of a pinch.  Always keep one or two in inventory.
   They can be stolen from <span class="location">Brynmaer</span>.
 * Learn to exploit the most important glitches:
     * Shop glitch: get an item for cheap (or free) by selecting a
       neighboring item (or blank space), then press the direction toward
       the item you want and very quickly afterwards (next frame or two)
       tap A to buy it for the previously-selected price.  Take advantage
       of this at the start of the game by walking through the new passage
       to <span class="location">Portoa</span> and stealing some better armor.
       [See video explanation][shop-glitch]
     * Statue glitch: pass a number of spots that are supposed to
       be blocked by statues or guards by approaching them from the right,
       then holding left and down while continually dismissing the dialog.
       You will be pushed up a little each time and eventually will pass
       them.  To do the reverse, hold down and right to be pushed left.
       [See video explanation][statue-glitch]
     * Stom fight glitch: warp to <span clas="location">Leaf</span>
       immediately after Stom takes the first stab to win the fight right
       away.  Don't warp anywhere else as it can softlock the game.
     * Sword charge glitch: higher level charges can be used temporarily
       without having the ball or bracelet if a different sword does have
       the higher level upgrade.  To do so, equip the sword and the higher
       upgrade and leave the inventory screen.  Then go back into inventory,
       equip the sword without the upgrade, and before leaving the menu,
       press "start" to save the game.  Soft-reset the console and load the
       game.  The higher charges (and higher damage) will be available until
       the inventory screen is entered.
       [See video explanation][sword-charge-glitch]
     * A few very specific skips are also possible:
       [Teleport skip] [Rabbit skip], [Ghetto flight]
     * Many of these glitches may be disabled completely.  If the shop
       glitch is disabled, then larger gold drops will be provided.
 * The early game is the hardest, when you don't have many sword options.
   Once it starts to open up a bit, things usually get quite a bit easier.

[dungeon maps]: http://mikesrpgcenter.com/crystalis/index.html#maps
[shop-glitch]: https://www.youtube.com/watch?v=j05u6x3irNg&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C&index=7
[statue-glitch]: https://www.youtube.com/watch?v=ROBcZpUwiJ8&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C&index=5
[sword-charge-glitch]: https://www.youtube.com/watch?v=6hXOutvuD1Q&index=2&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C
[Teleport skip]: https://www.youtube.com/watch?v=bsHdN4_5q4M&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C&index=1
[Rabbit skip]: https://www.youtube.com/watch?v=P2Ou1TI8yTk&index=4&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C
[Ghetto flight]: https://www.youtube.com/watch?v=P2Ou1TI8yTk&index=6&list=PLyA9BtOXggkiOGWAj-tjnqLang97E8G7C

# Gameplay Changes

A number of gameplay changes have been made to support randomization.

 * Items are shuffled throughout the game.  Items are split into five
   categories (key items (anything required for progression, like swords,
   orbs, bows, and fetch quest items), bonus items (unique items not
   required for progression, like the passive equipped items), consumables
   (non-unique items), magics, and traps (mimics).  Flags are provided to
   control exactly whether and how these categories are shuffled.
 * Adds a "difficulty level", which can be seen in the
   bottom-right corner next to the player's level.  Each key or
   bonus item that is picked up increases the difficulty level by 1, to a
   maximum of 47.
 * Enemies are shuffled throughout the game.
 * Enemy stats (attack, defense, HP, experience and gold
   rewards) are normalized based on the difficulty level.
 * A passage is (optionally) opened between <span class="location">Valley
   of Wind</span> and <span class="location">Lime Tree</span>.
 * A number of triggers have been slightly changed (see below).
 * A number of characters spawn in multiple locations independent of
   game events (e.g. <span class="npc">Zebu</span> remains in <span class="location">Zebu's
   Cave</span> the entire game, rather than "moving" to <span class="location">Shyron</span>
   after calming the sea).
 * Some minor bug fixes: screen shaking is fixed, and <span class="boss">Vampire 2</span>
   no longer speeds up near the start of the fight.
 * <span class="location">Swan gate</span> now has a pair of guards on the opposite side,
   to allow going through either direction (with <span class="magic">Change</span>).
   The guards will only despawn after the gate is open.
 * It is now possible to teleport out of the tower, and to get
   back in via the <span class="location">crypt</span>.
 * <span class="item">Sword of Thunder</span> always teleports to
   <span class="location">Shyron</span>, no matter where it's found
   (though this can be disabled).  The warp checkpoint is immediately set,
   and in case there's no way back, <span class="npc">Asina</span> will
   teleport the player back to <span class="location">Mezame Shrine</span>.
 * When continuing, a minimum amount of "pity" HP and MP are given.
   Normally this is 5 HP and 1 MP (to prevent immediate death from
   terrain and ensure <span class="magic">Flight</span> is possible), but
   when swordless it is 20 MP (to ensure <span class="magic">Change</span>
   or <span class="magic">Teleport</span> is possible as well).
 * The "quest item" inventory row (3rd row of second page) has eight extra
   invisible slots to accommodate situations where quest items build up
   without being consumed.  To access the additional items, "drop" one of the
   visible items and it will cycle a new item into its place (the item is not
   lost: it can be recovered by repeating this process enough times).

# Maps 
 * A passage may optionally (via the <span class="flag">Rp</span> flag)
   be opened between the Valley of Wind (outside Leaf) and Waterfall Valley
   (outside Portoa).
 * The back entrance to the windmill cave is closed until the
   <span class="item">Windmill Key</span> has been used in the windmill.
 * The back entrance to the summit cave (next to Portoa) is now closed
   until the <span class="item">Key to Prison</span> has been used.  The
   key can be used on either side of the cave.
 * A small piece of land has been added to connect the entrance to the
   underground channel with the beach that the hurt dolphin spawns on.
   This prevents some possible softlocks.
 * A number of cave entrances in the game are closed until the player
   exits Mezame shrine.  This should be unobservable unless the player
   wild warps out of the starting screen, rather than exiting to the south.

# Items
 * Inventory sorting is disabled for swords and orbs/bracelets to prevent
   items from clobbering each other.
 * Key items can overflow into an invisible buffer; if you have items in
   this buffer, you can "drop" a key item to recover the overflowed items.
   The "dropped" item will take its place in the buffer.
 * <span class="item">Alarm Flute</span> is now a key item, given by
   Zebu's student (along with the starting cash) in Leaf.
 * <span class="item">Alarm Flute</span> and <span class="item">Flute of
   Lime</span> are now multi-use items. Each will disappear after the
   second successful use.
 * The second <span class="item">Flute of Lime</span> chest now contains
   a <span class="item">Mirrored Shield</span> and is counted as a bonus
   item for shuffling purposes.
 * Orbs and bracelets are progressive upgrades: the first item will be
   the orb, and the second will be the bracelet, regardless of the order
   the chests are opened in.
 * Orbs and bracelets may now (optionally) be automatically equipped.
   Just change swords and the powerup will change, too.
 * Sword damage has been renormalized.  Rather than depending on the
   element (normally, wind=1, fire=2, water=4, thunder=8), the sword power
   depends on the number of upgrades (no upgrades=2, ball only=4, bracelet=8).
 * Stab damage no longer doubles the sword base power, but is
   now always just 2, on top of the base power of the sword.
 * The <span class="item">Power Ring</span> is nerfed to double the
   sword base damage, rather than the level.
 * <span class="item">Pendant of Deo</span> is buffed to provide MP while
   moving (under <span class="flag">Td</span>).
 * <span class="item">Iron Necklace</span> and <span class="item">Shield
   Ring</span> are buffed to double the armor/shield value, rather than the
   level.
 * <span class="item">Rabbit Boots</span> now also allows charging swords
   to level 2 while moving (under <span class="flag">Tr</span>).
 * <span class="item">Leather Boots</span> are (optionally) replaced with
   <span class="item">Speed Boots</span>.
 * <span class="item">Medical Herb</span> and <span class="item">Fruit of
   Power</span> can be optionally buffed to three different levels: in
   hard mode (<span class="flag">Hm</span>) there is no buff (32 HP, 32 MP),
   in default mode (no flag) they are buffed to 64 HP and 48 MP.  In easy
   mode (<span class="flag">Em</span>) they are buffed to 96 HP and 64 MP.
 * Mimics will only ever shuffle into visible chests (this does not include
   boss drops).
 * Consumables and armor/shields can only shuffle into chests, so that
   a full inventory does not cause the item to disappear.
 * <span class="item">Opel Statue</span> now works automatically and
   cannot be selected.  It also correctly clears status effects.
 * <span class="item">Psycho Shield</span> and <span class="item">Psycho
   Armor</span> are nerfed to only provide 20 DEF each.
   <span class="item">Battle Shield</span> and <span class="item">Ceramic
   Armor</span> are now the armors with highest (32) DEF.
 * <span class="item">Sacred Shield</span> now prevents curse instead of
   paralysis.  <span class="item">Ceramic Shield</span> blocks paralysis.
 * <span class="item">Platinum Shield</span> and <span class="item">Mirrored
   Shield</span> each have 2 DEF extra.
 * Powerful armors will only provide up to a maximum of LVL*3 defense.
 * Shops are now randomized (under <span class="flag">Ps</span>).
   The prices of tools and inns increases over time (doubling every 10
   scaling levels), while the prices of armors decreases over time (halving
   every 12 scaling levels).
 * Flute of Lime can be used twice for both the "guards" as well as Akahana.
 * Alarm Flute can no longer be found in shops but is instead shuffled in as 
   a multi-use key item for windmill guard and Kensu.

# Triggers

In the following, items in brackets refer to whatever item
is shuffled into a slot, while unparenthesized items refer to the
actual item.

 * Zebu, Tornel, Stom, Akahana, Asina, and Kensu are always available
   in the different locations as long as they need to be, regardless of
   any other story events that occur.
 * Zebu will spawn the sleeping Windmill Guard even after starting the
   windmill.
 * The Leaf abduction will not happen unless the player has talked to
   Zebu and Kelbesque has not yet been defeated.
 * Defeating Kelbesque is an alternative condition (rather than talking
   to the rabbit) to get into Mt Sabre North.
 * [Paralysis] and freeing the villagers now both require having defeated
   Kelbesque, rather than just stepping into the cave.  It can be learned
   at either entrance.
 * [Barrier] now requires calming the sea, rather than just ghetto flight.
 * The Queen of Portoa will not "go on vacation" and reveal herself as
   Asina until after the Mesia recording has been viewed (this ensures
   both Sword and Orb of Water are acquired, guaranteeing that the back
   room is reachable).
 * If Queen of Portoa doesn't give [Flute of Lime] before turning into
   Asina, just talk to her again after getting [Recover].
 * Fog Lamp cannot be returned unless Shell Flute is
   acquired. Optionally (with the 'Rd' flag), it's also required
   to have healed the dolphin (note that this means that without
   the flag it's possible to heal the dolphin while riding the
   dolphin.  Don't worry, it's his sister).
 * Kensu will not appear in the beach cabin until Fog Lamp has been
   returned.
 * The Shyron massacre requires both the actual Sword of Thunder and
   getting the [Key to Stxy] from Zebu in Shyron.

# Bug Reports

Please report bugs either on [GitHub] or on the Discord.  An effective bug report includes the following:

 * All relevant information about the seed: the software
   version that generated it, the flag set, the seed, and the
   checksum.  These can all be seen in the "codename entry"
   computer upon starting a new game, but the easiest way to
   get it is The easiest way to get this is to <a href="check">
   extract it directly from the image</a>.
 * As much detail as possible to reproduce the bug.  A link
   to a twitch clip of the bug manifesting is ideal, together
   with explanation of any preceding events that seem relevant.
   At the very least, answer the following questions: (1) what
   were you doing, (2) what did you expect to happen, and (3)
   what happened instead?

[GitHub]: https://github.com/shicks/crystalis-randomizer/issues
