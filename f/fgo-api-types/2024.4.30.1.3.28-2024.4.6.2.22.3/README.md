# Comparing `tmp/fgo_api_types-2024.4.30.1.3.28.tar.gz` & `tmp/fgo_api_types-2024.4.6.2.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.4.30.1.3.28.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.4.6.2.22.3.tar", max compression
```

## Comparing `fgo_api_types-2024.4.30.1.3.28.tar` & `fgo_api_types-2024.4.6.2.22.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-04-30 01:03:11.365220 fgo_api_types-2024.4.30.1.3.28/LICENSE
--rw-r--r--   0        0        0      449 2024-04-30 01:03:11.365220 fgo_api_types-2024.4.30.1.3.28/README.md
--rw-r--r--   0        0        0        0 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/base.py
--rw-r--r--   0        0        0     4511 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3843 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/common.py
--rw-r--r--   0        0        0    41932 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/enums.py
--rw-r--r--   0        0        0   183237 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    86686 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/nice.py
--rw-r--r--   0        0        0    59461 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19445 2024-04-30 01:03:28.829284 fgo_api_types-2024.4.30.1.3.28/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-04-30 01:03:29.149285 fgo_api_types-2024.4.30.1.3.28/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.30.1.3.28/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/LICENSE
+-rw-r--r--   0        0        0      449 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4368 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3762 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py
+-rw-r--r--   0        0        0    40655 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   176026 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    85618 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59051 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19285 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-04-06 02:22:03.705703 fgo_api_types-2024.4.6.2.22.3/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.6.2.22.3/PKG-INFO
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/LICENSE` & `fgo_api_types-2024.4.6.2.22.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/basic.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from decimal import Decimal
-from typing import Any, Optional, Sequence
+from typing import Optional, Sequence
 
 from pydantic import Field, HttpUrl
 
 from .base import BaseModelORJson
 from .common import BasicCostume, BuffScript, MCAssets, NiceTrait
 from .enums import Attribute, FuncApplyTarget, SvtClass
 from .gameenums import (
@@ -22,36 +22,31 @@
 )
 
 
 class BasicBuff(BaseModelORJson):
     id: int
     name: str
     originalName: str
-    detail: str
     icon: HttpUrl
     type: NiceBuffType
-    buffGroup: int
     script: BuffScript
-    originalScript: dict[str, Any]
     vals: list[NiceTrait]
     tvals: list[NiceTrait]
     ckSelfIndv: list[NiceTrait]
     ckOpIndv: list[NiceTrait]
-    maxRate: int
 
 
 class BasicFunction(BaseModelORJson):
     funcId: int
     funcType: NiceFuncType
     funcTargetType: NiceFuncTargetType
     funcTargetTeam: FuncApplyTarget
     functvals: list[NiceTrait]
     overWriteTvalsList: list[list[NiceTrait]]
     funcquestTvals: list[NiceTrait]
-    funcPopupText: str
     traitVals: list[NiceTrait] = []
     buffs: Sequence[BasicBuff]
 
 
 class BasicSkill(BaseModelORJson):
     id: int
     name: str
@@ -74,15 +69,14 @@
     originalOverwriteName: str | None = None
     type: NiceSvtType
     flag: NiceSvtFlag
     flags: list[NiceSvtFlagOriginal]
     classId: int
     className: SvtClass | str
     attribute: Attribute
