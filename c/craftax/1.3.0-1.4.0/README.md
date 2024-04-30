# Comparing `tmp/craftax-1.3.0.tar.gz` & `tmp/craftax-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craftax-1.3.0.tar", last modified: Sun Apr  7 21:37:45 2024, max compression
+gzip compressed data, was "craftax-1.4.0.tar", last modified: Tue Apr 30 12:58:28 2024, max compression
```

## Comparing `craftax-1.3.0.tar` & `craftax-1.4.0.tar`

### file list

```diff
@@ -1,262 +1,264 @@
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1059 2024-03-06 09:23:28.000000 craftax-1.3.0/LICENSE
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       73 2024-03-27 11:54:45.000000 craftax-1.3.0/MANIFEST.in
--rw-r--r--   0 mans4835  (1001) mans4835  (1001)     8674 2024-04-07 21:37:45.926173 craftax-1.3.0/PKG-INFO
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7789 2024-04-07 21:36:12.000000 craftax-1.3.0/README.md
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.898172 craftax-1.3.0/craftax/
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.898172 craftax-1.3.0/craftax/craftax/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/__init__.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/assets/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      607 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/0.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1827 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/1.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1501 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1559 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/3.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1533 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/4.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1518 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/5.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1567 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/6.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1538 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/7.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1506 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/8.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1535 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/9.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1825 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-down.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1731 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-left.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1752 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-right.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1833 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow-up.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      603 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      602 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/arrow_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      652 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/bat.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      719 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/book.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      654 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/boots_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      652 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/boots_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      693 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/bow.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      953 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chest.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chestplate_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/chestplate_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      866 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/coal.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1983 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/cow.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      621 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/dagger.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5735 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug-2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5762 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug-3.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5761 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       84 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/debug_tile.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      996 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/deep_thing.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      790 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/dexterity.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      605 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_boots.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      685 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_chestplate.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      642 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_helmet.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      609 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_pants.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      733 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      714 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/diamond_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2492 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/drink.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1087 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/enchantment_table_fire.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1092 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/enchantment_table_ice.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2213 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/energy.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2449 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fence.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      674 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_elemental.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      710 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      959 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_stone.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1140 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fire_tree.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fireball.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2292 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/food.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1141 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/fountain.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      723 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/frost_troll.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      910 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/furnace.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      860 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gnome_archer.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      847 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gnome_warrior.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      691 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1099 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1210 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1161 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/grave3.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      741 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/gravel.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2721 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/health.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      666 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/helmet_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      666 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/helmet_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      689 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_elemental.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      719 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      994 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ice_shrub.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      668 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iceball.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      933 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/intelligence.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1048 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      613 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_boots.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      681 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_chestplate.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      642 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_helmet.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      608 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_pants.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2354 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2390 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/iron_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/knight.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      889 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/knight_archer.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      737 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/kobold.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_down.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      855 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_down_blocked.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      612 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ladder_up.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2130 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/lava.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      755 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/leaves.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      758 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/lizard.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      745 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/log.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      695 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/mana.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1150 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/necromancer.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1128 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/necromancer_vulnerable.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      769 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/orc_mage.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      777 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/orc_soldier.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      709 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pants_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      702 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pants_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7488 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/path.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      325 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/path_moss.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      809 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/pigman.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2154 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant-ripe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2511 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant-young.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2080 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/plant_on_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6186 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-down.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6195 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-left.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6212 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-right.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6590 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-sleep.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6144 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player-up.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/player.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      715 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_blue.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      723 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_cyan.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      705 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_green.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      715 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_pink.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      708 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_red.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      707 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/potion_yellow.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      245 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1110 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/ruby.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sand.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1817 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sapling.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      957 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sapphire.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5993 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/skeleton.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      673 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/slimeball.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/snail.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      668 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/spider.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stalagmite.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7242 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2345 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2429 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/stone_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      670 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/strength.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      613 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sword_fire_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      620 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/sword_ice_enchantment.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      885 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/table.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)  1769538 2024-03-27 11:45:23.000000 craftax-1.3.0/craftax/craftax/assets/texture_cache.pbz2
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      615 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/torch_in_inventory.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1197 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/torch_on_path.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7782 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/tree.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      698 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/troll.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2127 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/unknown.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      126 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      163 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wall_moss.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/water.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1577 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2045 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2453 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/wood_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      718 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/xp.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2089 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/assets/zombie.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    34412 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/constants.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2909 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/craftax_state.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/envs/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/envs/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      484 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/common.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3079 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/craftax_pixels_env.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3720 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)   106092 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/game_logic.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6938 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/play_craftax.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    41178 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/renderer.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/util/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    11631 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/util/game_logic_utils.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/maths_utils.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2382 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/util/noise.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.914173 craftax-1.3.0/craftax/craftax/world_gen/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax/world_gen/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    24490 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/world_gen/world_gen.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     9213 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax/world_gen/world_gen_configs.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.918172 craftax-1.3.0/craftax/craftax_classic/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/__init__.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.922172 craftax-1.3.0/craftax/craftax_classic/assets/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1827 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/1.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1501 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1559 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/3.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1533 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/4.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1518 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/5.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1567 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/6.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1538 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/7.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1506 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/8.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1535 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/9.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1825 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-down.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1731 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-left.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1752 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-right.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1833 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/arrow-up.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      866 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/coal.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1983 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/cow.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5735 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug-2.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5762 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug-3.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5761 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       84 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/debug_tile.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      839 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/diamond.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2492 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/drink.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2213 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/energy.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2449 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/fence.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2292 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/food.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      910 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/furnace.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      691 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2721 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/health.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1048 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2354 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2390 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/iron_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2130 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/lava.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      755 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/leaves.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      745 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/log.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7488 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/path.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2154 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant-ripe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2511 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant-young.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2080 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      219 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/plant_on_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6186 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-down.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6195 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-left.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6212 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-right.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6590 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-sleep.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     6144 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player-up.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      813 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/player.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      245 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      729 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/sand.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1817 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/sapling.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     5993 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/skeleton.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7242 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2345 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2429 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/stone_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      885 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/table.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7782 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/tree.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2127 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/unknown.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2198 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/water.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1577 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2045 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood_pickaxe.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2453 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/wood_sword.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2089 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/assets/zombie.png
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    13946 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/constants.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/craftax_classic/envs/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      505 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/common.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3171 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_pixels_env.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2053 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_state.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3819 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    58163 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/game_logic.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     4387 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/play_craftax_classic.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    24401 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/renderer.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/craftax_classic/util/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/util/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     2382 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/craftax_classic/util/noise.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)    10956 2024-04-07 21:31:09.000000 craftax-1.3.0/craftax/craftax_classic/world_gen.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax/environment_base/
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        0 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/__init__.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     3107 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/environment_no_auto_reset.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      290 2024-03-27 11:54:45.000000 craftax-1.3.0/craftax/environment_base/util.py
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     7389 2024-03-27 14:01:47.000000 craftax-1.3.0/craftax/environment_base/wrappers.py
-drwxrwxr-x   0 mans4835  (1001) mans4835  (1001)        0 2024-04-07 21:37:45.926173 craftax-1.3.0/craftax.egg-info/
--rw-r--r--   0 mans4835  (1001) mans4835  (1001)     8674 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/PKG-INFO
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     9455 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/SOURCES.txt
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        1 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/dependency_links.txt
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      147 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/entry_points.txt
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)      116 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/requires.txt
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)        8 2024-04-07 21:37:45.000000 craftax-1.3.0/craftax.egg-info/top_level.txt
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)     1058 2024-04-07 21:36:12.000000 craftax-1.3.0/pyproject.toml
--rw-rw-r--   0 mans4835  (1001) mans4835  (1001)       38 2024-04-07 21:37:45.926173 craftax-1.3.0/setup.cfg
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1059 2024-04-03 13:05:48.000000 craftax-1.4.0/LICENSE
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       73 2024-03-26 16:11:15.000000 craftax-1.4.0/MANIFEST.in
+-rw-r--r--   0 mikey     (1000) mikey     (1000)     9080 2024-04-30 12:58:28.211010 craftax-1.4.0/PKG-INFO
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     8195 2024-04-30 12:57:32.000000 craftax-1.4.0/README.md
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.195010 craftax-1.4.0/craftax/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.195010 craftax-1.4.0/craftax/craftax/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.203009 craftax-1.4.0/craftax/craftax/assets/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      607 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/0.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/1.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/4.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/5.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/6.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/7.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/8.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/9.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      603 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      602 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/arrow_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/bat.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/book.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      654 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/boots_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/boots_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      693 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/bow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      953 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/chest.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/chestplate_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/chestplate_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/coal.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/cow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      621 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/dagger.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/debug-2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/debug-3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/debug.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/debug_tile.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      996 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/deep_thing.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      790 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/dexterity.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      605 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_boots.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      685 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_chestplate.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_helmet.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      609 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_pants.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      733 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      714 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/diamond_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/drink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1087 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/enchantment_table_fire.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1092 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/enchantment_table_ice.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/energy.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      674 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fire_elemental.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      710 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fire_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      959 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fire_stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1140 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fire_tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fireball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/food.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1141 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/fountain.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/frost_troll.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/furnace.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      860 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/gnome_archer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      847 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/gnome_warrior.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1099 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/grave.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1210 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/grave2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1161 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/grave3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      741 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/gravel.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/health.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/helmet_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/helmet_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      689 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ice_elemental.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ice_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      994 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ice_shrub.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iceball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      933 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/intelligence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_boots.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      681 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_chestplate.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_helmet.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      608 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_pants.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/iron_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/knight.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      889 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/knight_archer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      737 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/kobold.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ladder_down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      855 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ladder_down_blocked.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      612 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ladder_up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/lava.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/leaves.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      758 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/lizard.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/log.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      695 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/mana.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1150 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/necromancer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1128 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/necromancer_vulnerable.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      769 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/orc_mage.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      777 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/orc_soldier.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      709 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/pants_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      702 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/pants_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      325 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/path_moss.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      809 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/pigman.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/plant-ripe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/plant-young.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/plant.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player-sleep.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/player.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_blue.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_cyan.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      705 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_green.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_pink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      708 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_red.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      707 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/potion_yellow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1110 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/ruby.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/sand.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/sapling.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      957 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/sapphire.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/skeleton.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      673 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/slimeball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/snail.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/spider.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1219 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/stalagmite.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/stone_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/stone_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/strength.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/sword_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      620 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/sword_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/table.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)  1769538 2024-03-26 15:46:49.000000 craftax-1.4.0/craftax/craftax/assets/texture_cache.pbz2
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      615 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/torch_in_inventory.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1197 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/torch_on_path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      698 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/troll.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/unknown.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      126 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wall.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      163 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wall2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      198 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wall_moss.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/water.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wood.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wood_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/wood_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      718 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/xp.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/assets/zombie.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    34413 2024-04-15 14:38:21.000000 craftax-1.4.0/craftax/craftax/constants.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2741 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax/craftax_state.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.203009 craftax-1.4.0/craftax/craftax/envs/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/envs/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     4853 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5388 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)   106352 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax/game_logic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7029 2024-04-15 14:38:17.000000 craftax-1.4.0/craftax/craftax/play_craftax.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    41178 2024-03-28 18:50:50.000000 craftax-1.4.0/craftax/craftax/renderer.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.203009 craftax-1.4.0/craftax/craftax/util/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/util/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    11631 2024-03-28 18:50:50.000000 craftax-1.4.0/craftax/craftax/util/game_logic_utils.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      594 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax/util/maths_utils.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2534 2024-04-30 10:50:13.000000 craftax-1.4.0/craftax/craftax/util/noise.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.203009 craftax-1.4.0/craftax/craftax/world_gen/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax/world_gen/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    24840 2024-04-30 10:50:13.000000 craftax-1.4.0/craftax/craftax/world_gen/world_gen.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     9213 2024-03-28 18:50:50.000000 craftax-1.4.0/craftax/craftax/world_gen/world_gen_configs.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.203009 craftax-1.4.0/craftax/craftax_classic/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/craftax/craftax_classic/assets/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/1.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/4.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/5.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/6.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/7.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/8.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/9.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/arrow-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/arrow-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/arrow-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/arrow-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/coal.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/cow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/debug-2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/debug-3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/debug.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/debug_tile.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/diamond.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/drink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/energy.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/fence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/food.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/furnace.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/health.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/iron.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/iron_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/iron_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/lava.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/leaves.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/log.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/plant-ripe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/plant-young.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/plant.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player-sleep.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/player.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/sand.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/sapling.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/skeleton.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/stone_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/stone_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/table.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)  1262198 2024-03-26 15:51:57.000000 craftax-1.4.0/craftax/craftax_classic/assets/texture_cache_classic.pbz2
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/unknown.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/water.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/wood.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/wood_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/wood_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/assets/zombie.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    13946 2024-03-28 18:50:50.000000 craftax-1.4.0/craftax/craftax_classic/constants.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/craftax/craftax_classic/envs/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/envs/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      505 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/envs/common.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     4973 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax_classic/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2086 2024-04-30 10:50:13.000000 craftax-1.4.0/craftax/craftax_classic/envs/craftax_state.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5443 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax_classic/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    58460 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax_classic/game_logic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     4984 2024-04-08 10:22:04.000000 craftax-1.4.0/craftax/craftax_classic/play_craftax_classic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    24401 2024-03-28 18:50:50.000000 craftax-1.4.0/craftax/craftax_classic/renderer.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/craftax/craftax_classic/util/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/craftax_classic/util/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2535 2024-04-30 10:50:13.000000 craftax-1.4.0/craftax/craftax_classic/util/noise.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    11690 2024-04-30 10:50:13.000000 craftax-1.4.0/craftax/craftax_classic/world_gen.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2441 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/craftax_env.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/craftax/environment_base/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/environment_base/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2622 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/environment_base/environment_bases.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      290 2024-03-26 16:11:15.000000 craftax-1.4.0/craftax/environment_base/util.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6749 2024-04-30 12:51:00.000000 craftax-1.4.0/craftax/environment_base/wrappers.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 12:58:28.211010 craftax-1.4.0/craftax.egg-info/
+-rw-r--r--   0 mikey     (1000) mikey     (1000)     9080 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/PKG-INFO
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     9517 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        1 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      154 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/entry_points.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      116 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/requires.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        8 2024-04-30 12:58:28.000000 craftax-1.4.0/craftax.egg-info/top_level.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1065 2024-04-30 12:51:47.000000 craftax-1.4.0/pyproject.toml
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       38 2024-04-30 12:58:28.211010 craftax-1.4.0/setup.cfg
```

### Comparing `craftax-1.3.0/LICENSE` & `craftax-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/PKG-INFO` & `craftax-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craftax
-Version: 1.3.0
+Version: 1.4.0
 Summary: An open-world environment for training RL agents
 Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
 Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
 Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -67,15 +67,15 @@
 Craftax conforms to the gymnax interface:
 ```python
 rng = jax.random.PRNGKey(0)
 rng, _rng = jax.random.split(rng)
 rngs = jax.random.split(_rng, 3)
 
 # Create environment
-env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
+env = make_craftax_env_from_name("Craftax-Symbolic-v1", auto_reset=True)
 env_params = env.default_params
 
 # Get an initial state and observation
 obs, state = env.reset(rngs[0], env_params)
 
 # Pick random action
 action = env.action_space(env_params).sample(rngs[1])
@@ -121,19 +121,22 @@
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
 To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
-Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
-This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
+Craftax provides the option to use optimistic resets to improve performance, which means that we provide access to environments that **do not auto-reset**.
+Environments obtained from `make_craftax_env_from_name` or `make_craftax_env_from_args` with `auto_reset=False` will not automatically reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in `OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).
+See `ppo.py` in [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct usage.
+Using `auto_reset=True` will return a regular auto-reset environment, which can be treated like any other gymnax environment.
 
 ### Texture Caching
-We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch.
+We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch every run.
 ```
 export CRAFTAX_RELOAD_TEXTURES=true
 ```
 
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.3.0 Summary: An open-world
+Metadata-Version: 2.1 Name: craftax Version: 1.4.0 Summary: An open-world
 environment for training RL agents Author-email: Michael Matthews
 eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
 Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
@@ -10,15 +10,15 @@
 pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
 checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
 Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -28,23 +28,23 @@
 Craftax/main/images/dungeon_crawling.gif]
 [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
 farming.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/
 images/magic.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/
 main/images/mining.gif]
 # ð Basic Usage Craftax conforms to the gymnax interface: ```python rng =
 jax.random.PRNGKey(0) rng, _rng = jax.random.split(rng) rngs = jax.random.split
