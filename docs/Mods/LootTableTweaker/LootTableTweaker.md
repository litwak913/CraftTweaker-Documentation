# LootTableTweaker

[LootTableTweaker](https://minecraft.curseforge.com/projects/loottabletweaker) 添加了一些简单的函数来对战利品表进行修改。

## 删除战利品

删除一个的战利品表和它的所有战利品条目。
```java
// mods.ltt.LootTable.removeTable(String table);
mods.ltt.LootTable.removeTable("minecraft:chests/simple_dungeon");
```

删除一个战利品表的随机池。
```java
// mods.ltt.LootTable.removePool(String table, String pool);
mods.ltt.LootTable.removePool("minecraft:chests/simple_dungeon", "main");
```

删除一个战利品表随机池的一个战利品条目。
```java
// mods.ltt.LootTable.removeEntry(String table, String pool, String entry);
mods.ltt.LootTable.removeEntry("minecraft:chests/simple_dungeon", "main", "minecraft:iron_horse_armor");
```

删除一个战利品表随机池中的某个特定物品。
```java
//mods.ltt.LootTable.removeItem(String table, String pool, String entry);
mods.ltt.LootTable.removeItem("minecraft:chests/simple_dungeon", "main", "minecraft:golden_apple");
```

删除所有某个 mod 添加的战利品条目。
```java
// mods.ltt.LootTable.removeModEntry(String modid);
mods.ltt.LootTable.removeModEntry("modid");
```

删除所有包含某 mod 添加物品的战利品条目。
Removes all entries containing items added by the mod.
```java
// mods.ltt.LootTable.removeModItem(String modid);
mods.ltt.LootTable.removeModItem("modid");
```

删除所有某 mod 添加的战利品表。
```java
// mods.ltt.LootTable.removeModTable(String modid);
mods.ltt.LootTable.removeModTable("modid");
```

从所有战利品表中删除某物品。
```java
// mods.ltt.LootTable.removeGlobalItem(String itemId);
mods.ltt.LootTable.removeGlobalItem("minecraft:iron_ingot");
```