-    traits: list[NiceTrait]
     rarity: int
     atkMax: int
     hpMax: int
     face: HttpUrl
     costume: dict[int, BasicCostume] = Field(
         ...,
         title="Costume Details",
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/common.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,14 @@
     Due to a limitation in Pydantic and OpenAPI schema generation, `dict[str, Any]`
     is used in place of either BasicBuff or NiceBuff
     """
 
     targetLimit: NiceBuffConvertLimitType
     convertType: NiceBuffConvertType
     targets: list[int] | list[NiceTrait] | list[dict[str, Any]]
-    targetBuffs: list[dict[str, Any]]
-    targetIndividualities: list[NiceTrait]
     convertBuffs: list[dict[str, Any]]
     script: BuffConvertScript
     effectId: int
 
 
 class BuffScript(BaseModel):
     checkIndvType: Optional[int] = None
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/enums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,17 +356,14 @@
     salemAbby = "salemAbby"
     uOlgaMarie = "uOlgaMarie"
     uOlgaMarieAlienGod = "uOlgaMarieAlienGod"
     beast = "beast"
     beastVI = "beastVI"
     beastVIBoss = "beastVIBoss"
     uOlgaMarieFlare = "uOlgaMarieFlare"
-    uOlgaMarieAqua = "uOlgaMarieAqua"
-    uOlgaMarieFlareCollection = "uOlgaMarieFlareCollection"
-    uOlgaMarieAquaCollection = "uOlgaMarieAquaCollection"
     atlasUnmappedClass = "atlasUnmappedClass"
     # OTHER = "OTHER"
     ALL = "ALL"
     # EXTRA = "EXTRA"
     # MIX = "MIX"
 
 
@@ -403,31 +400,28 @@
     30: SvtClass.beastILost,
     31: SvtClass.uOlgaMarieAlienGod,
     32: SvtClass.uOlgaMarie,
     33: SvtClass.beast,
     34: SvtClass.beastVI,
     35: SvtClass.beastVIBoss,
     36: SvtClass.uOlgaMarieFlare,
-    37: SvtClass.uOlgaMarieAqua,
     97: SvtClass.unknown,
     # 98
     # 99
     # 100
     107: SvtClass.agarthaPenth,
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
     # 1000: SvtClass.OTHER,
     # For Support List
     1001: SvtClass.ALL,
     # 1002: SvtClass.EXTRA,
     # 1003: SvtClass.MIX,
     # 1004: SvtClass.EXTRA1,
     # 1005: SvtClass.EXTRA2,
-    9001: SvtClass.uOlgaMarieFlareCollection,
-    9002: SvtClass.uOlgaMarieAquaCollection,
 }
 
 
 def get_class_name(class_id: int) -> SvtClass | str:
     if class_id in CLASS_NAME:
         return CLASS_NAME[class_id]
     else:
@@ -1005,27 +999,14 @@
     groupServant = "groupServant"
     takeruDummyTrait = "takeruDummyTrait"
     artsBuff = "artsBuff"
     busterBuff = "busterBuff"
     quickBuff = "quickBuff"
     FSNServant = "FSNServant"
     fieldDarkness = "fieldDarkness"
-    magicBullet = "magicBullet"
-    protagonistCorrection = "protagonistCorrection"
-    normalAokoBuff = "normalAokoBuff"
-    magicBulletAtkBuff = "magicBulletAtkBuff"
-    demeritFunction = "demeritFunction"
-    extraBuff = "extraBuff"
-    robinCounter = "robinCounter"
-    kuonjiAliceFormA = "kuonjiAliceFormA"
-    kuonjiAliceFormB = "kuonjiAliceFormB"
-    instantDeathFunction = "instantDeathFunction"
-    forceInstantDeathFunction = "forceInstantDeathFunction"
-    buffGutsOnInstantDeath = "buffGutsOnInstantDeath"
-    robinAllGone = "robinAllGone"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -1212,23 +1193,14 @@
     2876: Trait.caitCuCerpriestessAscension3To4,
     2878: Trait.fieldAir,
     2879: Trait.caitCuCerpriestessOnTheField,
     2880: Trait.elementalsWrath,
     2881: Trait.groupServant,
     2883: Trait.FSNServant,
     2884: Trait.fieldDarkness,
-    2885: Trait.magicBullet,
-    2886: Trait.robinCounter,
-    2887: Trait.robinAllGone,
-    2888: Trait.protagonistCorrection,
-    2903: Trait.kuonjiAliceFormB,
-    2911: Trait.normalAokoBuff,
-    2912: Trait.magicBulletAtkBuff,
-    2913: Trait.kuonjiAliceFormA,
-    2914: Trait.buffGutsOnInstantDeath,
     # 2xxx: CQ or Story quests buff
     3000: Trait.attackPhysical,  # Normal attack, including NP
     3001: Trait.attackProjectile,
     3002: Trait.attackMagical,
     3004: Trait.buffPositiveEffect,
     3005: Trait.buffNegativeEffect,  # mutually exclusive with 3004
     3006: Trait.buffIncreaseDamage,  # catch all damage: atk, np, powermod, ...
@@ -1300,18 +1272,14 @@
     3088: Trait.marking,
     3089: Trait.burnEffectivenessUp,
     3090: Trait.buffBuffSuccessRateUp,
     3091: Trait.takeruDummyTrait,
     3092: Trait.artsBuff,
     3093: Trait.busterBuff,
     3094: Trait.quickBuff,
-    3096: Trait.instantDeathFunction,
-    3097: Trait.forceInstantDeathFunction,
-    3098: Trait.demeritFunction,
-    3100: Trait.extraBuff,
     # 6016: No detail
     # 6021: No detail
     # 6022: No detail
     # 10xxx: CCC Kiara buff
     4001: Trait.cardArts,
     4002: Trait.cardBuster,
     4003: Trait.cardQuick,
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/gameenums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,18 +258,14 @@
     SUB_FIELD_BUFF = 131
     EVENT_FORTIFICATION_POINT_UP = 132
     GAIN_NP_INDIVIDUAL_SUM = 133
     SET_QUEST_ROUTE_FLAG = 134
     LAST_USE_PLAYER_SKILL_COPY = 135
     CHANGE_ENEMY_MASTER_FACE = 136
     DAMAGE_VALUE_SAFE_ONCE = 137
-    ADD_BATTLE_VALUE = 138
-    SET_BATTLE_VALUE = 139
-    GAIN_MULTIPLY_NP = 140
-    LOSS_MULTIPLY_NP = 141
 
 
 class NiceFuncType(StrEnum):
     """Function Type Enum"""
 
     none = "none"
     addState = "addState"
@@ -368,18 +364,14 @@
     subFieldBuff = "subFieldBuff"
     eventFortificationPointUp = "eventFortificationPointUp"
     gainNpIndividualSum = "gainNpIndividualSum"
     setQuestRouteFlag = "setQuestRouteFlag"
     lastUsePlayerSkillCopy = "lastUsePlayerSkillCopy"
     changeEnemyMasterFace = "changeEnemyMasterFace"
     damageValueSafeOnce = "damageValueSafeOnce"
-    addBattleValue = "addBattleValue"
-    setBattleValue = "setBattleValue"
-    gainMultiplyNp = "gainMultiplyNp"
-    lossMultiplyNp = "lossMultiplyNp"
 
 
 FUNC_TYPE_NAME: dict[int, NiceFuncType] = {
     0: NiceFuncType.none,
     1: NiceFuncType.addState,
     2: NiceFuncType.subState,
     3: NiceFuncType.damage,
@@ -476,18 +468,14 @@
     131: NiceFuncType.subFieldBuff,
     132: NiceFuncType.eventFortificationPointUp,
     133: NiceFuncType.gainNpIndividualSum,
     134: NiceFuncType.setQuestRouteFlag,
     135: NiceFuncType.lastUsePlayerSkillCopy,
     136: NiceFuncType.changeEnemyMasterFace,
     137: NiceFuncType.damageValueSafeOnce,
-    138: NiceFuncType.addBattleValue,
-    139: NiceFuncType.setBattleValue,
-    140: NiceFuncType.gainMultiplyNp,
-    141: NiceFuncType.lossMultiplyNp,
 }
 
 
 class FuncTargetType(IntEnum):
     SELF = 0
     PT_ONE = 1
     PT_ANOTHER = 2
@@ -663,15 +651,15 @@
     SUB_MAXHP = 82
     BATTLESTART_FUNCTION = 83
     WAVESTART_FUNCTION = 84
     SELFTURNEND_FUNCTION = 85
     DAMAGE_FUNCTION = 86
     UP_GIVEGAIN_HP = 87
     DOWN_GIVEGAIN_HP = 88
-    COMMANDATTACK_AFTER_FUNCTION = 89
+    COMMANDATTACK_FUNCTION = 89
     DEADATTACK_FUNCTION = 90
     UP_SPECIALDEFENCE = 91
     DOWN_SPECIALDEFENCE = 92
     UP_DAMAGEDROPNP = 93
     DOWN_DAMAGEDROPNP = 94
     ENTRY_FUNCTION = 95
     UP_CHAGETD = 96
@@ -702,25 +690,25 @@
     PIERCE_DEFENCE = 121
     UP_GUTS_HP = 122
     DOWN_GUTS_HP = 123
     UP_FUNCGAIN_NP = 124
     DOWN_FUNCGAIN_NP = 125
     UP_FUNC_HP_REDUCE = 126
     DOWN_FUNC_HP_REDUCE = 127
-    UP_DEFENCE_COMMANDDAMAGE = 128
-    DOWN_DEFENCE_COMMANDDAMAGE = 129
+    UP_DEFENCECOMMAN_DAMAGE = 128
+    DOWN_DEFENCECOMMAN_DAMAGE = 129
     NPATTACK_PREV_BUFF = 130
     FIX_COMMANDCARD = 131
     DONOT_GAINNP = 132
     FIELD_INDIVIDUALITY = 133
     DONOT_ACT_COMMANDTYPE = 134
     UP_DAMAGE_EVENT_POINT = 135
     UP_DAMAGE_SPECIAL = 136
-    ATTACK_AFTER_FUNCTION = 137
-    COMMANDCODEATTACK_BEFORE_FUNCTION = 138
+    ATTACK_FUNCTION = 137
+    COMMANDCODEATTACK_FUNCTION = 138
     DONOT_NOBLE_COND_MISMATCH = 139
     DONOT_SELECT_COMMANDCARD = 140
     DONOT_REPLACE = 141
     SHORTEN_USER_EQUIP_SKILL = 142
     TD_TYPE_CHANGE = 143
     OVERWRITE_CLASS_RELATION = 144
     TD_TYPE_CHANGE_ARTS = 145
@@ -764,23 +752,14 @@
     WAR_BOARD_IGNORE_DEFEATPOINT = 184
     SKILL_AFTER_FUNCTION = 185
     TREASURE_DEVICE_AFTER_FUNCTION = 186
     SKILL_AFTER_FUNCTION_MAIN_ONLY = 187
     TREASURE_DEVICE_AFTER_FUNCTION_MAIN_ONLY = 188
     PREVENT_INVISIBLE_WHEN_INSTANT_DEATH = 189
     OVERWRITE_SUBATTRIBUTE = 190
-    AVOIDANCE_ATTACK_DEATH_DAMAGE = 191
-    AVOID_FUNCTION_EXECUTE_SELF = 192
-    PIERCE_SUBDAMAGE = 193
-    CONTINUE_FUNCTION = 194
-    ADD_SPECIALDAMAGE = 195
-    SUB_SPECIALDAMAGE = 196
-    ADD_FUNC_HP_REDUCE = 197
-    SUB_FUNC_HP_REDUCE = 198
-    CHANGE_BGM = 199
     TO_FIELD_CHANGE_FIELD = 10001
     TO_FIELD_AVOID_BUFF = 10002
     TO_FIELD_SUB_INDIVIDUALITY_FIELD = 10003
 
 
 class NiceBuffType(StrEnum):
     """Buff Type Enum"""
@@ -855,15 +834,15 @@
     subMaxhp = "subMaxhp"
     battlestartFunction = "battlestartFunction"
     wavestartFunction = "wavestartFunction"
     selfturnendFunction = "selfturnendFunction"
     damageFunction = "damageFunction"
     upGivegainHp = "upGivegainHp"
     downGivegainHp = "downGivegainHp"
-    commandattackAfterFunction = "commandattackAfterFunction"
+    commandattackFunction = "commandattackFunction"
     deadattackFunction = "deadattackFunction"
     upSpecialdefence = "upSpecialdefence"
     downSpecialdefence = "downSpecialdefence"
     upDamagedropnp = "upDamagedropnp"
     downDamagedropnp = "downDamagedropnp"
     entryFunction = "entryFunction"
     upChagetd = "upChagetd"
@@ -894,25 +873,25 @@
     pierceDefence = "pierceDefence"
     upGutsHp = "upGutsHp"
     downGutsHp = "downGutsHp"
     upFuncgainNp = "upFuncgainNp"
     downFuncgainNp = "downFuncgainNp"
     upFuncHpReduce = "upFuncHpReduce"
     downFuncHpReduce = "downFuncHpReduce"
-    upDefenceCommanddamage = "upDefenceCommanddamage"
-    downDefenceCommanddamage = "downDefenceCommanddamage"
+    upDefencecommanDamage = "upDefencecommanDamage"
+    downDefencecommanDamage = "downDefencecommanDamage"
     npattackPrevBuff = "npattackPrevBuff"
     fixCommandcard = "fixCommandcard"
     donotGainnp = "donotGainnp"
     fieldIndividuality = "fieldIndividuality"
     donotActCommandtype = "donotActCommandtype"
     upDamageEventPoint = "upDamageEventPoint"
     upDamageSpecial = "upDamageSpecial"
-    attackAfterFunction = "attackAfterFunction"
-    commandcodeattackBeforeFunction = "commandcodeattackBeforeFunction"
+    attackFunction = "attackFunction"
+    commandcodeattackFunction = "commandcodeattackFunction"
     donotNobleCondMismatch = "donotNobleCondMismatch"
     donotSelectCommandcard = "donotSelectCommandcard"
     donotReplace = "donotReplace"
     shortenUserEquipSkill = "shortenUserEquipSkill"
     tdTypeChange = "tdTypeChange"
     overwriteClassRelation = "overwriteClassRelation"
     tdTypeChangeArts = "tdTypeChangeArts"
@@ -956,23 +935,14 @@
     warBoardIgnoreDefeatpoint = "warBoardIgnoreDefeatpoint"
     skillAfterFunction = "skillAfterFunction"
     treasureDeviceAfterFunction = "treasureDeviceAfterFunction"
     skillAfterFunctionMainOnly = "skillAfterFunctionMainOnly"
     treasureDeviceAfterFunctionMainOnly = "treasureDeviceAfterFunctionMainOnly"
     preventInvisibleWhenInstantDeath = "preventInvisibleWhenInstantDeath"
     overwriteSubattribute = "overwriteSubattribute"
-    avoidanceAttackDeathDamage = "avoidanceAttackDeathDamage"
-    avoidFunctionExecuteSelf = "avoidFunctionExecuteSelf"
-    pierceSubdamage = "pierceSubdamage"
-    continueFunction = "continueFunction"
-    addSpecialdamage = "addSpecialdamage"
-    subSpecialdamage = "subSpecialdamage"
-    addFuncHpReduce = "addFuncHpReduce"
-    subFuncHpReduce = "subFuncHpReduce"
-    changeBgm = "changeBgm"
     toFieldChangeField = "toFieldChangeField"
     toFieldAvoidBuff = "toFieldAvoidBuff"
     toFieldSubIndividualityField = "toFieldSubIndividualityField"
 
 
 BUFF_TYPE_NAME: dict[int, NiceBuffType] = {
     0: NiceBuffType.none,
@@ -1045,15 +1015,15 @@
     82: NiceBuffType.subMaxhp,
     83: NiceBuffType.battlestartFunction,
     84: NiceBuffType.wavestartFunction,
     85: NiceBuffType.selfturnendFunction,
     86: NiceBuffType.damageFunction,
     87: NiceBuffType.upGivegainHp,
     88: NiceBuffType.downGivegainHp,
-    89: NiceBuffType.commandattackAfterFunction,
+    89: NiceBuffType.commandattackFunction,
     90: NiceBuffType.deadattackFunction,
     91: NiceBuffType.upSpecialdefence,
     92: NiceBuffType.downSpecialdefence,
     93: NiceBuffType.upDamagedropnp,
     94: NiceBuffType.downDamagedropnp,
     95: NiceBuffType.entryFunction,
     96: NiceBuffType.upChagetd,
@@ -1084,25 +1054,25 @@
     121: NiceBuffType.pierceDefence,
     122: NiceBuffType.upGutsHp,
     123: NiceBuffType.downGutsHp,
     124: NiceBuffType.upFuncgainNp,
     125: NiceBuffType.downFuncgainNp,
     126: NiceBuffType.upFuncHpReduce,
     127: NiceBuffType.downFuncHpReduce,
-    128: NiceBuffType.upDefenceCommanddamage,
-    129: NiceBuffType.downDefenceCommanddamage,
+    128: NiceBuffType.upDefencecommanDamage,
+    129: NiceBuffType.downDefencecommanDamage,
     130: NiceBuffType.npattackPrevBuff,
     131: NiceBuffType.fixCommandcard,
     132: NiceBuffType.donotGainnp,
     133: NiceBuffType.fieldIndividuality,
     134: NiceBuffType.donotActCommandtype,
     135: NiceBuffType.upDamageEventPoint,
     136: NiceBuffType.upDamageSpecial,
-    137: NiceBuffType.attackAfterFunction,
-    138: NiceBuffType.commandcodeattackBeforeFunction,
+    137: NiceBuffType.attackFunction,
+    138: NiceBuffType.commandcodeattackFunction,
     139: NiceBuffType.donotNobleCondMismatch,
     140: NiceBuffType.donotSelectCommandcard,
     141: NiceBuffType.donotReplace,
     142: NiceBuffType.shortenUserEquipSkill,
     143: NiceBuffType.tdTypeChange,
     144: NiceBuffType.overwriteClassRelation,
     145: NiceBuffType.tdTypeChangeArts,
@@ -1146,23 +1116,14 @@
     184: NiceBuffType.warBoardIgnoreDefeatpoint,
     185: NiceBuffType.skillAfterFunction,
     186: NiceBuffType.treasureDeviceAfterFunction,
     187: NiceBuffType.skillAfterFunctionMainOnly,
     188: NiceBuffType.treasureDeviceAfterFunctionMainOnly,
     189: NiceBuffType.preventInvisibleWhenInstantDeath,
     190: NiceBuffType.overwriteSubattribute,
-    191: NiceBuffType.avoidanceAttackDeathDamage,
-    192: NiceBuffType.avoidFunctionExecuteSelf,
-    193: NiceBuffType.pierceSubdamage,
-    194: NiceBuffType.continueFunction,
-    195: NiceBuffType.addSpecialdamage,
-    196: NiceBuffType.subSpecialdamage,
-    197: NiceBuffType.addFuncHpReduce,
-    198: NiceBuffType.subFuncHpReduce,
-    199: NiceBuffType.changeBgm,
     10001: NiceBuffType.toFieldChangeField,
     10002: NiceBuffType.toFieldAvoidBuff,
     10003: NiceBuffType.toFieldSubIndividualityField,
 }
 
 
 class BuffAction(IntEnum):
@@ -1219,15 +1180,15 @@
     REGAIN_NP_USED_NOBLE = 50
     FUNCTION_DEAD = 51
     MAXHP_RATE = 52
     MAXHP_VALUE = 53
     FUNCTION_WAVESTART = 54
     FUNCTION_SELFTURNEND = 55
     GIVE_GAIN_HP = 56
-    FUNCTION_COMMANDATTACK_AFTER = 57
+    FUNCTION_COMMANDATTACK = 57
     FUNCTION_DEADATTACK = 58
     FUNCTION_ENTRY = 59
     CHAGETD = 60
     GRANT_SUBSTATE = 61
     TOLERANCE_SUBSTATE = 62
     GRANT_INSTANTDEATH = 63
     FUNCTION_DAMAGE = 64
@@ -1242,16 +1203,16 @@
     FUNCTION_NPATTACK = 73
     FIX_COMMANDCARD = 74
     DONOT_GAINNP = 75
     FIELD_INDIVIDUALITY = 76
     DONOT_ACT_COMMANDTYPE = 77
     DAMAGE_EVENT_POINT = 78
     DAMAGE_SPECIAL = 79
-    FUNCTION_ATTACK_AFTER = 80
-    FUNCTION_COMMANDCODEATTACK_BEFORE = 81
+    FUNCTION_ATTACK = 80
+    FUNCTION_COMMANDCODEATTACK = 81
     DONOT_NOBLE_COND_MISMATCH = 82
     DONOT_SELECT_COMMANDCARD = 83
     DONOT_REPLACE = 84
     SHORTEN_USER_EQUIP_SKILL = 85
     TD_TYPE_CHANGE = 86
     OVERWRITE_CLASS_RELATION = 87
     FUNCTION_COMMANDATTACK_BEFORE = 88
@@ -1291,22 +1252,14 @@
     FUNCTION_SKILL_AFTER = 122
     FUNCTION_SKILL_AFTER_MAIN_ONLY = 123
     FUNCTION_TREASURE_DEVICE_AFTER = 124
     FUNCTION_TREASURE_DEVICE_AFTER_MAIN_ONLY = 125
     GUTS = 126
     PREVENT_INVISIBLE_WHEN_INSTANT_DEATH = 127
     OVERWRITE_SUBATTRIBUTE = 128
-    AVOIDANCE_ATTACK_DEATH_DAMAGE = 129
-    AVOID_FUNCTION_EXECUTE_SELF = 130
-    FUNCTION_CONTINUE = 131
-    PIERCE_SUBDAMAGE = 132
-    RECEIVE_DAMAGE_PIERCE = 133
-    SPECIAL_RECEIVE_DAMAGE = 134
-    FUNC_HP_REDUCE_VALUE = 135
-    CHANGE_BGM = 136
 
 
 class NiceBuffAction(StrEnum):
     """Buff Action Type Enum"""
 
     none = "none"
     commandAtk = "commandAtk"
@@ -1361,15 +1314,15 @@
     regainNpUsedNoble = "regainNpUsedNoble"
     functionDead = "functionDead"
     maxhpRate = "maxhpRate"
     maxhpValue = "maxhpValue"
     functionWavestart = "functionWavestart"
     functionSelfturnend = "functionSelfturnend"
     giveGainHp = "giveGainHp"
-    functionCommandattackAfter = "functionCommandattackAfter"
+    functionCommandattack = "functionCommandattack"
     functionDeadattack = "functionDeadattack"
     functionEntry = "functionEntry"
     chagetd = "chagetd"
     grantSubstate = "grantSubstate"
     toleranceSubstate = "toleranceSubstate"
     grantInstantdeath = "grantInstantdeath"
     functionDamage = "functionDamage"
@@ -1384,16 +1337,16 @@
     functionNpattack = "functionNpattack"
     fixCommandcard = "fixCommandcard"
     donotGainnp = "donotGainnp"
     fieldIndividuality = "fieldIndividuality"
     donotActCommandtype = "donotActCommandtype"
     damageEventPoint = "damageEventPoint"
     damageSpecial = "damageSpecial"
-    functionAttackAfter = "functionAttackAfter"
-    functionCommandcodeattackBefore = "functionCommandcodeattackBefore"
+    functionAttack = "functionAttack"
+    functionCommandcodeattack = "functionCommandcodeattack"
     donotNobleCondMismatch = "donotNobleCondMismatch"
     donotSelectCommandcard = "donotSelectCommandcard"
     donotReplace = "donotReplace"
     shortenUserEquipSkill = "shortenUserEquipSkill"
     tdTypeChange = "tdTypeChange"
     overwriteClassRelation = "overwriteClassRelation"
     functionCommandattackBefore = "functionCommandattackBefore"
@@ -1433,22 +1386,14 @@
     functionSkillAfter = "functionSkillAfter"
     functionSkillAfterMainOnly = "functionSkillAfterMainOnly"
     functionTreasureDeviceAfter = "functionTreasureDeviceAfter"
     functionTreasureDeviceAfterMainOnly = "functionTreasureDeviceAfterMainOnly"
     guts = "guts"
     preventInvisibleWhenInstantDeath = "preventInvisibleWhenInstantDeath"
     overwriteSubattribute = "overwriteSubattribute"
-    avoidanceAttackDeathDamage = "avoidanceAttackDeathDamage"
-    avoidFunctionExecuteSelf = "avoidFunctionExecuteSelf"
-    functionContinue = "functionContinue"
-    pierceSubdamage = "pierceSubdamage"
-    receiveDamagePierce = "receiveDamagePierce"
-    specialReceiveDamage = "specialReceiveDamage"
-    funcHpReduceValue = "funcHpReduceValue"
-    changeBgm = "changeBgm"
 
 
 BUFF_ACTION_NAME: dict[int, NiceBuffAction] = {
     0: NiceBuffAction.none,
     1: NiceBuffAction.commandAtk,
     2: NiceBuffAction.commandDef,
     3: NiceBuffAction.atk,
@@ -1501,15 +1446,15 @@
     50: NiceBuffAction.regainNpUsedNoble,
     51: NiceBuffAction.functionDead,
     52: NiceBuffAction.maxhpRate,
     53: NiceBuffAction.maxhpValue,
     54: NiceBuffAction.functionWavestart,
     55: NiceBuffAction.functionSelfturnend,
     56: NiceBuffAction.giveGainHp,
-    57: NiceBuffAction.functionCommandattackAfter,
+    57: NiceBuffAction.functionCommandattack,
     58: NiceBuffAction.functionDeadattack,
     59: NiceBuffAction.functionEntry,
     60: NiceBuffAction.chagetd,
     61: NiceBuffAction.grantSubstate,
     62: NiceBuffAction.toleranceSubstate,
     63: NiceBuffAction.grantInstantdeath,
     64: NiceBuffAction.functionDamage,
@@ -1524,16 +1469,16 @@
     73: NiceBuffAction.functionNpattack,
     74: NiceBuffAction.fixCommandcard,
     75: NiceBuffAction.donotGainnp,
     76: NiceBuffAction.fieldIndividuality,
     77: NiceBuffAction.donotActCommandtype,
     78: NiceBuffAction.damageEventPoint,
     79: NiceBuffAction.damageSpecial,
-    80: NiceBuffAction.functionAttackAfter,
-    81: NiceBuffAction.functionCommandcodeattackBefore,
+    80: NiceBuffAction.functionAttack,
+    81: NiceBuffAction.functionCommandcodeattack,
     82: NiceBuffAction.donotNobleCondMismatch,
     83: NiceBuffAction.donotSelectCommandcard,
     84: NiceBuffAction.donotReplace,
     85: NiceBuffAction.shortenUserEquipSkill,
     86: NiceBuffAction.tdTypeChange,
     87: NiceBuffAction.overwriteClassRelation,
     88: NiceBuffAction.functionCommandattackBefore,
@@ -1573,22 +1518,14 @@
     122: NiceBuffAction.functionSkillAfter,
     123: NiceBuffAction.functionSkillAfterMainOnly,
     124: NiceBuffAction.functionTreasureDeviceAfter,
     125: NiceBuffAction.functionTreasureDeviceAfterMainOnly,
     126: NiceBuffAction.guts,
     127: NiceBuffAction.preventInvisibleWhenInstantDeath,
     128: NiceBuffAction.overwriteSubattribute,
-    129: NiceBuffAction.avoidanceAttackDeathDamage,
-    130: NiceBuffAction.avoidFunctionExecuteSelf,
-    131: NiceBuffAction.functionContinue,
-    132: NiceBuffAction.pierceSubdamage,
-    133: NiceBuffAction.receiveDamagePierce,
-    134: NiceBuffAction.specialReceiveDamage,
-    135: NiceBuffAction.funcHpReduceValue,
-    136: NiceBuffAction.changeBgm,
 }
 
 
 class BuffLimit(IntEnum):
     NONE = 0
     UPPER = 1
     LOWER = 2
@@ -1709,78 +1646,64 @@
     CounterLv = 93
     CounterOc = 94
     UseTreasureDevice = 95
     SkillReaction = 96
     BehaveAsFamilyBuff = 97
     UnSubStateWhileLinkedToOthers = 98
     NotAccompanyWhenLinkedTargetMoveState = 99
-    NotTargetSkillIdArray = 100
-    ShortTurn = 101
-    FieldIndividuality = 102
-    BGId = 103
-    BGType = 104
-    BgmId = 105
-    TakeOverFieldState = 106
-    TakeOverNextWaveBGAndBGM = 107
-    RemoveFieldBuffActorDeath = 108
-    FieldBuffGrantType = 109
-    Priority = 110
-    AddIndividualityEx = 111
-    IgnoreResistance = 112
-    GainNpTargetPassiveIndividuality = 113
-    HpReduceToRegainIndiv = 114
-    DisplayActualRecoveryHpFlag = 115
-    ShiftDeckIndex = 116
-    PopValueText = 117
-    IsLossHpPerNow = 118
-    CopyTargetFunctionType = 119
-    CopyFunctionTargetPTOnly = 120
-    IgnoreValueUp = 121
-    ApplyValueUp = 122
-    ActNoDamageBuff = 123
-    ActSelectIndex = 124
-    CopyTargetBuffType = 125
-    NotSkillCopyTargetFuncIds = 126
-    NotSkillCopyTargetIndividualities = 127
-    ClassIconAuraEffectId = 128
-    ActMasterGenderType = 129
-    IntervalTurn = 130
-    IntervalCount = 131
-    TriggeredFieldCountTarget = 132
-    TriggeredFieldCountRange = 133
-    TargetEnemyRange = 134
-    TriggeredFuncPositionSameTarget = 135
-    TriggeredFuncPositionAll = 136
-    TriggeredTargetHpRange = 137
-    TriggeredTargetHpRateRange = 138
-    ExcludeUnSubStateIndiv = 139
-    ProgressTurnOnBoard = 140
-    CheckTargetResurrectable = 141
-    CancelTransform = 142
-    UnSubStateWhenContinue = 143
-    CheckTargetHaveDefeatPoint = 144
-    NPFixedDamageValue = 145
-    IgnoreShiftSafeDamage = 146
-    ActAttackFunction = 147
-    DelayRemoveBuffExpiredOnPlayerTurn = 148
-    AllowRemoveBuff = 149
-    NotExecFunctionIfKeepAliveOnWarBoard = 150
-    SnapShotParamAddSelfIndv = 151
-    SnapShotParamAddOpIndv = 152
-    SnapShotParamAddFieldIndv = 153
-    SnapShotParamAddValue = 154
-    SnapShotParamAddMaxValue = 155
-    SnapShotParamAddMaxCount = 156
-    NotExecOnTransform = 157
-    NotRemoveOnTransform = 158
-    PriorityBgm = 159
-    BgmAllowSubPlaying = 160
-    BgPriority = 161
-    PriorityBg = 162
-    ResetBgmPriorityAtWaveStart = 163
+    AllowSubBgmPlaying = 100
+    NotTargetSkillIdArray = 101
+    ShortTurn = 102
+    FieldIndividuality = 103
+    BGId = 104
+    BGType = 105
+    BgmId = 106
+    TakeOverFieldState = 107
+    TakeOverNextWaveBGAndBGM = 108
+    RemoveFieldBuffActorDeath = 109
+    FieldBuffGrantType = 110
+    Priority = 111
+    AddIndividualityEx = 112
+    IgnoreResistance = 113
+    GainNpTargetPassiveIndividuality = 114
+    HpReduceToRegainIndiv = 115
+    DisplayActualRecoveryHpFlag = 116
+    ShiftDeckIndex = 117
+    PopValueText = 118
+    IsLossHpPerNow = 119
+    CopyTargetFunctionType = 120
+    CopyFunctionTargetPTOnly = 121
+    IgnoreValueUp = 122
+    ApplyValueUp = 123
+    ActNoDamageBuff = 124
+    ActSelectIndex = 125
+    CopyTargetBuffType = 126
+    NotSkillCopyTargetFuncIds = 127
+    NotSkillCopyTargetIndividualities = 128
+    ClassIconAuraEffectId = 129
+    ActMasterGenderType = 130
+    IntervalTurn = 131
+    IntervalCount = 132
+    TriggeredFieldCountTarget = 133
+    TriggeredFieldCountRange = 134
+    TargetEnemyRange = 135
+    TriggeredFuncPositionSameTarget = 136
+    TriggeredFuncPositionAll = 137
+    TriggeredTargetHpRange = 138
+    TriggeredTargetHpRateRange = 139
+    ExcludeUnSubStateIndiv = 140
+    ProgressTurnOnBoard = 141
+    CheckTargetResurrectable = 142
+    CancelTransform = 143
+    UnSubStateWhenContinue = 144
+    CheckTargetHaveDefeatPoint = 145
+    NPFixedDamageValue = 146
+    IgnoreShiftSafeDamage = 147
+    ActAttackFunction = 148
+    DelayRemoveBuffExpiredOnPlayerTurn = 149
 
 
 class ClassRelationOverwriteType(IntEnum):
     OVERWRITE_FORCE = 0
     OVERWRITE_MORE_THAN_TARGET = 1
     OVERWRITE_LESS_THAN_TARGET = 2
 
@@ -1831,15 +1754,14 @@
     EUQIP_SKILL_USE_ITEM = 28
     SVT_COIN = 29
     FRIENDSHIP_UP_ITEM = 30
     PP = 31
     TRADE_AP = 32
     RI = 33
     STORMPOD = 34
-    BATTLE_ITEM = 35
 
 
 class NiceItemType(StrEnum):
     """Item Type Enum"""
 
     qp = "qp"
     stone = "stone"
@@ -1871,15 +1793,14 @@
     euqipSkillUseItem = "euqipSkillUseItem"
     svtCoin = "svtCoin"
     friendshipUpItem = "friendshipUpItem"
     pp = "pp"
     tradeAp = "tradeAp"
     ri = "ri"
     stormpod = "stormpod"
-    battleItem = "battleItem"
 
 
 ITEM_TYPE_NAME: dict[int, NiceItemType] = {
     1: NiceItemType.qp,
     2: NiceItemType.stone,
     3: NiceItemType.apRecover,
     4: NiceItemType.apAdd,
@@ -1909,15 +1830,14 @@
     28: NiceItemType.euqipSkillUseItem,
     29: NiceItemType.svtCoin,
     30: NiceItemType.friendshipUpItem,
     31: NiceItemType.pp,
     32: NiceItemType.tradeAp,
     33: NiceItemType.ri,
     34: NiceItemType.stormpod,
-    35: NiceItemType.battleItem,
 }
 
 
 class GiftType(IntEnum):
     SERVANT = 1
     ITEM = 2
     FRIENDSHIP = 3
@@ -1929,15 +1849,14 @@
     COSTUME_RELEASE = 9
     COSTUME_GET = 10
     COMMAND_CODE = 11
     EVENT_POINT_BUFF = 12
     EVENT_BOARD_GAME_TOKEN = 13
     EVENT_COMMAND_ASSIST = 14
     EVENT_HEEL_PORTRAIT = 15
-    BATTLE_ITEM = 16
 
 
 class NiceGiftType(StrEnum):
     """Gift Type Enum"""
 
     servant = "servant"
     item = "item"
@@ -1950,15 +1869,14 @@
     costumeRelease = "costumeRelease"
     costumeGet = "costumeGet"
     commandCode = "commandCode"
     eventPointBuff = "eventPointBuff"
     eventBoardGameToken = "eventBoardGameToken"
     eventCommandAssist = "eventCommandAssist"
     eventHeelPortrait = "eventHeelPortrait"
-    battleItem = "battleItem"
 
 
 GIFT_TYPE_NAME: dict[int, NiceGiftType] = {
     1: NiceGiftType.servant,
     2: NiceGiftType.item,
     3: NiceGiftType.friendship,
     4: NiceGiftType.userExp,
@@ -1969,15 +1887,14 @@
     9: NiceGiftType.costumeRelease,
     10: NiceGiftType.costumeGet,
     11: NiceGiftType.commandCode,
     12: NiceGiftType.eventPointBuff,
     13: NiceGiftType.eventBoardGameToken,
     14: NiceGiftType.eventCommandAssist,
     15: NiceGiftType.eventHeelPortrait,
-    16: NiceGiftType.battleItem,
 }
 
 
 class ShopType(IntEnum):
     NONE = 0
     EVENT_ITEM = 1
     MANA = 2
@@ -2420,17 +2337,14 @@
     PLAY_QUEST_PHASE = 209
     NOT_PLAY_QUEST_PHASE = 210
     EVENT_START_TO_END = 211
     COMMON_VALUE_ABOVE = 212
     COMMON_VALUE_BELOW = 213
     COMMON_VALUE_EQUAL = 214
     ELAPSED_TIME_AFTER_QUEST_CLEAR = 215
-    WITH_STARTING_MEMBER = 216
-    LATEST_QUEST_PHASE_EQUAL = 217
-    NOT_LATEST_QUEST_PHASE_EQUAL = 218
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
     questClear = "questClear"
@@ -2641,17 +2555,14 @@
     playQuestPhase = "playQuestPhase"
     notPlayQuestPhase = "notPlayQuestPhase"
     eventStartToEnd = "eventStartToEnd"
     commonValueAbove = "commonValueAbove"
     commonValueBelow = "commonValueBelow"
     commonValueEqual = "commonValueEqual"
     elapsedTimeAfterQuestClear = "elapsedTimeAfterQuestClear"
-    withStartingMember = "withStartingMember"
-    latestQuestPhaseEqual = "latestQuestPhaseEqual"
-    notLatestQuestPhaseEqual = "notLatestQuestPhaseEqual"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
     3: NiceCondType.useItemEternity,
@@ -2860,17 +2771,14 @@
     209: NiceCondType.playQuestPhase,
     210: NiceCondType.notPlayQuestPhase,
     211: NiceCondType.eventStartToEnd,
     212: NiceCondType.commonValueAbove,
     213: NiceCondType.commonValueBelow,
     214: NiceCondType.commonValueEqual,
     215: NiceCondType.elapsedTimeAfterQuestClear,
-    216: NiceCondType.withStartingMember,
-    217: NiceCondType.latestQuestPhaseEqual,
-    218: NiceCondType.notLatestQuestPhaseEqual,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
     FRIENDSHIP = 3
@@ -3911,28 +3819,14 @@
     COUNT_PLAYER_SKILL_EQUAL_INCLUDE_MASTER_SKILL = 190
     TOTAL_TURN_HIGHER = 191
     TOTAL_TURN_LOWER = 192
     TOTAL_TURN_EQUAL = 193
     CHECK_WAR_BOARD_SQUARE_INDIVIDUALITY = 194
     CHECK_PT_HIGHER_NPGAUGE = 195
     CHECK_SELF_HIGHER_NPGAUGE = 196
-    CHECK_BATTLE_VALUE_ABOVE = 197
-    CHECK_BATTLE_VALUE_EQUAL = 198
-    CHECK_BATTLE_VALUE_NOT_EQUAL = 199
-    CHECK_BATTLE_VALUE_BELOW = 200
-    CHECK_BATTLE_VALUE_BETWEEN = 201
-    CHECK_BATTLE_VALUE_NOT_BETWEEN = 202
-    CHECK_USE_MASTER_SKILL_INDEX = 203
-    CHECK_USE_MASTER_SKILL_INDEX_THIS_TURN = 204
-    COUNT_MASTER_SKILL_HIGHER_THIS_TURN = 205
-    COUNT_MASTER_SKILL_LOWER_THIS_TURN = 206
-    COUNT_MASTER_SKILL_EQUAL_THIS_TURN = 207
-    COUNT_MASTER_SKILL_HIGHER_THIS_WAVE = 208
-    COUNT_MASTER_SKILL_LOWER_THIS_WAVE = 209
-    COUNT_MASTER_SKILL_EQUAL_THIS_WAVE = 210
 
 
 class NiceAiCond(StrEnum):
     """AI Cond Enum"""
 
     none = "none"
     hpHigher = "hpHigher"
@@ -4103,28 +3997,14 @@
     countPlayerSkillEqualIncludeMasterSkill = "countPlayerSkillEqualIncludeMasterSkill"
     totalTurnHigher = "totalTurnHigher"
     totalTurnLower = "totalTurnLower"
     totalTurnEqual = "totalTurnEqual"
     checkWarBoardSquareIndividuality = "checkWarBoardSquareIndividuality"
     checkPtHigherNpgauge = "checkPtHigherNpgauge"
     checkSelfHigherNpgauge = "checkSelfHigherNpgauge"
-    checkBattleValueAbove = "checkBattleValueAbove"
-    checkBattleValueEqual = "checkBattleValueEqual"
-    checkBattleValueNotEqual = "checkBattleValueNotEqual"
-    checkBattleValueBelow = "checkBattleValueBelow"
-    checkBattleValueBetween = "checkBattleValueBetween"
-    checkBattleValueNotBetween = "checkBattleValueNotBetween"
-    checkUseMasterSkillIndex = "checkUseMasterSkillIndex"
-    checkUseMasterSkillIndexThisTurn = "checkUseMasterSkillIndexThisTurn"
-    countMasterSkillHigherThisTurn = "countMasterSkillHigherThisTurn"
-    countMasterSkillLowerThisTurn = "countMasterSkillLowerThisTurn"
-    countMasterSkillEqualThisTurn = "countMasterSkillEqualThisTurn"
-    countMasterSkillHigherThisWave = "countMasterSkillHigherThisWave"
-    countMasterSkillLowerThisWave = "countMasterSkillLowerThisWave"
-    countMasterSkillEqualThisWave = "countMasterSkillEqualThisWave"
 
 
 AI_COND_NAME: dict[int, NiceAiCond] = {
     0: NiceAiCond.none,
     10: NiceAiCond.hpHigher,
     11: NiceAiCond.hpLower,
     20: NiceAiCond.actcount,
@@ -4277,28 +4157,14 @@
     190: NiceAiCond.countPlayerSkillEqualIncludeMasterSkill,
     191: NiceAiCond.totalTurnHigher,
     192: NiceAiCond.totalTurnLower,
     193: NiceAiCond.totalTurnEqual,
     194: NiceAiCond.checkWarBoardSquareIndividuality,
     195: NiceAiCond.checkPtHigherNpgauge,
     196: NiceAiCond.checkSelfHigherNpgauge,
-    197: NiceAiCond.checkBattleValueAbove,
-    198: NiceAiCond.checkBattleValueEqual,
-    199: NiceAiCond.checkBattleValueNotEqual,
-    200: NiceAiCond.checkBattleValueBelow,
-    201: NiceAiCond.checkBattleValueBetween,
-    202: NiceAiCond.checkBattleValueNotBetween,
-    203: NiceAiCond.checkUseMasterSkillIndex,
-    204: NiceAiCond.checkUseMasterSkillIndexThisTurn,
-    205: NiceAiCond.countMasterSkillHigherThisTurn,
-    206: NiceAiCond.countMasterSkillLowerThisTurn,
-    207: NiceAiCond.countMasterSkillEqualThisTurn,
-    208: NiceAiCond.countMasterSkillHigherThisWave,
-    209: NiceAiCond.countMasterSkillLowerThisWave,
-    210: NiceAiCond.countMasterSkillEqualThisWave,
 }
 
 
 class AiActType(IntEnum):
     NONE = 0
     RANDOM = 1
     ATTACK = 2
@@ -4800,19 +4666,14 @@
     CHECK_TARGET_SKILL_THISTURN = 34
     CHECK_SELECT_CHAIN = 35
     COUNT_PLAYER_NP = 36
     COUNT_PLAYER_SKILL = 37
     COUNT_PLAYER_SKILL_INCLUDE_MASTER_SKILL = 38
     TOTAL_TURN = 39
     WAR_BOARD_SQUARE_INDIVIDUALITY = 40
-    CHECK_BATTLE_VALUE = 41
-    CHECK_PLAYER_MASTER_SKILL_INDEX = 42
-    CHECK_PLAYER_MASTER_SKILL_INDEX_THIS_TURN = 43
-    COUNT_PLAYER_MASTER_SKILL_THIS_TURN = 44
-    COUNT_PLAYER_MASTER_SKILL_THIS_WAVE = 45
 
 
 class NiceAiCondParameter(StrEnum):
     """Ai Condition Parameter"""
 
     none = "none"
     turn = "turn"
@@ -4851,19 +4712,14 @@
     checkTargetSkillThisturn = "checkTargetSkillThisturn"
     checkSelectChain = "checkSelectChain"
     countPlayerNp = "countPlayerNp"
     countPlayerSkill = "countPlayerSkill"
     countPlayerSkillIncludeMasterSkill = "countPlayerSkillIncludeMasterSkill"
     totalTurn = "totalTurn"
     warBoardSquareIndividuality = "warBoardSquareIndividuality"
-    checkBattleValue = "checkBattleValue"
-    checkPlayerMasterSkillIndex = "checkPlayerMasterSkillIndex"
-    checkPlayerMasterSkillIndexThisTurn = "checkPlayerMasterSkillIndexThisTurn"
-    countPlayerMasterSkillThisTurn = "countPlayerMasterSkillThisTurn"
-    countPlayerMasterSkillThisWave = "countPlayerMasterSkillThisWave"
 
 
 AI_COND_PARAMETER_NAME: dict[int, NiceAiCondParameter] = {
     0: NiceAiCondParameter.none,
     1: NiceAiCondParameter.turn,
     2: NiceAiCondParameter.space,
     3: NiceAiCondParameter.prevActid,
@@ -4900,19 +4756,14 @@
     34: NiceAiCondParameter.checkTargetSkillThisturn,
     35: NiceAiCondParameter.checkSelectChain,
     36: NiceAiCondParameter.countPlayerNp,
     37: NiceAiCondParameter.countPlayerSkill,
     38: NiceAiCondParameter.countPlayerSkillIncludeMasterSkill,
     39: NiceAiCondParameter.totalTurn,
     40: NiceAiCondParameter.warBoardSquareIndividuality,
-    41: NiceAiCondParameter.checkBattleValue,
-    42: NiceAiCondParameter.checkPlayerMasterSkillIndex,
-    43: NiceAiCondParameter.checkPlayerMasterSkillIndexThisTurn,
-    44: NiceAiCondParameter.countPlayerMasterSkillThisTurn,
-    45: NiceAiCondParameter.countPlayerMasterSkillThisWave,
 }
 
 
 class AiRefineTarget(IntEnum):
     ANY = 0
     ALL = 1
     HIGHER = 2
@@ -4943,45 +4794,36 @@
     NONE = 0
     EQUAL = 1
     EQUAL_NOT = 2
     HIGHER = 3
     LOWER = 4
     MULTIPLE = 5
     EXIST = 6
-    BETWEEN = 7
-    BETWEEN_NOT = 8
-    ALL_EXIST = 9
 
 
 class NiceAiCondCheck(StrEnum):
     """Ai Condition Check"""
 
     none = "none"
     equal = "equal"
     equalNot = "equalNot"
     higher = "higher"
     lower_ = "lower"
     multiple = "multiple"
     exist = "exist"
-    between = "between"
-    betweenNot = "betweenNot"
-    allExist = "allExist"
 
 
 AI_COND_CHECK_NAME: dict[int, NiceAiCondCheck] = {
     0: NiceAiCondCheck.none,
     1: NiceAiCondCheck.equal,
     2: NiceAiCondCheck.equalNot,
     3: NiceAiCondCheck.higher,
     4: NiceAiCondCheck.lower_,
     5: NiceAiCondCheck.multiple,
     6: NiceAiCondCheck.exist,
-    7: NiceAiCondCheck.between,
-    8: NiceAiCondCheck.betweenNot,
-    9: NiceAiCondCheck.allExist,
 }
 
 
 class TreasureDeviceEffectFlag(IntEnum):
     SUPPORT = -1
     ATTACK_ENEMY_ALL = 1
     ATTACK_ENEMY_ONE = 2
@@ -5704,31 +5546,7 @@
     1: NiceSvtDeadType.escape,
     2: NiceSvtDeadType.stand,
     3: NiceSvtDeadType.effect,
     4: NiceSvtDeadType.wait,
     5: NiceSvtDeadType.energy,
     6: NiceSvtDeadType.crystal,
 }
-
-
-class AiAllocationSvtFlag(IntEnum):
-    ALL = 0
-    OWN = 1
-    FRIEND = 2
-    NPC = 4
-
-
-class NiceAiAllocationSvtFlag(StrEnum):
-    """AI Allocation Svt Flag"""
-
-    all = "all"
-    own = "own"
-    friend = "friend"
-    npc = "npc"
-
-
-AI_ALLOCATION_SVT_FLAG_NAME: dict[int, NiceAiAllocationSvtFlag] = {
-    0: NiceAiAllocationSvtFlag.all,
-    1: NiceAiAllocationSvtFlag.own,
-    2: NiceAiAllocationSvtFlag.friend,
-    4: NiceAiAllocationSvtFlag.npc,
-}
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/nice.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     StageLimitActType,
     SvtClass,
 )
 from .gameenums import (
     NiceAiActNum,
     NiceAiActTarget,
     NiceAiActType,
-    NiceAiAllocationSvtFlag,
     NiceAiCond,
     NiceBattleFieldEnvironmentGrantType,
     NiceBuffType,
     NiceCardType,
     NiceClassBoardSkillType,
     NiceClassBoardSquareFlag,
     NiceCombineAdjustTarget,
@@ -346,18 +345,19 @@
     UseTreasureDevice: int | None = None
     SkillReaction: int | None = None
     BehaveAsFamilyBuff: int | None = None
     UnSubStateWhileLinkedToOthers: int | None = Field(
         default=None,
         description="The buff with this dataVal is removed if the linked buff is removed.",
     )
+    AllowSubBgmPlaying: int | None = None
     NotAccompanyWhenLinkedTargetMoveState: int | None = None
     NotTargetSkillIdArray: list[int] | None = None
     ShortTurn: int | None = None
-    FieldIndividuality: list[int] | None = None
+    FieldIndividuality: int | None = None
     BGId: int | None = None
     BGType: int | None = None
     BgmId: int | None = None
     TakeOverFieldState: int | None = None
     TakeOverNextWaveBGAndBGM: int | None = None
     RemoveFieldBuffActorDeath: int | None = None
     FieldBuffGrantType: int | None = None
@@ -396,29 +396,14 @@
     CancelTransform: int | None = None
     UnSubStateWhenContinue: int | None = None
     CheckTargetHaveDefeatPoint: int | None = None
     NPFixedDamageValue: int | None = None
     IgnoreShiftSafeDamage: int | None = None
     ActAttackFunction: int | None = None
     DelayRemoveBuffExpiredOnPlayerTurn: int | None = None
-    AllowRemoveBuff: int | None = None
-    NotExecFunctionIfKeepAliveOnWarBoard: int | None = None
-    SnapShotParamAddSelfIndv: list[int] | None = None
-    SnapShotParamAddOpIndv: list[int] | None = None
-    SnapShotParamAddFieldIndv: list[int] | None = None
-    SnapShotParamAddValue: int | None = None
-    SnapShotParamAddMaxValue: int | None = None
-    SnapShotParamAddMaxCount: int | None = None
-    NotExecOnTransform: int | None = None
-    NotRemoveOnTransform: int | None = None
-    PriorityBgm: int | None = None
-    BgmAllowSubPlaying: int | None = None
-    BgPriority: int | None = None
-    PriorityBg: int | None = None
-    ResetBgmPriorityAtWaveStart: int | None = None
     # Extra dataval from SkillLvEntty.DIC_KEY_APPLY_SUPPORT_SVT
     ApplySupportSvt: Optional[int] = None
     # These are not DataVals but guesses from SkillLvEntity and EventDropUpValInfo
     Individuality: Optional[int] = None
     EventId: Optional[int] = None
     AddCount: Optional[int] = None
     RateCount: Optional[int] = None
@@ -507,15 +492,14 @@
     icon: Optional[HttpUrl] = None
     priority: int
     isDispValue: bool
 
 
 class FunctionScript(BaseModel):
     overwriteTvals: list[list[NiceTrait]] | None = None
-    funcIndividuality: list[NiceTrait] | None = None
 
 
 class NiceBaseFunction(BaseModelORJson):
     funcId: int = Field(..., title="Function ID", description="Function ID")
     funcType: NiceFuncType = Field(
         ..., title="Function type", description="Function type"
     )
@@ -1786,14 +1770,15 @@
     condGroup: int
     condType: NiceCondType
     targetIds: list[int]
     targetNum: int
     conditionMessage: str
     closedMessage: str
     flag: int
+    detail: Optional[NiceEventMissionConditionDetail] = None
     details: list[NiceEventMissionConditionDetail] | None = None
 
 
 class NiceEventMission(BaseModelORJson):
     id: int
     flag: int
     type: NiceMissionType
@@ -1886,21 +1871,23 @@
 class NiceEventTreasureBox(BaseModelORJson):
     slot: int
     id: int
     idx: int
     treasureBoxGifts: list[NiceEventTreasureBoxGift]
     maxDrawNumOnce: int
     extraGifts: list[NiceGift]
+    commonConsume: NiceCommonConsume
     consumes: list[NiceCommonConsume]
 
 
 class NiceEventDiggingBlock(BaseModelORJson):
     id: int
     eventId: int
     image: HttpUrl
+    commonConsume: NiceCommonConsume
     consumes: list[NiceCommonConsume]
     objectId: int
     diggingEventPoint: int
     blockNum: int
 
 
 class NiceEventDiggingReward(BaseModelORJson):
@@ -1920,14 +1907,15 @@
     rewards: list[NiceEventDiggingReward]
 
 
 class NiceEventCooltimeReward(BaseModelORJson):
     spotId: int
     lv: int
     name: str
+    commonRelease: NiceCommonRelease
     releaseConditions: list[NiceCommonRelease]
     cooltime: int
     addEventPointRate: int
     gifts: list[NiceGift]
     upperLimitGiftNum: int
 
 
@@ -2477,20 +2465,14 @@
     id: int
     type: NiceBattleFieldEnvironmentGrantType
     priority: int
     individuality: list[NiceTrait]
     imageId: int
 
 
-class NiceAiAllocation(BaseModelORJson):
-    aiIds: list[int]
-    individuality: NiceTrait
-    applySvtType: list[NiceAiAllocationSvtFlag]
-
-
 class NiceStage(BaseModelORJson):
     wave: int
     bgm: NiceBgm
     startEffectId: int
     fieldAis: list[FieldAi] = []
     call: list[int] = Field([], title="Summon these NPC IDs")
     enemyFieldPosCount: int | None = None
@@ -2499,15 +2481,14 @@
     limitAct: StageLimitActType | None = Field(
         None, title="Action after turn countdown is over"
     )
     battleBg: NiceBattleBg | None = None
     NoEntryIds: list[int] | None = None
     waveStartMovies: list[NiceStageStartMovie] = []
     cutin: NiceStageCutIn | None = None
-    aiAllocations: list[NiceAiAllocation] | None = None
     originalScript: dict[str, Any]
     enemies: list[QuestEnemy] = []
 
 
 class NiceQuestMessage(BaseModelORJson):
     idx: int
     message: str
@@ -2611,35 +2592,30 @@
     detail: QuestEnemy | None = None
     aiIds: list[int]
 
 
 class NiceQuestPhaseOverwriteEquipSkill(BaseModelORJson):
     lv: int
     id: int
-    condId: int | None = None
 
 
 class NiceQuestPhaseOverwriteEquipSkills(BaseModelORJson):
-    iconId: int | None = None
-    cutInView: int | None = None  # 1: ShowMasterSkillCutIn
-    notDispEquipSkillIconSplit: int | None = None
+    iconId: int
     skills: list[NiceQuestPhaseOverwriteEquipSkill]
 
 
 class NiceQuestPhaseExtraDetail(BaseModelORJson):
     questSelect: list[int] | None = None
     singleForceSvtId: int | None = None
     hintTitle: str | None = None
     hintMessage: str | None = None
     aiNpc: NiceQuestPhaseAiNpc | None = None
     aiMultiNpc: list[NiceQuestPhaseAiNpc] | None = None
     overwriteEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
-    addEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
     waveSetup: int | None = None  # U Olga Marie Quest
-    interruptibleQuest: int | None = None
     masterImageId: int | None = None
 
 
 class NiceRestriction(BaseModelORJson):
     id: int
     name: str
     type: NiceRestrictionType
@@ -2922,15 +2898,14 @@
     squares: list[NiceClassBoardSquare]
     lines: list[NiceClassBoardLine]
 
 
 class NiceFuncTypeDetail(BaseModelORJson):
     funcType: NiceFuncType
     ignoreValueUp: bool
-    individuality: list[NiceTrait] | None = None
 
 
 class NiceBuffTypeDetail(BaseModelORJson):
     buffType: NiceBuffType
     ignoreValueUp: bool
     script: dict[str, Any]
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/raw.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,23 +251,14 @@
 
 
 class MstSvtAdd(BaseModelORJson):
     svtId: int
     script: dict[str, Any]
 
 
-class MstSvtTransform(BaseModelORJson):
-    befSvtId: int
-    befDispLimitCount: int
-    befTitle: str
-    aftSvtId: int
-    aftDispLimitCount: int
-    aftTitle: str
-
-
 # Dummy ID that is used when enemy servant does an extra attack instead of NP
 EXTRA_ATTACK_TD_ID = 100
 
 
 class MstTreasureDevice(BaseModelORJson):
     individuality: list[int]  # [3000, 4001, 4007],
     script: dict[str, Any]  # {"limitSeqId_12": 800140, "randomWeights_3": [50, 50]},
@@ -1937,25 +1928,14 @@
 class MstQuestRestrictionInfo(BaseModelORJson):
     script: dict[str, Any]
     questId: int
     phase: int
     flag: int
 
 
-class MstQuestPhasePresent(BaseModelORJson):
-    questId: int
-    phase: int
-    giftId: int
-    presentMessageId: int
-    condType: int
-    condId: int
-    condNum: int
-    script: dict[str, Any]
-
-
 class MstRestriction(BaseModelORJson):
     targetVals: list[int]
     targetVals2: list[int] | None
     id: int
     name: str
     type: int
     rangeType: int
@@ -2446,15 +2426,14 @@
     id: int
     detail: str
 
 
 class MstFuncTypeDetail(BaseModelORJson):
     funcType: int
     ignoreValueUp: bool
-    individuality: list[int] | None = None
 
 
 class MstBuffTypeDetail(BaseModelORJson):
     buffType: int
     ignoreValueUp: bool
     script: dict[str, Any]
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/rayshift.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.30.1.3.28/fgo_api_types/search.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,27 +343,25 @@
     popupText: Optional[str] = Query(None, max_length=999)
     type: list[NiceFuncType] = Query([])
     targetType: list[NiceFuncTargetType] = Query([])
     targetTeam: list[FuncApplyTarget] = Query([])
     vals: list[Union[Trait, int]] = Query([])
     tvals: list[Union[Trait, int]] = Query([])
     questTvals: list[Union[Trait, int]] = Query([])
-    funcIndividuality: list[Union[Trait, int]] = Query([])
 
     def hasSearchParams(self) -> bool:
         return any(
             [
                 self.popupText,
                 self.type,
                 self.targetType,
                 self.targetTeam,
                 self.vals,
                 self.tvals,
                 self.questTvals,
-                self.funcIndividuality,
             ]
         )
 
     DESCRIPTION: ClassVar[str] = inspect.cleandoc(
         """
         Search and return the list of matched buffs.
 
@@ -371,15 +369,14 @@
         - **type**: an item of NiceFuncType.
         - **targetType**: an item of NiceFuncTargetType.
         - **targetTeam**: `player`, `enemy` or `playerAndEnemy`.
         - **vals**: an integer or a trait enum. Note that trait enums will be converted to integers before searching
         so the search might return vals with buffs that have the same ids.
         - **tvals**: an integer or a trait enum.
         - **questTvals**: integer.
-        - **funcIndividuality**: an integer or a trait enum.
 
         At least one of the parameter is required for the query.
         """
     )
 
 
 @dataclass
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/pyproject.toml` & `fgo_api_types-2024.4.6.2.22.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.04.30.01.03.28"
+version = "2024.04.06.02.22.03"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.4.30.1.3.28/PKG-INFO` & `fgo_api_types-2024.4.6.2.22.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.4.30.1.3.28
+Version: 2024.4.6.2.22.3
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