-(_rng, 3) # Create environment env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
-env_params = env.default_params # Get an initial state and observation obs,
-state = env.reset(rngs[0], env_params) # Pick random action action =
-env.action_space(env_params).sample(rngs[1]) # Step environment obs, state,
-reward, done, info = env.step(rngs[2], state, action, env_params) ``` # â¬ï¸
-Installation The latest Craftax release can be installed from PyPi: ``` pip
-install craftax ``` If you want the most recent commit instead use: ``` pip
-install git+https://github.com/MichaelTMatthews/Craftax.git@main ``` ##
-Extending Craftax If you want to extend Craftax, run (make sure you have
+(_rng, 3) # Create environment env = make_craftax_env_from_name("Craftax-
+Symbolic-v1", auto_reset=True) env_params = env.default_params # Get an initial
+state and observation obs, state = env.reset(rngs[0], env_params) # Pick random
+action action = env.action_space(env_params).sample(rngs[1]) # Step environment
+obs, state, reward, done, info = env.step(rngs[2], state, action, env_params)
+``` # â¬ï¸ Installation The latest Craftax release can be installed from
+PyPi: ``` pip install craftax ``` If you want the most recent commit instead
+use: ``` pip install git+https://github.com/MichaelTMatthews/Craftax.git@main
+``` ## Extending Craftax If you want to extend Craftax, run (make sure you have
 `pip>=23.0`): ``` git clone https://github.com/MichaelTMatthews/Craftax.git cd
 Craftax pip install --editable . ``` ## GPU-Enabled JAX By default, both of the
 above methods will install JAX on the CPU. If you want to run JAX on a GPU/TPU,
 you'll need to install the correct wheel for your system from _J_A_X. For NVIDIA
 GPU the command is: ``` pip install -U "jax[cuda12_pip]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
@@ -52,27 +52,32 @@
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
 Experiment To run experiments see the [Craftax Baselines](https://github.com/
 MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
 Resets Craftax provides the option to use optimistic resets to improve
-performance, which means that (unlike regular gymnax environments) it **does
-not auto-reset** by default. This means that the environment should always be
-wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
-`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
-`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
-texture cache to avoid recreating the texture atlas every time Craftax is
+performance, which means that we provide access to environments that **do not
+auto-reset**. Environments obtained from `make_craftax_env_from_name` or
+`make_craftax_env_from_args` with `auto_reset=False` will not automatically
+reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in
+`OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper`
+(to recover the default gymnax auto-reset behaviour). See `ppo.py` in [Craftax
+Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct
+usage. Using `auto_reset=True` will return a regular auto-reset environment,
+which can be treated like any other gymnax environment. ### Texture Caching We
+use a texture cache to avoid recreating the texture atlas every time Craftax is
 imported. If you are just running Craftax as a benchmark this will not affect
 you. However, if you are editing the game (e.g. adding new blocks, entities
 etc.) then a stale cache could cause errors. You can export the following
-environment variable to force textures to be created from scratch. ``` export
-CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
-algorithm please open a PR and provide a reference to the source of the
-results. We report reward as a % of the maximum (226). ## Craftax-1B |
+environment variable to force textures to be created from scratch every run.
+``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
+to add an algorithm please open a PR and provide a reference to the source of
+the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
 | _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
```

### Comparing `craftax-1.3.0/README.md` & `craftax-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -38,15 +38,15 @@
 Craftax conforms to the gymnax interface:
 ```python
 rng = jax.random.PRNGKey(0)
 rng, _rng = jax.random.split(rng)
 rngs = jax.random.split(_rng, 3)
 
 # Create environment
-env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
+env = make_craftax_env_from_name("Craftax-Symbolic-v1", auto_reset=True)
 env_params = env.default_params
 
 # Get an initial state and observation
 obs, state = env.reset(rngs[0], env_params)
 
 # Pick random action
 action = env.action_space(env_params).sample(rngs[1])
@@ -92,19 +92,22 @@
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
 To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
-Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
-This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
+Craftax provides the option to use optimistic resets to improve performance, which means that we provide access to environments that **do not auto-reset**.
+Environments obtained from `make_craftax_env_from_name` or `make_craftax_env_from_args` with `auto_reset=False` will not automatically reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in `OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).
+See `ppo.py` in [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct usage.
+Using `auto_reset=True` will return a regular auto-reset environment, which can be treated like any other gymnax environment.
 
 ### Texture Caching
-We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch.
+We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch every run.
 ```
 export CRAFTAX_RELOAD_TEXTURES=true
 ```
 
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -16,23 +16,23 @@
 Craftax/main/images/dungeon_crawling.gif]
 [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
 farming.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/
 images/magic.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/
 main/images/mining.gif]
 # ð Basic Usage Craftax conforms to the gymnax interface: ```python rng =
 jax.random.PRNGKey(0) rng, _rng = jax.random.split(rng) rngs = jax.random.split
-(_rng, 3) # Create environment env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
-env_params = env.default_params # Get an initial state and observation obs,
-state = env.reset(rngs[0], env_params) # Pick random action action =
-env.action_space(env_params).sample(rngs[1]) # Step environment obs, state,
-reward, done, info = env.step(rngs[2], state, action, env_params) ``` # â¬ï¸
-Installation The latest Craftax release can be installed from PyPi: ``` pip
-install craftax ``` If you want the most recent commit instead use: ``` pip
-install git+https://github.com/MichaelTMatthews/Craftax.git@main ``` ##
-Extending Craftax If you want to extend Craftax, run (make sure you have
+(_rng, 3) # Create environment env = make_craftax_env_from_name("Craftax-
+Symbolic-v1", auto_reset=True) env_params = env.default_params # Get an initial
+state and observation obs, state = env.reset(rngs[0], env_params) # Pick random
+action action = env.action_space(env_params).sample(rngs[1]) # Step environment
+obs, state, reward, done, info = env.step(rngs[2], state, action, env_params)
+``` # â¬ï¸ Installation The latest Craftax release can be installed from
+PyPi: ``` pip install craftax ``` If you want the most recent commit instead
+use: ``` pip install git+https://github.com/MichaelTMatthews/Craftax.git@main
+``` ## Extending Craftax If you want to extend Craftax, run (make sure you have
 `pip>=23.0`): ``` git clone https://github.com/MichaelTMatthews/Craftax.git cd
 Craftax pip install --editable . ``` ## GPU-Enabled JAX By default, both of the
 above methods will install JAX on the CPU. If you want to run JAX on a GPU/TPU,
 you'll need to install the correct wheel for your system from _J_A_X. For NVIDIA
 GPU the command is: ``` pip install -U "jax[cuda12_pip]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
@@ -40,27 +40,32 @@
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
 Experiment To run experiments see the [Craftax Baselines](https://github.com/
 MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
 Resets Craftax provides the option to use optimistic resets to improve
-performance, which means that (unlike regular gymnax environments) it **does
-not auto-reset** by default. This means that the environment should always be
-wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
-`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
-`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
-texture cache to avoid recreating the texture atlas every time Craftax is
+performance, which means that we provide access to environments that **do not
+auto-reset**. Environments obtained from `make_craftax_env_from_name` or
+`make_craftax_env_from_args` with `auto_reset=False` will not automatically
+reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in
+`OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper`
+(to recover the default gymnax auto-reset behaviour). See `ppo.py` in [Craftax
+Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct
+usage. Using `auto_reset=True` will return a regular auto-reset environment,
+which can be treated like any other gymnax environment. ### Texture Caching We
+use a texture cache to avoid recreating the texture atlas every time Craftax is
 imported. If you are just running Craftax as a benchmark this will not affect
 you. However, if you are editing the game (e.g. adding new blocks, entities
 etc.) then a stale cache could cause errors. You can export the following
-environment variable to force textures to be created from scratch. ``` export
-CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
-algorithm please open a PR and provide a reference to the source of the
-results. We report reward as a % of the maximum (226). ## Craftax-1B |
+environment variable to force textures to be created from scratch every run.
+``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
+to add an algorithm please open a PR and provide a reference to the source of
+the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
 | _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
```

### Comparing `craftax-1.3.0/craftax/craftax/assets/0.png` & `craftax-1.4.0/craftax/craftax/assets/0.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/1.png` & `craftax-1.4.0/craftax/craftax/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/2.png` & `craftax-1.4.0/craftax/craftax/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/3.png` & `craftax-1.4.0/craftax/craftax/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/4.png` & `craftax-1.4.0/craftax/craftax/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/5.png` & `craftax-1.4.0/craftax/craftax/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/6.png` & `craftax-1.4.0/craftax/craftax/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/7.png` & `craftax-1.4.0/craftax/craftax/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/8.png` & `craftax-1.4.0/craftax/craftax/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/9.png` & `craftax-1.4.0/craftax/craftax/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow-down.png` & `craftax-1.4.0/craftax/craftax/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow-left.png` & `craftax-1.4.0/craftax/craftax/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow-right.png` & `craftax-1.4.0/craftax/craftax/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow-up.png` & `craftax-1.4.0/craftax/craftax/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/arrow_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/arrow_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/arrow_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/bat.png` & `craftax-1.4.0/craftax/craftax/assets/bat.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/book.png` & `craftax-1.4.0/craftax/craftax/assets/book.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/boots_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/boots_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/boots_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/boots_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/bow.png` & `craftax-1.4.0/craftax/craftax/assets/bow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/chest.png` & `craftax-1.4.0/craftax/craftax/assets/chest.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/chestplate_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/chestplate_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/chestplate_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/chestplate_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/coal.png` & `craftax-1.4.0/craftax/craftax/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/cow.png` & `craftax-1.4.0/craftax/craftax/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/dagger.png` & `craftax-1.4.0/craftax/craftax/assets/dagger.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/debug-2.png` & `craftax-1.4.0/craftax/craftax/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/debug-3.png` & `craftax-1.4.0/craftax/craftax/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/debug.png` & `craftax-1.4.0/craftax/craftax/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/deep_thing.png` & `craftax-1.4.0/craftax/craftax/assets/deep_thing.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/dexterity.png` & `craftax-1.4.0/craftax/craftax/assets/dexterity.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond.png` & `craftax-1.4.0/craftax/craftax/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_boots.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_chestplate.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_helmet.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_pants.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_pickaxe.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/diamond_sword.png` & `craftax-1.4.0/craftax/craftax/assets/diamond_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/drink.png` & `craftax-1.4.0/craftax/craftax/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/enchantment_table_fire.png` & `craftax-1.4.0/craftax/craftax/assets/enchantment_table_fire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/enchantment_table_ice.png` & `craftax-1.4.0/craftax/craftax/assets/enchantment_table_ice.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/energy.png` & `craftax-1.4.0/craftax/craftax/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fence.png` & `craftax-1.4.0/craftax/craftax/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fire_elemental.png` & `craftax-1.4.0/craftax/craftax/assets/fire_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fire_grass.png` & `craftax-1.4.0/craftax/craftax/assets/fire_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fire_stone.png` & `craftax-1.4.0/craftax/craftax/assets/fire_stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fire_tree.png` & `craftax-1.4.0/craftax/craftax/assets/fire_tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fireball.png` & `craftax-1.4.0/craftax/craftax/assets/fireball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/food.png` & `craftax-1.4.0/craftax/craftax/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/fountain.png` & `craftax-1.4.0/craftax/craftax/assets/fountain.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/frost_troll.png` & `craftax-1.4.0/craftax/craftax/assets/frost_troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/furnace.png` & `craftax-1.4.0/craftax/craftax/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/gnome_archer.png` & `craftax-1.4.0/craftax/craftax/assets/gnome_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/gnome_warrior.png` & `craftax-1.4.0/craftax/craftax/assets/gnome_warrior.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/grass.png` & `craftax-1.4.0/craftax/craftax/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/grave.png` & `craftax-1.4.0/craftax/craftax/assets/grave.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/grave2.png` & `craftax-1.4.0/craftax/craftax/assets/grave2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/grave3.png` & `craftax-1.4.0/craftax/craftax/assets/grave3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/gravel.png` & `craftax-1.4.0/craftax/craftax/assets/gravel.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/health.png` & `craftax-1.4.0/craftax/craftax/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/helmet_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/helmet_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/helmet_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/helmet_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ice_elemental.png` & `craftax-1.4.0/craftax/craftax/assets/ice_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ice_grass.png` & `craftax-1.4.0/craftax/craftax/assets/ice_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ice_shrub.png` & `craftax-1.4.0/craftax/craftax/assets/ice_shrub.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iceball.png` & `craftax-1.4.0/craftax/craftax/assets/iceball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/intelligence.png` & `craftax-1.4.0/craftax/craftax/assets/intelligence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron.png` & `craftax-1.4.0/craftax/craftax/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_boots.png` & `craftax-1.4.0/craftax/craftax/assets/iron_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_chestplate.png` & `craftax-1.4.0/craftax/craftax/assets/iron_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_helmet.png` & `craftax-1.4.0/craftax/craftax/assets/iron_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_pants.png` & `craftax-1.4.0/craftax/craftax/assets/iron_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_pickaxe.png` & `craftax-1.4.0/craftax/craftax/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/iron_sword.png` & `craftax-1.4.0/craftax/craftax/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/knight.png` & `craftax-1.4.0/craftax/craftax/assets/knight.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/knight_archer.png` & `craftax-1.4.0/craftax/craftax/assets/knight_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/kobold.png` & `craftax-1.4.0/craftax/craftax/assets/kobold.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ladder_down.png` & `craftax-1.4.0/craftax/craftax/assets/ladder_down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ladder_down_blocked.png` & `craftax-1.4.0/craftax/craftax/assets/ladder_down_blocked.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ladder_up.png` & `craftax-1.4.0/craftax/craftax/assets/ladder_up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/lava.png` & `craftax-1.4.0/craftax/craftax/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/leaves.png` & `craftax-1.4.0/craftax/craftax/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/lizard.png` & `craftax-1.4.0/craftax/craftax/assets/lizard.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/log.png` & `craftax-1.4.0/craftax/craftax/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/mana.png` & `craftax-1.4.0/craftax/craftax/assets/mana.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/necromancer.png` & `craftax-1.4.0/craftax/craftax/assets/necromancer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/necromancer_vulnerable.png` & `craftax-1.4.0/craftax/craftax/assets/necromancer_vulnerable.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/orc_mage.png` & `craftax-1.4.0/craftax/craftax/assets/orc_mage.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/orc_soldier.png` & `craftax-1.4.0/craftax/craftax/assets/orc_soldier.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/pants_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/pants_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/pants_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/pants_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/path.png` & `craftax-1.4.0/craftax/craftax/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/pigman.png` & `craftax-1.4.0/craftax/craftax/assets/pigman.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/plant-ripe.png` & `craftax-1.4.0/craftax/craftax/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/plant-young.png` & `craftax-1.4.0/craftax/craftax/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/plant.png` & `craftax-1.4.0/craftax/craftax/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player-down.png` & `craftax-1.4.0/craftax/craftax/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player-left.png` & `craftax-1.4.0/craftax/craftax/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player-right.png` & `craftax-1.4.0/craftax/craftax/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player-sleep.png` & `craftax-1.4.0/craftax/craftax/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player-up.png` & `craftax-1.4.0/craftax/craftax/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/player.png` & `craftax-1.4.0/craftax/craftax/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_blue.png` & `craftax-1.4.0/craftax/craftax/assets/potion_blue.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_cyan.png` & `craftax-1.4.0/craftax/craftax/assets/potion_cyan.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_green.png` & `craftax-1.4.0/craftax/craftax/assets/potion_green.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_pink.png` & `craftax-1.4.0/craftax/craftax/assets/potion_pink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_red.png` & `craftax-1.4.0/craftax/craftax/assets/potion_red.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/potion_yellow.png` & `craftax-1.4.0/craftax/craftax/assets/potion_yellow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/ruby.png` & `craftax-1.4.0/craftax/craftax/assets/ruby.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/sand.png` & `craftax-1.4.0/craftax/craftax/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/sapling.png` & `craftax-1.4.0/craftax/craftax/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/sapphire.png` & `craftax-1.4.0/craftax/craftax/assets/sapphire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/skeleton.png` & `craftax-1.4.0/craftax/craftax/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/slimeball.png` & `craftax-1.4.0/craftax/craftax/assets/slimeball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/snail.png` & `craftax-1.4.0/craftax/craftax/assets/snail.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/spider.png` & `craftax-1.4.0/craftax/craftax/assets/spider.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/stalagmite.png` & `craftax-1.4.0/craftax/craftax/assets/stalagmite.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/stone.png` & `craftax-1.4.0/craftax/craftax/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/stone_pickaxe.png` & `craftax-1.4.0/craftax/craftax/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/stone_sword.png` & `craftax-1.4.0/craftax/craftax/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/strength.png` & `craftax-1.4.0/craftax/craftax/assets/strength.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/sword_fire_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/sword_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/sword_ice_enchantment.png` & `craftax-1.4.0/craftax/craftax/assets/sword_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/table.png` & `craftax-1.4.0/craftax/craftax/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/texture_cache.pbz2` & `craftax-1.4.0/craftax/craftax/assets/texture_cache.pbz2`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/torch_in_inventory.png` & `craftax-1.4.0/craftax/craftax/assets/torch_in_inventory.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/torch_on_path.png` & `craftax-1.4.0/craftax/craftax/assets/torch_on_path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/tree.png` & `craftax-1.4.0/craftax/craftax/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/troll.png` & `craftax-1.4.0/craftax/craftax/assets/troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/unknown.png` & `craftax-1.4.0/craftax/craftax/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/water.png` & `craftax-1.4.0/craftax/craftax/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/wood.png` & `craftax-1.4.0/craftax/craftax/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/wood_pickaxe.png` & `craftax-1.4.0/craftax/craftax/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/wood_sword.png` & `craftax-1.4.0/craftax/craftax/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/xp.png` & `craftax-1.4.0/craftax/craftax/assets/xp.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/assets/zombie.png` & `craftax-1.4.0/craftax/craftax/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/constants.py` & `craftax-1.4.0/craftax/craftax/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # GAME CONSTANTS
 OBS_DIM = (9, 11)
 assert OBS_DIM[0] % 2 == 1 and OBS_DIM[1] % 2 == 1
 MAX_OBS_DIM = max(OBS_DIM)
 BLOCK_PIXEL_SIZE_HUMAN = 64
 BLOCK_PIXEL_SIZE_IMG = 16
-BLOCK_PIXEL_SIZE_AGENT = 7
+BLOCK_PIXEL_SIZE_AGENT = 10
 INVENTORY_OBS_HEIGHT = 4
 TEXTURE_CACHE_FILE = os.path.join(
     pathlib.Path(__file__).parent.resolve(), "assets", "texture_cache.pbz2"
 )
 
 # ENUMS
 class BlockType(Enum):
```

### Comparing `craftax-1.3.0/craftax/craftax/craftax_state.py` & `craftax-1.4.0/craftax/craftax/craftax_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,14 @@
     position: jnp.ndarray
     health: jnp.ndarray
     mask: jnp.ndarray
     attack_cooldown: jnp.ndarray
     type_id: jnp.ndarray
 
 
-# @struct.dataclass
-# class Projectiles(Mobs):
-#     directions: jnp.ndarray
-#     lifetimes: jnp.ndarray
-
-
 @struct.dataclass
 class EnvState:
     map: jnp.ndarray
     item_map: jnp.ndarray
     mob_map: jnp.ndarray
     light_map: jnp.ndarray
     down_ladders: jnp.ndarray
@@ -115,17 +109,15 @@
 
 
 @struct.dataclass
 class EnvParams:
     max_timesteps: int = 100000
     day_length: int = 300
 
-    melee_mob_health: int = 5
-    passive_mob_health: int = 3
-    ranged_mob_health: int = 3
+    always_diamond: bool = False
 
     mob_despawn_distance: int = 14
     max_attribute: int = 5
 
     god_mode: bool = False
 
     fractal_noise_angles: tuple[int, int, int, int] = (None, None, None, None)
```

### Comparing `craftax-1.3.0/craftax/craftax/envs/craftax_pixels_env.py` & `craftax-1.4.0/craftax/craftax/envs/craftax_pixels_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from jax import lax
-from gymnax.environments import spaces
+from gymnax.environments import spaces, environment
 from typing import Tuple, Optional
 import chex
 
-from craftax.craftax.envs.common import compute_score
 from craftax.craftax.constants import *
-from craftax.craftax.game_logic import craftax_step
+from craftax.craftax.game_logic import craftax_step, is_game_over
 from craftax.craftax.craftax_state import EnvState, EnvParams, StaticEnvParams
 from craftax.craftax.renderer import render_craftax_pixels
-from craftax.craftax.util.game_logic_utils import has_beaten_boss
 from craftax.craftax.world_gen.world_gen import generate_world
-from craftax.environment_base.environment_no_auto_reset import EnvironmentNoAutoReset
+from craftax.environment_base.environment_bases import EnvironmentNoAutoReset
 
 
-class CraftaxPixelsEnv(EnvironmentNoAutoReset):
+class CraftaxPixelsEnvNoAutoReset(EnvironmentNoAutoReset):
     def __init__(self, static_env_params: Optional[StaticEnvParams] = None):
         super().__init__()
 
         if static_env_params is None:
-            static_env_params = CraftaxPixelsEnv.default_static_params()
+            static_env_params = self.default_static_params()
         self.static_env_params = static_env_params
 
     @property
     def default_params(self) -> EnvParams:
         return EnvParams()
 
     @staticmethod
@@ -32,16 +30,15 @@
     def step_env(
         self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
 
         state, reward = craftax_step(key, state, action, params, self.static_env_params)
 
         done = self.is_terminal(state, params)
-        info = compute_score(state, done)
-        info["discount"] = self.discount(state, params)
+        info = {"discount": self.discount(state, params)}
 
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
             reward,
             done,
             info,
@@ -55,22 +52,86 @@
         return self.get_obs(state), state
 
     def get_obs(self, state: EnvState) -> chex.Array:
         pixels = render_craftax_pixels(state, BLOCK_PIXEL_SIZE_AGENT) / 255.0
         return pixels
 
     def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
-        done_steps = state.timestep >= params.max_timesteps
-        is_dead = state.player_health <= 0
-        defeated_boss = has_beaten_boss(state, self.static_env_params)
+        return is_game_over(state, params, self.static_env_params)
 
-        is_terminal = jnp.logical_or(is_dead, done_steps)
-        is_terminal = jnp.logical_or(is_terminal, defeated_boss)
+    @property
+    def name(self) -> str:
+        return "Craftax-Pixels-NoAutoReset-v1"
+
+    @property
+    def num_actions(self) -> int:
+        return len(Action)
+
+    def action_space(self, params: Optional[EnvParams] = None) -> spaces.Discrete:
+        return spaces.Discrete(len(Action))
+
+    def observation_space(self, params: EnvParams) -> spaces.Box:
+        return spaces.Box(
+            0.0,
+            1.0,
+            (
+                OBS_DIM[1] * BLOCK_PIXEL_SIZE_AGENT,
+                (OBS_DIM[0] + INVENTORY_OBS_HEIGHT) * BLOCK_PIXEL_SIZE_AGENT,
+                3,
+            ),
+            dtype=jnp.int32,
+        )
+
+
+class CraftaxPixelsEnv(environment.Environment):
+    def __init__(self, static_env_params: Optional[StaticEnvParams] = None):
+        super().__init__()
+
+        if static_env_params is None:
+            static_env_params = self.default_static_params()
+        self.static_env_params = static_env_params
 
-        return is_terminal
+    @property
+    def default_params(self) -> EnvParams:
+        return EnvParams()
+
+    @staticmethod
+    def default_static_params() -> StaticEnvParams:
+        return StaticEnvParams()
+
+    def step_env(
+        self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
+    ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
+
+        state, reward = craftax_step(key, state, action, params, self.static_env_params)
+
+        done = self.is_terminal(state, params)
+        info = {"discount": self.discount(state, params)}
+
+        return (
+            lax.stop_gradient(self.get_obs(state)),
+            lax.stop_gradient(state),
+            reward,
+            done,
+            info,
+        )
+
+    def reset_env(
+        self, rng: chex.PRNGKey, params: EnvParams
+    ) -> Tuple[chex.Array, EnvState]:
+        state = generate_world(rng, params, self.static_env_params)
+
+        return self.get_obs(state), state
+
+    def get_obs(self, state: EnvState) -> chex.Array:
+        pixels = render_craftax_pixels(state, BLOCK_PIXEL_SIZE_AGENT) / 255.0
+        return pixels
+
+    def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
+        return is_game_over(state, params, self.static_env_params)
 
     @property
     def name(self) -> str:
         return "Craftax-Pixels-v1"
 
     @property
     def num_actions(self) -> int:
```

### Comparing `craftax-1.3.0/craftax/craftax/envs/craftax_symbolic_env.py` & `craftax-1.4.0/craftax/craftax_classic/envs/craftax_symbolic_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,53 @@
-import jax
 from jax import lax
-from gymnax.environments import spaces
+from gymnax.environments import spaces, environment
 from typing import Tuple, Optional
 import chex
 
-from craftax.craftax.envs.common import compute_score
-from craftax.environment_base.environment_no_auto_reset import EnvironmentNoAutoReset
-from craftax.craftax.constants import *
-from craftax.craftax.game_logic import craftax_step
-from craftax.craftax.craftax_state import EnvState, EnvParams, StaticEnvParams
-from craftax.craftax.renderer import render_craftax_symbolic
-from craftax.craftax.util.game_logic_utils import has_beaten_boss
-from craftax.craftax.world_gen.world_gen import generate_world
+from craftax.environment_base.environment_bases import EnvironmentNoAutoReset
+from craftax.craftax_classic.envs.common import compute_score
+from craftax.craftax_classic.constants import *
+from craftax.craftax_classic.game_logic import craftax_step, is_game_over
+from craftax.craftax_classic.envs.craftax_state import (
+    EnvState,
+    EnvParams,
+    StaticEnvParams,
+)
+from craftax.craftax_classic.renderer import render_craftax_symbolic
+from craftax.craftax_classic.world_gen import generate_world
 
 
-class CraftaxSymbolicEnv(EnvironmentNoAutoReset):
-    def __init__(self, static_env_params: Optional[StaticEnvParams] = None):
+def get_map_obs_shape():
+    num_mobs = 4
+    num_blocks = len(BlockType)
+
+    return OBS_DIM[0], OBS_DIM[1], num_blocks + num_mobs
+
+
+def get_flat_map_obs_shape():
+    map_obs_shape = get_map_obs_shape()
+    return map_obs_shape[0] * map_obs_shape[1] * map_obs_shape[2]
+
+
+def get_inventory_obs_shape():
+    inv_size = 12
+    num_intrinsics = 4
+    light_level = 1
+    is_sleeping = 1
+    direction = 4
+
+    return inv_size + num_intrinsics + light_level + is_sleeping + direction
+
+
+class CraftaxClassicSymbolicEnvNoAutoReset(EnvironmentNoAutoReset):
+    def __init__(self, static_env_params: StaticEnvParams = None):
         super().__init__()
 
         if static_env_params is None:
-            static_env_params = CraftaxSymbolicEnv.default_static_params()
+            static_env_params = self.default_static_params()
         self.static_env_params = static_env_params
 
     @property
     def default_params(self) -> EnvParams:
         return EnvParams()
 
     @staticmethod
@@ -46,69 +70,111 @@
             done,
             info,
         )
 
     def reset_env(
         self, rng: chex.PRNGKey, params: EnvParams
     ) -> Tuple[chex.Array, EnvState]:
-        rng, _rng = jax.random.split(rng)
-        state = generate_world(_rng, params, self.static_env_params)
+        state = generate_world(rng, params, self.static_env_params)
 
         return self.get_obs(state), state
 
     def get_obs(self, state: EnvState) -> chex.Array:
         pixels = render_craftax_symbolic(state)
         return pixels
 
     def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
-        done_steps = state.timestep >= params.max_timesteps
-        is_dead = state.player_health <= 0
-        defeated_boss = has_beaten_boss(state, self.static_env_params)
-
-        is_terminal = jnp.logical_or(is_dead, done_steps)
-        is_terminal = jnp.logical_or(is_terminal, defeated_boss)
-
-        return is_terminal
+        return is_game_over(state, params)
 
     @property
     def name(self) -> str:
-        return "Craftax-Symbolic-v1"
+        return "Craftax-Classic-Symbolic-NoAutoReset-v1"
 
     @property
     def num_actions(self) -> int:
-        return len(Action)
+        return 17
 
     def action_space(self, params: Optional[EnvParams] = None) -> spaces.Discrete:
-        return spaces.Discrete(len(Action))
+        return spaces.Discrete(17)
+
+    def observation_space(self, params: EnvParams) -> spaces.Box:
+        flat_map_obs_shape = get_flat_map_obs_shape()
+        inventory_obs_shape = get_inventory_obs_shape()
+
+        obs_shape = flat_map_obs_shape + inventory_obs_shape
+
+        return spaces.Box(
+            0.0,
+            1.0,
+            (obs_shape,),
+            dtype=jnp.int32,
+        )
+
+
+class CraftaxClassicSymbolicEnv(environment.Environment):
+    def __init__(self, static_env_params: StaticEnvParams = None):
+        super().__init__()
+
+        if static_env_params is None:
+            static_env_params = self.default_static_params()
+        self.static_env_params = static_env_params
+
+    @property
+    def default_params(self) -> EnvParams:
+        return EnvParams()
 
     @staticmethod
-    def get_map_obs_shape():
-        num_mob_classes = 5
-        num_mob_types = 8
-        num_blocks = len(BlockType)
-        num_items = len(ItemType)
+    def default_static_params() -> StaticEnvParams:
+        return StaticEnvParams()
+
+    def step_env(
+        self, rng: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
+    ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
+        state, reward = craftax_step(rng, state, action, params, self.static_env_params)
+
+        done = self.is_terminal(state, params)
+        info = compute_score(state, done)
+        info["discount"] = self.discount(state, params)
 
         return (
-            OBS_DIM[0],
-            OBS_DIM[1],
-            num_blocks + num_items + num_mob_classes * num_mob_types + 1,
+            lax.stop_gradient(self.get_obs(state)),
+            lax.stop_gradient(state),
+            reward,
+            done,
+            info,
         )
 
-    @staticmethod
-    def get_flat_map_obs_shape():
-        map_obs_shape = CraftaxSymbolicEnv.get_map_obs_shape()
-        return map_obs_shape[0] * map_obs_shape[1] * map_obs_shape[2]
+    def reset_env(
+        self, rng: chex.PRNGKey, params: EnvParams
+    ) -> Tuple[chex.Array, EnvState]:
+        state = generate_world(rng, params, self.static_env_params)
 
-    @staticmethod
-    def get_inventory_obs_shape():
-        return 51
+        return self.get_obs(state), state
+
+    def get_obs(self, state: EnvState) -> chex.Array:
+        pixels = render_craftax_symbolic(state)
+        return pixels
+
+    def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
+        return is_game_over(state, params)
+
+    @property
+    def name(self) -> str:
+        return "Craftax-Classic-Symbolic-v1"
+
+    @property
+    def num_actions(self) -> int:
+        return 17
+
+    def action_space(self, params: Optional[EnvParams] = None) -> spaces.Discrete:
+        return spaces.Discrete(17)
 
     def observation_space(self, params: EnvParams) -> spaces.Box:
-        flat_map_obs_shape = self.get_flat_map_obs_shape()
-        inventory_obs_shape = self.get_inventory_obs_shape()
+        flat_map_obs_shape = get_flat_map_obs_shape()
+        inventory_obs_shape = get_inventory_obs_shape()
 
         obs_shape = flat_map_obs_shape + inventory_obs_shape
 
         return spaces.Box(
             0.0,
             1.0,
             (obs_shape,),
```

### Comparing `craftax-1.3.0/craftax/craftax/game_logic.py` & `craftax-1.4.0/craftax/craftax/game_logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from craftax.craftax.util.game_logic_utils import *
 
 
+def is_game_over(state, params, static_env_params):
+    done_steps = state.timestep >= params.max_timesteps
+    is_dead = state.player_health <= 0
+    defeated_boss = has_beaten_boss(state, static_env_params)
+
+    return done_steps | is_dead | defeated_boss
+
+
 def update_plants_with_eat(state, plant_position, static_params):
     def _is_plant(unused, index):
         return None, (state.growing_plants_positions[index] == plant_position).all()
 
     _, is_plant = jax.lax.scan(
         _is_plant, None, jnp.arange(static_params.max_growing_plants)
     )
```

### Comparing `craftax-1.3.0/craftax/craftax/play_craftax.py` & `craftax-1.4.0/craftax/craftax/play_craftax.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,32 +94,32 @@
         pygame.init()
         pygame.key.set_repeat(250, 75)
 
         self.screen_surface = pygame.display.set_mode(self.screen_size)
 
         self._render = jax.jit(render_craftax_pixels, static_argnums=(1,))
 
-    def render(self, env_state):
+    def update(self):
         # Update pygame events
         self.pygame_events = list(pygame.event.get())
 
+        # Update screen
+        pygame.display.flip()
+
+    def render(self, env_state):
         # Clear
         self.screen_surface.fill((0, 0, 0))
 
         pixels = self._render(env_state, block_pixel_size=BLOCK_PIXEL_SIZE_HUMAN)
         pixels = jnp.repeat(pixels, repeats=self.pixel_render_size, axis=0)
         pixels = jnp.repeat(pixels, repeats=self.pixel_render_size, axis=1)
 
         surface = pygame.surfarray.make_surface(np.array(pixels).transpose((1, 0, 2)))
         self.screen_surface.blit(surface, (0, 0))
 
-        # Update screen
-        pygame.display.flip()
-        # time.sleep(0.01)
-
     def is_quit_requested(self):
         for event in self.pygame_events:
             if event.type == pygame.QUIT:
                 return True
         return False
 
     def get_action_from_keypress(self, state):
@@ -157,43 +157,46 @@
     rng = jax.random.PRNGKey(np.random.randint(2**31))
     rng, _rng = jax.random.split(rng)
     obs, env_state = env.reset(_rng, env_params)
 
     pixel_render_size = 64 // BLOCK_PIXEL_SIZE_HUMAN
 
     renderer = CraftaxRenderer(env, env_params, pixel_render_size=pixel_render_size)
+    renderer.render(env_state)
 
     step_fn = jax.jit(env.step)
 
     traj_history = {"state": [env_state], "action": [], "reward": [], "done": []}
 
+    clock = pygame.time.Clock()
+
     while not renderer.is_quit_requested():
         action = renderer.get_action_from_keypress(env_state)
 
         if action is not None:
             rng, _rng = jax.random.split(rng)
             old_achievements = env_state.achievements
             obs, env_state, reward, done, info = step_fn(
                 _rng, env_state, action, env_params
             )
             new_achievements = env_state.achievements
             print_new_achievements(old_achievements, new_achievements)
 
-            if done:
-                obs, env_state = env.reset(_rng, env_params)
-
             if reward > 0.8:
                 print(f"Reward: {reward}\n")
 
             traj_history["state"].append(env_state)
             traj_history["action"].append(action)
             traj_history["reward"].append(reward)
             traj_history["done"].append(done)
 
-        renderer.render(env_state)
+            renderer.render(env_state)
+
+        renderer.update()
+        clock.tick(args.fps)
 
     if args.save_trajectories:
         save_name = f"play_data/trajectories_{int(time.time())}"
         if args.god_mode:
             save_name += "_GM"
         save_name += ".pkl"
         Path("play_data").mkdir(parents=True, exist_ok=True)
@@ -201,14 +204,15 @@
 
 
 def entry_point():
     parser = argparse.ArgumentParser()
     parser.add_argument("--god_mode", action="store_true")
     parser.add_argument("--debug", action="store_true")
     parser.add_argument("--save_trajectories", action="store_true")
+    parser.add_argument("--fps", type=int, default=60)
 
     args, rest_args = parser.parse_known_args(sys.argv[1:])
     if rest_args:
         raise ValueError(f"Unknown args {rest_args}")
 
     if args.debug:
         with jax.disable_jit():
```

### Comparing `craftax-1.3.0/craftax/craftax/renderer.py` & `craftax-1.4.0/craftax/craftax/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/util/game_logic_utils.py` & `craftax-1.4.0/craftax/craftax/util/game_logic_utils.py`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax/util/noise.py` & `craftax-1.4.0/craftax/craftax_classic/util/noise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
 
+# Code adapted for JAX from the original numpy implementation made by Pierre Vigier
+# Original code located at https://github.com/pvigier/perlin-numpy
+
+
 def interpolant(t):
     return t * t * t * (t * (t * 6 - 15) + 10)
 
 
 def generate_perlin_noise_2d(
     rng, shape, res, interpolant=interpolant, override_angles=None
 ):
```

### Comparing `craftax-1.3.0/craftax/craftax/world_gen/world_gen.py` & `craftax-1.4.0/craftax/craftax/world_gen/world_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,20 +350,15 @@
     item_map = item_map.at[ladder_up_position[0], ladder_up_position[1]].set(
         ItemType.LADDER_UP.value
     )
 
     return map, item_map, light_map, ladder_down_position, ladder_up_position
 
 
-def generate_smoothworld(rng, static_params, player_position, config, params=None):
-    if params is not None:
-        fractal_noise_angles = params.fractal_noise_angles
-    else:
-        fractal_noise_angles = (None, None, None, None, None)
-
+def generate_smoothworld(rng, static_params, player_position, config, params):
     player_proximity_map = get_distance_map(
         player_position, static_params.map_size
     ).astype(jnp.float32)
     player_proximity_map_water = (
         player_proximity_map / config.player_proximity_map_water_strength
     )
     player_proximity_map_water = jnp.clip(
@@ -385,15 +380,15 @@
 
     rng, _rng = jax.random.split(rng)
     water = generate_fractal_noise_2d(
         _rng,
         static_params.map_size,
         small_res,
         octaves=1,
-        override_angles=fractal_noise_angles[0],
+        override_angles=params.fractal_noise_angles[0],
     )
     water = water + player_proximity_map_water - 1.0
 
     # Water
     rng, _rng = jax.random.split(rng)
     map = jnp.where(
         water > config.water_threshold, config.sea_block, config.default_block
@@ -412,29 +407,29 @@
     rng, _rng = jax.random.split(rng)
     mountain = (
         generate_fractal_noise_2d(
             _rng,
             static_params.map_size,
             small_res,
             octaves=1,
-            override_angles=fractal_noise_angles[1],
+            override_angles=params.fractal_noise_angles[1],
         )
         + 0.05
     )
     mountain = mountain + player_proximity_map_mountain - 1.0
     map = jnp.where(mountain > mountain_threshold, config.mountain_block, map)
 
     # Paths
     rng, _rng = jax.random.split(rng)
     path_x = generate_fractal_noise_2d(
         _rng,
         static_params.map_size,
         x_res,
         octaves=1,
-        override_angles=fractal_noise_angles[2],
+        override_angles=params.fractal_noise_angles[2],
     )
     path = jnp.logical_and(mountain > mountain_threshold, path_x > 0.8)
     map = jnp.where(path > 0.5, config.path_block, map)
 
     path_y = path_x.T
     path = jnp.logical_and(mountain > mountain_threshold, path_y > 0.8)
     map = jnp.where(path > 0.5, config.path_block, map)
@@ -447,15 +442,15 @@
     # Trees
     rng, _rng = jax.random.split(rng)
     tree_noise = generate_fractal_noise_2d(
         _rng,
         static_params.map_size,
         larger_res,
         octaves=1,
-        override_angles=fractal_noise_angles[3],
+        override_angles=params.fractal_noise_angles[3],
     )
     tree = (tree_noise > config.tree_threshold_perlin) * jax.random.uniform(
         rng, shape=static_params.map_size
     ) > config.tree_threshold_uniform
     tree = jnp.logical_and(tree, map == config.tree_requirement_block)
     map = jnp.where(tree, config.tree, map)
 
@@ -478,14 +473,37 @@
     # Lava
     lava_map = jnp.logical_and(
         mountain > 0.85,
         tree_noise > 0.7,
     )
     map = jnp.where(lava_map, config.lava, map)
 
+    # Add diamond if always_diamond flag is set
+    adding_diamond = jnp.logical_and(
+        config.default_block == BlockType.GRASS.value,  # Hacky check for overworld
+        params.always_diamond,
+    )
+    valid_diamond = (map.flatten() == BlockType.STONE.value).astype(jnp.float32)
+    rng, _rng = jax.random.split(rng)
+    diamond_index = jax.random.choice(
+        _rng,
+        jnp.arange(static_params.map_size[0] * static_params.map_size[1]),
+        p=valid_diamond / valid_diamond.sum(),
+    )
+    diamond_position = jnp.array(
+        [
+            diamond_index // static_params.map_size[0],
+            diamond_index % static_params.map_size[0],
+        ]
+    )
+    diamond_replace_block = jax.lax.select(
+        adding_diamond, BlockType.DIAMOND.value, BlockType.STONE.value
+    )
+    map = map.at[diamond_position[0], diamond_position[1]].set(diamond_replace_block)
+
     # Light map
     light_map = (
         jnp.ones(static_params.map_size, dtype=jnp.float32) * config.default_light
     )
 
     # Make sure player spawns on grass
     map = map.at[player_position[0], player_position[1]].set(config.player_spawn)
@@ -552,33 +570,16 @@
         [static_params.map_size[0] // 2, static_params.map_size[1] // 2]
     )
 
     # Generate smoothgens (overworld, caves, elemental levels, boss level)
     rngs = jax.random.split(rng, 7)
     rng, _rng = rngs[0], rngs[1:]
 
-    overworld = generate_smoothworld(
-        _rng[0],
-        static_params,
-        player_position,
-        jax.tree_map(lambda x: x[0], ALL_SMOOTHGEN_CONFIGS),
-        params=params,
-    )
-
-    smoothgens = jax.vmap(generate_smoothworld, in_axes=(0, None, None, 0))(
-        _rng[1:],
-        static_params,
-        player_position,
-        jax.tree_map(lambda x: x[1:], ALL_SMOOTHGEN_CONFIGS),
-    )
-
-    smoothgens = jax.tree_map(
-        lambda over, others: jnp.concatenate([jnp.array([over]), others], axis=0),
-        overworld,
-        smoothgens,
+    smoothgens = jax.vmap(generate_smoothworld, in_axes=(0, None, None, 0, None))(
+        _rng, static_params, player_position, ALL_SMOOTHGEN_CONFIGS, params
     )
 
     # Generate dungeons
     rngs = jax.random.split(rng, 4)
     rng, _rng = rngs[0], rngs[1:]
     dungeons = jax.vmap(generate_dungeon, in_axes=(0, None, 0))(
         _rng, static_params, ALL_DUNGEON_CONFIGS
```

### Comparing `craftax-1.3.0/craftax/craftax/world_gen/world_gen_configs.py` & `craftax-1.4.0/craftax/craftax/world_gen/world_gen_configs.py`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/1.png` & `craftax-1.4.0/craftax/craftax_classic/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/2.png` & `craftax-1.4.0/craftax/craftax_classic/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/3.png` & `craftax-1.4.0/craftax/craftax_classic/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/4.png` & `craftax-1.4.0/craftax/craftax_classic/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/5.png` & `craftax-1.4.0/craftax/craftax_classic/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/6.png` & `craftax-1.4.0/craftax/craftax_classic/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/7.png` & `craftax-1.4.0/craftax/craftax_classic/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/8.png` & `craftax-1.4.0/craftax/craftax_classic/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/9.png` & `craftax-1.4.0/craftax/craftax_classic/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/arrow-down.png` & `craftax-1.4.0/craftax/craftax_classic/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/arrow-left.png` & `craftax-1.4.0/craftax/craftax_classic/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/arrow-right.png` & `craftax-1.4.0/craftax/craftax_classic/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/arrow-up.png` & `craftax-1.4.0/craftax/craftax_classic/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/coal.png` & `craftax-1.4.0/craftax/craftax_classic/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/cow.png` & `craftax-1.4.0/craftax/craftax_classic/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/debug-2.png` & `craftax-1.4.0/craftax/craftax_classic/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/debug-3.png` & `craftax-1.4.0/craftax/craftax_classic/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/debug.png` & `craftax-1.4.0/craftax/craftax_classic/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/diamond.png` & `craftax-1.4.0/craftax/craftax_classic/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/drink.png` & `craftax-1.4.0/craftax/craftax_classic/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/energy.png` & `craftax-1.4.0/craftax/craftax_classic/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/fence.png` & `craftax-1.4.0/craftax/craftax_classic/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/food.png` & `craftax-1.4.0/craftax/craftax_classic/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/furnace.png` & `craftax-1.4.0/craftax/craftax_classic/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/grass.png` & `craftax-1.4.0/craftax/craftax_classic/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/health.png` & `craftax-1.4.0/craftax/craftax_classic/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/iron.png` & `craftax-1.4.0/craftax/craftax_classic/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/iron_pickaxe.png` & `craftax-1.4.0/craftax/craftax_classic/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/iron_sword.png` & `craftax-1.4.0/craftax/craftax_classic/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/lava.png` & `craftax-1.4.0/craftax/craftax_classic/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/leaves.png` & `craftax-1.4.0/craftax/craftax_classic/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/log.png` & `craftax-1.4.0/craftax/craftax_classic/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/path.png` & `craftax-1.4.0/craftax/craftax_classic/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/plant-ripe.png` & `craftax-1.4.0/craftax/craftax_classic/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/plant-young.png` & `craftax-1.4.0/craftax/craftax_classic/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/plant.png` & `craftax-1.4.0/craftax/craftax_classic/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player-down.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player-left.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player-right.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player-sleep.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player-up.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/player.png` & `craftax-1.4.0/craftax/craftax_classic/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/sand.png` & `craftax-1.4.0/craftax/craftax_classic/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/sapling.png` & `craftax-1.4.0/craftax/craftax_classic/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/skeleton.png` & `craftax-1.4.0/craftax/craftax_classic/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/stone.png` & `craftax-1.4.0/craftax/craftax_classic/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/stone_pickaxe.png` & `craftax-1.4.0/craftax/craftax_classic/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/stone_sword.png` & `craftax-1.4.0/craftax/craftax_classic/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/table.png` & `craftax-1.4.0/craftax/craftax_classic/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/tree.png` & `craftax-1.4.0/craftax/craftax_classic/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/unknown.png` & `craftax-1.4.0/craftax/craftax_classic/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/water.png` & `craftax-1.4.0/craftax/craftax_classic/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/wood.png` & `craftax-1.4.0/craftax/craftax_classic/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/wood_pickaxe.png` & `craftax-1.4.0/craftax/craftax_classic/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/wood_sword.png` & `craftax-1.4.0/craftax/craftax_classic/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/assets/zombie.png` & `craftax-1.4.0/craftax/craftax_classic/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/constants.py` & `craftax-1.4.0/craftax/craftax_classic/constants.py`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/envs/craftax_pixels_env.py` & `craftax-1.4.0/craftax/environment_base/environment_bases.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,87 @@
-from jax import lax
-from gymnax.environments import spaces
-from typing import Tuple, Optional
+from dataclasses import dataclass
+
+import jax
 import chex
+from typing import Tuple, Union, Optional
+from functools import partial
+from flax import struct
+
 
-from craftax.environment_base.environment_no_auto_reset import EnvironmentNoAutoReset
-from craftax.craftax_classic.envs.common import compute_score
-from craftax.craftax_classic.constants import *
-from craftax.craftax_classic.game_logic import craftax_step
-from craftax.craftax_classic.envs.craftax_state import (
-    EnvState,
-    EnvParams,
-    StaticEnvParams,
-)
-from craftax.craftax_classic.renderer import render_craftax_pixels
-from craftax.craftax_classic.world_gen import generate_world
-
-
-class CraftaxClassicPixelsEnv(EnvironmentNoAutoReset):
-    def __init__(self, static_env_params: StaticEnvParams = None):
-        super().__init__()
-
-        if static_env_params is None:
-            static_env_params = CraftaxClassicPixelsEnv.default_static_params()
-        self.static_env_params = static_env_params
+class EnvironmentNoAutoReset(object):
+    """Similar to the base Gymnax environment but without auto-resets."""
 
     @property
-    def default_params(self) -> EnvParams:
-        return EnvParams()
+    def default_params(self):
+        return NotImplementedError
 
-    @staticmethod
-    def default_static_params() -> StaticEnvParams:
-        return StaticEnvParams()
+    @partial(jax.jit, static_argnums=(0, 4))
+    def step(
+        self,
+        key: chex.PRNGKey,
+        state,
+        action: Union[int, float],
+        params=None,
+    ):
+        """Performs step transitions in the environment."""
+        # Use default env parameters if no others specified
+        if params is None:
+            params = self.default_params
+        obs, state, reward, done, info = self.step_env(key, state, action, params)
+        return obs, state, reward, done, info
+
+    @partial(jax.jit, static_argnums=(0, 2))
+    def reset(self, key: chex.PRNGKey, params=None):
+        """Performs resetting of environment."""
+        # Use default env parameters if no others specified
+        if params is None:
+            params = self.default_params
+        obs, state = self.reset_env(key, params)
+        return obs, state
 
     def step_env(
-        self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
-    ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
-
-        state, reward = craftax_step(key, state, action, params, self.static_env_params)
-
-        done = self.is_terminal(state, params)
-        info = compute_score(state, done)
-        info["discount"] = self.discount(state, params)
-
-        return (
-            lax.stop_gradient(self.get_obs(state)),
-            lax.stop_gradient(state),
-            reward,
-            done,
-            info,
-        )
-
-    def reset_env(
-        self, rng: chex.PRNGKey, params: EnvParams
-    ) -> Tuple[chex.Array, EnvState]:
-        state = generate_world(rng, params, self.static_env_params)
-
-        return self.get_obs(state), state
-
-    def get_obs(self, state: EnvState) -> chex.Array:
-        pixels = render_craftax_pixels(state, BLOCK_PIXEL_SIZE_AGENT) / 255.0
-        # pixels = render_pixels_empty()
-        return pixels
-
-    def is_terminal(self, state: EnvState, params: EnvParams) -> bool:
-        done_steps = state.timestep >= params.max_timesteps
-        in_lava = (
-            state.map[state.player_position[0], state.player_position[1]]
-            == BlockType.LAVA.value
-        )
-        is_dead = state.player_health <= 0
-
-        is_terminal = jnp.logical_or(done_steps, in_lava)
-        is_terminal = jnp.logical_or(is_terminal, is_dead)
-
-        return is_terminal
+        self,
+        key: chex.PRNGKey,
+        state,
+        action: Union[int, float],
+        params,
+    ):
+        """Environment-specific step transition."""
+        raise NotImplementedError
+
+    def reset_env(self, key: chex.PRNGKey, params):
+        """Environment-specific reset."""
+        raise NotImplementedError
+
+    def get_obs(self, state) -> chex.Array:
+        """Applies observation function to state."""
+        raise NotImplementedError
+
+    def is_terminal(self, state, params) -> bool:
+        """Check whether state transition is terminal."""
+        raise NotImplementedError
+
+    def discount(self, state, params) -> float:
+        """Return a discount of zero if the episode has terminated."""
+        return jax.lax.select(self.is_terminal(state, params), 0.0, 1.0)
 
     @property
     def name(self) -> str:
-        return "Craftax-Classic-Pixels-v1"
+        """Environment name."""
+        return type(self).__name__
 
     @property
     def num_actions(self) -> int:
-        return 17
-
-    def action_space(self, params: Optional[EnvParams] = None) -> spaces.Discrete:
-        return spaces.Discrete(17)
+        """Number of actions possible in environment."""
+        raise NotImplementedError
 
-    def observation_space(self, params: EnvParams) -> spaces.Box:
-        return spaces.Box(
-            0.0,
-            1.0,
-            (
-                OBS_DIM[1] * BLOCK_PIXEL_SIZE_AGENT,
-                (OBS_DIM[0] + INVENTORY_OBS_HEIGHT) * BLOCK_PIXEL_SIZE_AGENT,
-                3,
-            ),
-            dtype=jnp.int32,
-        )
+    def action_space(self, params):
+        """Action space of the environment."""
+        raise NotImplementedError
+
+    def observation_space(self, params):
+        """Observation space of the environment."""
+        raise NotImplementedError
+
+    def state_space(self, params):
+        """State space of the environment."""
+        raise NotImplementedError
```

### Comparing `craftax-1.3.0/craftax/craftax_classic/envs/craftax_state.py` & `craftax-1.4.0/craftax/craftax_classic/envs/craftax_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
 
 @struct.dataclass
 class EnvParams:
     max_timesteps: int = 10000
     day_length: int = 300
 
+    always_diamond: bool = True
+
     zombie_health: int = 5
     cow_health: int = 3
     skeleton_health: int = 3
 
     mob_despawn_distance: int = 14
 
     spawn_cow_chance: float = 0.1
```

### Comparing `craftax-1.3.0/craftax/craftax_classic/game_logic.py` & `craftax-1.4.0/craftax/craftax_classic/game_logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import chex
 
 from craftax.craftax_classic.constants import *
 from craftax.craftax_classic.envs.craftax_state import *
 
 
+def is_game_over(state, params):
+    done_steps = state.timestep >= params.max_timesteps
+    in_lava = (
+        state.map[state.player_position[0], state.player_position[1]]
+        == BlockType.LAVA.value
+    )
+    is_dead = state.player_health <= 0
+
+    return done_steps | in_lava | is_dead
+
+
 def in_bounds(state, position):
     in_bounds_x = jnp.logical_and(0 <= position[0], position[0] < state.map.shape[0])
     in_bounds_y = jnp.logical_and(0 <= position[1], position[1] < state.map.shape[1])
     return jnp.logical_and(in_bounds_x, in_bounds_y)
 
 
 def is_in_wall(state, position):
```

### Comparing `craftax-1.3.0/craftax/craftax_classic/play_craftax_classic.py` & `craftax-1.4.0/craftax/craftax_classic/play_craftax_classic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import argparse
+import sys
+
 import pygame
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from craftax.craftax_classic.constants import (
@@ -11,14 +14,15 @@
     Achievement,
     BLOCK_PIXEL_SIZE_HUMAN,
 )
 from craftax.craftax_classic.envs.craftax_symbolic_env import (
     CraftaxClassicSymbolicEnv as CraftaxEnv,
 )
 from craftax.craftax_classic.renderer import render_craftax_pixels
+from craftax.environment_base.wrappers import AutoResetEnvWrapper
 
 KEY_MAPPING = {
     pygame.K_q: Action.NOOP,
     pygame.K_w: Action.UP,
     pygame.K_d: Action.RIGHT,
     pygame.K_s: Action.DOWN,
     pygame.K_a: Action.LEFT,
@@ -55,32 +59,33 @@
         pygame.init()
         pygame.key.set_repeat(250, 75)
 
         self.screen_surface = pygame.display.set_mode(self.screen_size)
 
         self._render = jax.jit(render_craftax_pixels, static_argnums=(1,))
 
-    def render(self, env_state):
+    def update(self):
         # Update pygame events
         self.pygame_events = list(pygame.event.get())
 
+        # Update screen
+        pygame.display.flip()
+        # time.sleep(0.01)
+
+    def render(self, env_state):
         # Clear
         self.screen_surface.fill((0, 0, 0))
 
         pixels = self._render(env_state, block_pixel_size=BLOCK_PIXEL_SIZE_HUMAN)
         pixels = jnp.repeat(pixels, repeats=self.pixel_render_size, axis=0)
         pixels = jnp.repeat(pixels, repeats=self.pixel_render_size, axis=1)
 
         surface = pygame.surfarray.make_surface(np.array(pixels).transpose((1, 0, 2)))
         self.screen_surface.blit(surface, (0, 0))
 
-        # Update screen
-        pygame.display.flip()
-        # time.sleep(0.01)
-
     def is_quit_requested(self):
         for event in self.pygame_events:
             if event.type == pygame.QUIT:
                 return True
         return False
 
     def get_action_from_keypress(self, state):
@@ -96,32 +101,36 @@
 
 def print_new_achievements(old_achievements, new_achievements):
     for i in range(len(old_achievements)):
         if old_achievements[i] == 0 and new_achievements[i] == 1:
             print(f"{Achievement(i).name} ({new_achievements.sum()}/{22})")
 
 
-def main():
+def main(args):
     env = CraftaxEnv(CraftaxEnv.default_static_params())
+    env = AutoResetEnvWrapper(env)
     env_params = env.default_params
 
     print("Controls")
     for k, v in KEY_MAPPING.items():
         print(f"{pygame.key.name(k)}: {v.name.lower()}")
 
     rng = jax.random.PRNGKey(np.random.randint(2**31))
     rng, _rng = jax.random.split(rng)
     _, env_state = env.reset(_rng, env_params)
 
     pixel_render_size = 64 // BLOCK_PIXEL_SIZE_HUMAN
 
     renderer = CraftaxRenderer(env, env_params, pixel_render_size=pixel_render_size)
+    renderer.render(env_state)
 
     step_fn = jax.jit(env.step)
 
+    clock = pygame.time.Clock()
+
     while not renderer.is_quit_requested():
         action = renderer.get_action_from_keypress(env_state)
 
         if action is not None:
             rng, _rng = jax.random.split(rng)
             old_achievements = env_state.achievements
             obs, env_state, reward, done, info = step_fn(
@@ -129,17 +138,31 @@
             )
             new_achievements = env_state.achievements
             print_new_achievements(old_achievements, new_achievements)
 
             if reward > 0.01 or reward < -0.01:
                 print(f"Reward: {reward}\n")
 
-        renderer.render(env_state)
+            renderer.render(env_state)
 
+        renderer.update()
+        clock.tick(args.fps)
 
-if __name__ == "__main__":
-    debug = False
-    if debug:
+
+def entry_point():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--debug", action="store_true")
+    parser.add_argument("--fps", type=int, default=60)
+
+    args, rest_args = parser.parse_known_args(sys.argv[1:])
+    if rest_args:
+        raise ValueError(f"Unknown args {rest_args}")
+
+    if args.debug:
         with jax.disable_jit():
-            main()
+            main(args)
     else:
-        main()
+        main(args)
+
+
+if __name__ == "__main__":
+    entry_point()
```

### Comparing `craftax-1.3.0/craftax/craftax_classic/renderer.py` & `craftax-1.4.0/craftax/craftax_classic/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.3.0/craftax/craftax_classic/util/noise.py` & `craftax-1.4.0/craftax/craftax/util/noise.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import jax
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
+# Code adapted for JAX from the original numpy implementation made by Pierre Vigier
+# Original code located at https://github.com/pvigier/perlin-numpy
+
 
 def interpolant(t):
     return t * t * t * (t * (t * 6 - 15) + 10)
 
 
 def generate_perlin_noise_2d(
     rng, shape, res, interpolant=interpolant, override_angles=None
```

### Comparing `craftax-1.3.0/craftax/craftax_classic/world_gen.py` & `craftax-1.4.0/craftax/craftax_classic/world_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,33 @@
         tree_noise > 0.7,
     )
     map = jnp.where(lava_map, BlockType.LAVA.value, map)
 
     # Make sure player spawns on grass
     map = map.at[player_position[0], player_position[1]].set(BlockType.GRASS.value)
 
+    # Add diamond if always_diamond flag is set
+    valid_diamond = (map.flatten() == BlockType.STONE.value).astype(jnp.float32)
+    rng, _rng = jax.random.split(rng)
+    diamond_index = jax.random.choice(
+        _rng,
+        jnp.arange(static_params.map_size[0] * static_params.map_size[1]),
+        p=valid_diamond / valid_diamond.sum(),
+    )
+    diamond_position = jnp.array(
+        [
+            diamond_index // static_params.map_size[0],
+            diamond_index % static_params.map_size[0],
+        ]
+    )
+    diamond_replace_block = jax.lax.select(
+        params.always_diamond, BlockType.DIAMOND.value, BlockType.STONE.value
+    )
+    map = map.at[diamond_position[0], diamond_position[1]].set(diamond_replace_block)
+
     # Zombies
 
     z_pos = jnp.zeros((static_params.max_zombies, 2), dtype=jnp.int32)
     z_health = jnp.ones(static_params.max_zombies, dtype=jnp.int32)
     z_mask = jnp.zeros(static_params.max_zombies, dtype=bool)
 
     # z_pos = z_pos.at[0].set(player_position + jnp.array([1, 0]))
```

### Comparing `craftax-1.3.0/craftax/environment_base/wrappers.py` & `craftax-1.4.0/craftax/environment_base/wrappers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import jax
 import jax.numpy as jnp
 import chex
 import numpy as np
 from flax import struct
 from functools import partial
 from typing import Optional, Tuple, Union, Any
-from gymnax.environments import environment, spaces
 
 
 class GymnaxWrapper(object):
     """Base class for Gymnax wrappers."""
 
     def __init__(self, env):
         self._env = env
@@ -18,26 +17,24 @@
     def __getattr__(self, name):
         return getattr(self._env, name)
 
 
 class BatchEnvWrapper(GymnaxWrapper):
     """Batches reset and step functions"""
 
-    def __init__(self, env: environment.Environment, num_envs: int):
+    def __init__(self, env, num_envs: int):
         super().__init__(env)
 
         self.num_envs = num_envs
 
         self.reset_fn = jax.vmap(self._env.reset, in_axes=(0, None))
         self.step_fn = jax.vmap(self._env.step, in_axes=(0, 0, 0, None))
 
     @partial(jax.jit, static_argnums=(0, 2))
-    def reset(
-        self, rng, params: Optional[environment.EnvParams] = None
-    ) -> Tuple[chex.Array, environment.EnvState]:
+    def reset(self, rng, params=None):
         rng, _rng = jax.random.split(rng)
         rngs = jax.random.split(_rng, self.num_envs)
         obs, env_state = self.reset_fn(rngs, params)
         return obs, env_state
 
     @partial(jax.jit, static_argnums=(0, 4))
     def step(self, rng, state, action, params=None):
@@ -47,21 +44,19 @@
 
         return obs, state, reward, done, info
 
 
 class AutoResetEnvWrapper(GymnaxWrapper):
     """Provides standard auto-reset functionality, providing the same behaviour as Gymnax-default."""
 
-    def __init__(self, env: environment.Environment):
+    def __init__(self, env):
         super().__init__(env)
 
     @partial(jax.jit, static_argnums=(0, 2))
-    def reset(
-        self, key, params: Optional[environment.EnvParams] = None
-    ) -> Tuple[chex.Array, environment.EnvState]:
+    def reset(self, key, params=None):
         return self._env.reset(key, params)
 
     @partial(jax.jit, static_argnums=(0, 4))
     def step(self, rng, state, action, params=None):
 
         rng, _rng = jax.random.split(rng)
         obs_st, state_st, reward, done, info = self._env.step(
@@ -89,31 +84,29 @@
     """
     Provides efficient 'optimistic' resets.
     The wrapper also necessarily handles the batching of environment steps and resetting.
     reset_ratio: the number of environment workers per environment reset.  Higher means more efficient but a higher
     chance of duplicate resets.
     """
 
-    def __init__(self, env: environment.Environment, num_envs: int, reset_ratio: int):
+    def __init__(self, env, num_envs: int, reset_ratio: int):
         super().__init__(env)
 
         self.num_envs = num_envs
         self.reset_ratio = reset_ratio
         assert (
             num_envs % reset_ratio == 0
         ), "Reset ratio must perfectly divide num envs."
         self.num_resets = self.num_envs // reset_ratio
 
         self.reset_fn = jax.vmap(self._env.reset, in_axes=(0, None))
         self.step_fn = jax.vmap(self._env.step, in_axes=(0, 0, 0, None))
 
     @partial(jax.jit, static_argnums=(0, 2))
-    def reset(
-        self, rng, params: Optional[environment.EnvParams] = None
-    ) -> Tuple[chex.Array, environment.EnvState]:
+    def reset(self, rng, params=None):
         rng, _rng = jax.random.split(rng)
         rngs = jax.random.split(_rng, self.num_envs)
         obs, env_state = self.reset_fn(rngs, params)
         return obs, env_state
 
     @partial(jax.jit, static_argnums=(0, 4))
     def step(self, rng, state, action, params=None):
@@ -132,15 +125,15 @@
         being_reset = jax.random.choice(
             _rng,
             jnp.arange(self.num_envs),
             shape=(self.num_resets,),
             p=done,
             replace=False,
         )
-        reset_indexes.at[being_reset].set(jnp.arange(self.num_resets))
+        reset_indexes = reset_indexes.at[being_reset].set(jnp.arange(self.num_resets))
 
         obs_re = obs_re[reset_indexes]
         state_re = jax.tree_map(lambda x: x[reset_indexes], state_re)
 
         # Auto-reset environment based on termination
         def auto_reset(done, state_re, state_st, obs_re, obs_st):
             state = jax.tree_map(
@@ -153,44 +146,42 @@
         state, obs = jax.vmap(auto_reset)(done, state_re, state_st, obs_re, obs_st)
 
         return obs, state, reward, done, info
 
 
 @struct.dataclass
 class LogEnvState:
-    env_state: environment.EnvState
+    env_state: Any
     episode_returns: float
     episode_lengths: int
     returned_episode_returns: float
     returned_episode_lengths: int
     timestep: int
 
 
 class LogWrapper(GymnaxWrapper):
     """Log the episode returns and lengths."""
 
-    def __init__(self, env: environment.Environment):
+    def __init__(self, env):
         super().__init__(env)
 
     @partial(jax.jit, static_argnums=(0, 2))
-    def reset(
-        self, key: chex.PRNGKey, params: Optional[environment.EnvParams] = None
-    ) -> Tuple[chex.Array, environment.EnvState]:
+    def reset(self, key: chex.PRNGKey, params=None):
         obs, env_state = self._env.reset(key, params)
         state = LogEnvState(env_state, 0.0, 0, 0.0, 0, 0)
         return obs, state
 
     @partial(jax.jit, static_argnums=(0, 4))
     def step(
         self,
         key: chex.PRNGKey,
-        state: environment.EnvState,
+        state,
         action: Union[int, float],
-        params: Optional[environment.EnvParams] = None,
-    ) -> Tuple[chex.Array, environment.EnvState, float, bool, dict]:
+        params=None,
+    ):
         obs, env_state, reward, done, info = self._env.step(
             key, state.env_state, action, params
         )
         new_episode_return = state.episode_returns + reward
         new_episode_length = state.episode_lengths + 1
         state = LogEnvState(
             env_state=env_state,
```

### Comparing `craftax-1.3.0/craftax.egg-info/PKG-INFO` & `craftax-1.4.0/craftax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craftax
-Version: 1.3.0
+Version: 1.4.0
 Summary: An open-world environment for training RL agents
 Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
 Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
 Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.3.0-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.0-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -67,15 +67,15 @@
 Craftax conforms to the gymnax interface:
 ```python
 rng = jax.random.PRNGKey(0)
 rng, _rng = jax.random.split(rng)
 rngs = jax.random.split(_rng, 3)
 
 # Create environment
-env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
+env = make_craftax_env_from_name("Craftax-Symbolic-v1", auto_reset=True)
 env_params = env.default_params
 
 # Get an initial state and observation
 obs, state = env.reset(rngs[0], env_params)
 
 # Pick random action
 action = env.action_space(env_params).sample(rngs[1])
@@ -121,19 +121,22 @@
 Since Craftax runs entirely in JAX, it will take some time to compile the rendering and step functions - it might take around 30s to render the first frame and then another 20s to take the first action.  After this it should be very quick.  A tutorial for how to beat the game is present in `tutorial.md`.  The controls are printed out at the beginning of play.
 
 # 📈 Experiment
 To run experiments see the [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) repository.
 
 # 🔪 Gotchas
 ### Optimistic Resets
-Craftax provides the option to use optimistic resets to improve performance, which means that (unlike regular gymnax environments) it **does not auto-reset** by default.
-This means that the environment should always be wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).  See `ppo.py` for correct usage of both wrappers.
+Craftax provides the option to use optimistic resets to improve performance, which means that we provide access to environments that **do not auto-reset**.
+Environments obtained from `make_craftax_env_from_name` or `make_craftax_env_from_args` with `auto_reset=False` will not automatically reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in `OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour).
+See `ppo.py` in [Craftax Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct usage.
+Using `auto_reset=True` will return a regular auto-reset environment, which can be treated like any other gymnax environment.
 
 ### Texture Caching
-We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch.
+We use a texture cache to avoid recreating the texture atlas every time Craftax is imported. If you are just running Craftax as a benchmark this will not affect you.  However, if you are editing the game (e.g. adding new blocks, entities etc.) then a stale cache could cause errors. You can export the following environment variable to force textures to be created from scratch every run.
 ```
 export CRAFTAX_RELOAD_TEXTURES=true
 ```
 
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.3.0 Summary: An open-world
+Metadata-Version: 2.1 Name: craftax Version: 1.4.0 Summary: An open-world
 environment for training RL agents Author-email: Michael Matthews
 eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
 Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
@@ -10,15 +10,15 @@
 pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
 checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
 Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._3_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._0_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -28,23 +28,23 @@
 Craftax/main/images/dungeon_crawling.gif]
 [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
 farming.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/
 images/magic.gif][https://raw.githubusercontent.com/MichaelTMatthews/Craftax/
 main/images/mining.gif]
 # ð Basic Usage Craftax conforms to the gymnax interface: ```python rng =
 jax.random.PRNGKey(0) rng, _rng = jax.random.split(rng) rngs = jax.random.split
-(_rng, 3) # Create environment env = AutoResetEnvWrapper(CraftaxSymbolicEnv())
-env_params = env.default_params # Get an initial state and observation obs,
-state = env.reset(rngs[0], env_params) # Pick random action action =
-env.action_space(env_params).sample(rngs[1]) # Step environment obs, state,
-reward, done, info = env.step(rngs[2], state, action, env_params) ``` # â¬ï¸
-Installation The latest Craftax release can be installed from PyPi: ``` pip
-install craftax ``` If you want the most recent commit instead use: ``` pip
-install git+https://github.com/MichaelTMatthews/Craftax.git@main ``` ##
-Extending Craftax If you want to extend Craftax, run (make sure you have
+(_rng, 3) # Create environment env = make_craftax_env_from_name("Craftax-
+Symbolic-v1", auto_reset=True) env_params = env.default_params # Get an initial
+state and observation obs, state = env.reset(rngs[0], env_params) # Pick random
+action action = env.action_space(env_params).sample(rngs[1]) # Step environment
+obs, state, reward, done, info = env.step(rngs[2], state, action, env_params)
+``` # â¬ï¸ Installation The latest Craftax release can be installed from
+PyPi: ``` pip install craftax ``` If you want the most recent commit instead
+use: ``` pip install git+https://github.com/MichaelTMatthews/Craftax.git@main
+``` ## Extending Craftax If you want to extend Craftax, run (make sure you have
 `pip>=23.0`): ``` git clone https://github.com/MichaelTMatthews/Craftax.git cd
 Craftax pip install --editable . ``` ## GPU-Enabled JAX By default, both of the
 above methods will install JAX on the CPU. If you want to run JAX on a GPU/TPU,
 you'll need to install the correct wheel for your system from _J_A_X. For NVIDIA
 GPU the command is: ``` pip install -U "jax[cuda12_pip]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` # ð® Play To
 play Craftax run: ``` play_craftax ``` or to play Craftax-Classic run: ```
@@ -52,27 +52,32 @@
 time to compile the rendering and step functions - it might take around 30s to
 render the first frame and then another 20s to take the first action. After
 this it should be very quick. A tutorial for how to beat the game is present in
 `tutorial.md`. The controls are printed out at the beginning of play. # ð
 Experiment To run experiments see the [Craftax Baselines](https://github.com/
 MichaelTMatthews/Craftax_Baselines) repository. # ðª Gotchas ### Optimistic
 Resets Craftax provides the option to use optimistic resets to improve
-performance, which means that (unlike regular gymnax environments) it **does
-not auto-reset** by default. This means that the environment should always be
-wrapped either in `OptimisticResetVecEnvWrapper` (for efficient resets) or
-`AutoResetEnvWrapper` (to recover the default gymnax auto-reset behaviour). See
-`ppo.py` for correct usage of both wrappers. ### Texture Caching We use a
-texture cache to avoid recreating the texture atlas every time Craftax is
+performance, which means that we provide access to environments that **do not
+auto-reset**. Environments obtained from `make_craftax_env_from_name` or
+`make_craftax_env_from_args` with `auto_reset=False` will not automatically
+reset and if not properly handled will continue episodes into invalid states.
+These environments should always be wrapped either in
+`OptimisticResetVecEnvWrapper`(for efficient resets) or `AutoResetEnvWrapper`
+(to recover the default gymnax auto-reset behaviour). See `ppo.py` in [Craftax
+Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines) for correct
+usage. Using `auto_reset=True` will return a regular auto-reset environment,
+which can be treated like any other gymnax environment. ### Texture Caching We
+use a texture cache to avoid recreating the texture atlas every time Craftax is
 imported. If you are just running Craftax as a benchmark this will not affect
 you. However, if you are editing the game (e.g. adding new blocks, entities
 etc.) then a stale cache could cause errors. You can export the following
-environment variable to force textures to be created from scratch. ``` export
-CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like to add an
-algorithm please open a PR and provide a reference to the source of the
-results. We report reward as a % of the maximum (226). ## Craftax-1B |
+environment variable to force textures to be created from scratch every run.
+``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
+to add an algorithm please open a PR and provide a reference to the source of
+the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Source | |:----------|---------------:|:----------
 ---------------------------------------------------------------:| | PPO-RNN |
 15.3 | _P_u_r_e_J_a_x_R_L | | PPO | 11.9 | _P_u_r_e_J_a_x_R_L | | ICM | 11.9 | _I_C_M | | E3B | 11.0
 | _E_3_B | ## Craftax-1M | Algorithm | Reward (% max) | Source | |:----------|----
 -----------:|:-----------------------------------------------------------------
 --------:| | PPO-RNN | 2.3 | _P_u_r_e_J_a_x_R_L | | PPO | 2.2 | _P_u_r_e_J_a_x_R_L | | ICM | 2.2
 | _I_C_M | | E3B | 2.2 | _E_3_B | # ð See Also - âï¸ [Crafter](https://
```

### Comparing `craftax-1.3.0/craftax.egg-info/SOURCES.txt` & `craftax-1.4.0/craftax.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+craftax/__init__.py
+craftax/craftax_env.py
 craftax.egg-info/PKG-INFO
 craftax.egg-info/SOURCES.txt
 craftax.egg-info/dependency_links.txt
 craftax.egg-info/entry_points.txt
 craftax.egg-info/requires.txt
 craftax.egg-info/top_level.txt
 craftax/craftax/__init__.py
@@ -155,15 +157,14 @@
 craftax/craftax/assets/water.png
 craftax/craftax/assets/wood.png
 craftax/craftax/assets/wood_pickaxe.png
 craftax/craftax/assets/wood_sword.png
 craftax/craftax/assets/xp.png
 craftax/craftax/assets/zombie.png
 craftax/craftax/envs/__init__.py
-craftax/craftax/envs/common.py
 craftax/craftax/envs/craftax_pixels_env.py
 craftax/craftax/envs/craftax_symbolic_env.py
 craftax/craftax/util/__init__.py
 craftax/craftax/util/game_logic_utils.py
 craftax/craftax/util/maths_utils.py
 craftax/craftax/util/noise.py
 craftax/craftax/world_gen/__init__.py
@@ -223,14 +224,15 @@
 craftax/craftax_classic/assets/sand.png
 craftax/craftax_classic/assets/sapling.png
 craftax/craftax_classic/assets/skeleton.png
 craftax/craftax_classic/assets/stone.png
 craftax/craftax_classic/assets/stone_pickaxe.png
 craftax/craftax_classic/assets/stone_sword.png
 craftax/craftax_classic/assets/table.png
+craftax/craftax_classic/assets/texture_cache_classic.pbz2
 craftax/craftax_classic/assets/tree.png
 craftax/craftax_classic/assets/unknown.png
 craftax/craftax_classic/assets/water.png
 craftax/craftax_classic/assets/wood.png
 craftax/craftax_classic/assets/wood_pickaxe.png
 craftax/craftax_classic/assets/wood_sword.png
 craftax/craftax_classic/assets/zombie.png
@@ -238,10 +240,10 @@
 craftax/craftax_classic/envs/common.py
 craftax/craftax_classic/envs/craftax_pixels_env.py
 craftax/craftax_classic/envs/craftax_state.py
 craftax/craftax_classic/envs/craftax_symbolic_env.py
 craftax/craftax_classic/util/__init__.py
 craftax/craftax_classic/util/noise.py
 craftax/environment_base/__init__.py
-craftax/environment_base/environment_no_auto_reset.py
+craftax/environment_base/environment_bases.py
 craftax/environment_base/util.py
 craftax/environment_base/wrappers.py
```

### Comparing `craftax-1.3.0/pyproject.toml` & `craftax-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "craftax"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
   { name="Michael Matthews", email="michael.matthews@eng.ox.ac.uk" },
 ]
 description = "An open-world environment for training RL agents"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -32,15 +32,15 @@
     "chex",
     "matplotlib",
     "imageio",
 ]
 
 [project.scripts]
 play_craftax = "craftax.craftax.play_craftax:entry_point"
-play_craftax_classic = "craftax.craftax_classic.play_craftax_classic:main"
+play_craftax_classic = "craftax.craftax_classic.play_craftax_classic:entry_point"
 
 [project.urls]
 Homepage = "https://github.com/MichaelTMatthews/Craftax"
 Issues = "https://github.com/MichaelTMatthews/Craftax/issues"
 
 [tool.setuptools.packages.find]
 include=["craftax*"]
```

