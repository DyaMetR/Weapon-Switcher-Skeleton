# Weapon Switcher Skeleton
A weapon switcher skeleton script for Garry's Mod. Lacks specific implementation, as it's left for each developer to decide.

## How to use

### Implementation

In order to make the selector work, you only have to use _3 functions_.

`moveCursor(forward)`

Moves the cursor one position, either forward or backwards.

+ **forward**: Whether the cursor should move forward or backwards.

`cycleSlot(slot)`

Moves the cursor forward one position inside a slot.

+ **slot**: The slot to move the cursor inside.

`equipSelectedWeapon()`

Equips the weapon currently selected by the switcher.

### When it's recommended to draw the weapon selector

When the weapon switcher selects a weapon, it'll set it's `curSlot` to 0. You can use the condition `curSlot > 0` to determine whether the weapon selector should be drawn (or not).

### Configuration

You can edit the function `skipEmpty(weapon)` to return whether the weapon switcher should skip weapons with no ammo available.
