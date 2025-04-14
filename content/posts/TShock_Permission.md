---
title: "TShock 5.2.4 权限表"
date: 2025-04-14
author: TShock
---
## TShock 5.2.4 权限表  
在TShock后台一键享受原版体验：  
```
/group addperm default tshock.ignore.damage tshock.ignore.projectile tshock.ignore.removetile tshock.npc.hurttown tshock.npc.spawnpets tshock.npc.startdd2 tshock.npc.startinvasion tshock.npc.summonboss tshock.tp.demonconch tshock.tp.magicconch tshock.tp.pylon   tshock.tp.rod tshock.tp.tppotion tshock.tp.wormhole   tshock.world.movenpc   tshock.world.time.usemoondial tshock.world.time.usesundial tshock.world.worldupgrades 
```
也可以使用[Ezperm 便捷权限](https://docs.terraria.ink/zh/guide/Ezperm.html) 这个插件
| 权限名称                              | 说明                                            | 命令                                                                                     | 享受原版体验 |
| --------------------------------- | ---------------------------------------------- | ---------------------------------------------------------------------------------------- | ------ |
| tshock.account.changepassword     | 用户可以在游戏中更改密码                                   | /password                                                                                |        |
| tshock.account.login              | 用户可以在游戏中登录。                                    | /login                                                                                   |        |
| tshock.account.logout             | 用户可以在游戏中登出。                                    | /logout                                                                                  |        |
| tshock.account.register           | 用户可以在游戏中注册账户。                                  | /register                                                                                |        |
| tshock.accountinfo.check          | 玩家可以检查用户名是否已注册，并查看其上次登录时间。                     | /accountinfo (/ai)                                                                       |        |
| tshock.accountinfo.details        | 玩家可以查看任意用户账户的详细信息。                             | 无                                                                                        |        |
| tshock.admin.antibuild            | 用户可以设置建筑保护状态。*                                 | /antibuild                                                                               |        |
| tshock.admin.ban                  | 用户可以封禁他人。                                      | /ban                                                                                     |        |
| tshock.admin.broadcast            | 用户可以广播消息。                                      | /broadcast (/bc /say)                                                                    |        |
| tshock.admin.group                | 用户可以管理组。                                       | /group                                                                                   |        |
| tshock.admin.itemban              | 用户可以管理物品封禁。                                    | /itemban                                                                                 |        |
| tshock.admin.kick                 | 用户可以踢出他人。                                      | /kick                                                                                    |        |
| tshock.admin.mute                 | 用户可以禁言和取消禁言用户。                                 | /mute (/unmute)                                                                          |        |
| tshock.admin.noban                | 防止你被封禁。                                        | 无                                                                                        |        |
| tshock.admin.nokick               | 防止你被踢出。                                        | 无                                                                                        |        |
| tshock.admin.projectileban        | 用户可以管理弹幕禁令。                                    | /projban                                                                                 |        |
| tshock.admin.region               | 用户可以管理区域。                                      | /region                                                                                  |        |
| tshock.admin.savessi              | 用户可以保存所有玩家的SSC（服务器端角色）状态。                      | /overridessc (/ossc), /savessc                                                           |        |
| tshock.admin.seeplayerids         | 用户可以使用/who -i 查看玩家的ID。                         | 无                                                                                        |        |
| tshock.admin.tempgroup            | 用户可以临时提升其他用户的组。                                | /tempgroup                                                                               |        |
| tshock.admin.tileban              | 用户可以管理物块禁令。                                    | /tileban                                                                                 |        |
| tshock.admin.userinfo             | 用户可以获得其他用户的信息。                                 | /userinfo (/ui)                                                                          |        |
| tshock.admin.viewlogs             | 具有此权限的用户将收到特定的日志消息。                            | /displaylogs                                                                             |        |
| tshock.admin.warp                 | 用户可以管理传送点。                                     | 无                                                                                        |        |
| tshock.annoy                      | 用户可以骚扰他人。                                      | /annoy, /rocket, /firework                                                               |        |
| tshock.buff.others                | 用户可以给其他玩家增益。                                   | /gbuff (/buffplayer)                                                                     |        |
| tshock.buff.self                  | 用户可以给自己增益。                                     | /buff                                                                                    |        |
| tshock.canchat                    | 玩家可以聊天。                                        | 无                                                                                        |        |
| tshock.cfg.createdumps            | 用户可以在服务器文件夹中创建泰拉瑞亚ID和权限矩阵的参考文件。                | /dump-reference-data                                                                     |        |
| tshock.cfg.maintenance            | 当有更新可用时，用户会收到通知，并且用户可以关闭或重启服务器。                | /checkupdates, /off (/exit /stop), /off-nosave (/exit-nosave<br> /stop-nosave), /version |        |
| tshock.cfg.password               | 用户可以编辑服务器密码。                                   | /serverpassword                                                                          |        |
| tshock.cfg.reload                 | 用户可以重新加载配置文件。                                  | /reload                                                                                  |        |
| tshock.cfg.whitelist              | 用户可以修改白名单。                                     | /whitelist                                                                               |        |
| tshock.clear                      | 用户可以清除物品或弹幕。                                   | /clear                                                                                   |        |
| tshock.godmode                    | 切换玩家旅行上帝模式                                     | /godmode (/god)                                                                          |        |
| tshock.godmode.other              | 用户可以切换其他玩家旅行上帝模式                               | 无                                                                                        |        |
| tshock.heal                       | 用户可以治愈玩家。                                      | /heal                                                                                    |        |
| tshock.ignore.damage              | 忽略伤害过高检测。                                      | 无                                                                                        | 推荐开启   |
| tshock.ignore.dropbanneditem      | 允许丢弃禁止的物品，而物品不会被清除。                            | 无                                                                                        |        |
| tshock.ignore.hp                  | 忽略血量上限检测。                                      | 无                                                                                        |        |
| tshock.ignore.itemstack           | 忽略物品堆叠数量检测。                                    | 无                                                                                        |        |
| tshock.ignore.liquid              | 忽略液体使用速率检测。                                    | 无                                                                                        |        |
| tshock.ignore.mp                  | 忽略魔力上限检测。                                      | 无                                                                                        |        |
| tshock.ignore.npcbuff             | 忽略给NPC上buff检测。                                 | 无                                                                                        |        |
| tshock.ignore.paint               | 忽略给刷漆速率检测。                                     | 无                                                                                        |        |
| tshock.ignore.placetile           | 忽略放物块速率检测。                                     | 无                                                                                        |        |
| tshock.ignore.projectile          | 忽略射弹幕速率检测。                                     | 无                                                                                        | 推荐开启   |
| tshock.ignore.removetile          | 忽略图格破坏速率检测。                                    | 无                                                                                        | 推荐开启   |
| tshock.ignore.sendtilesquare      | 允许无限制使用SendTileSquare功能，用于客户端世界编辑。             | 无                                                                                        |        |
| tshock.ignore.ssc                 | 绕过服务器端SSC（类似云存档）检查。                            | 无                                                                                        |        |
| tshock.info                       | 用户可以获得服务器信息。                                   | /serverinfo                                                                              |        |
| tshock.item.give                  | 用户可以给予物品。                                      | /give (/g)                                                                               |        |
| tshock.item.spawn                 | 用户可以生成物品。                                      | /item (/i)                                                                               |        |
| tshock.item.usebanned             | 允许你使用被禁止的物品。                                   | 无                                                                                        |        |
| tshock.journey.biomespreadfreeze  | 用户可以使用旅途界面停止世界的生物群系扩散。                         | 无                                                                                        |        |
| tshock.journey.godmode            | 用户可以在旅途界面切换上帝模式。                               | 无                                                                                        |        |
| tshock.journey.placementrange     | 用户可以在旅途界面切换增加放置范围。                             | 无                                                                                        |        |
| tshock.journey.rain.freeze        | 用户可以在旅途界面冻结世界降雨强度的变化。                          | 无                                                                                        |        |
| tshock.journey.rain.strength      | 用户可以在旅途界面设置世界降雨强度/种子。                          | 无                                                                                        |        |
| tshock.journey.research           | 用户可以在旅途界面进行物品研究。                               | 无                                                                                        |        |
| tshock.journey.setdifficulty      | 用户可以在旅途界面设置世界难度/模式。                            | 无                                                                                        |        |
| tshock.journey.setspawnrate       | 用户可以在旅途界面设置世界的NPC生成率。                          | 无                                                                                        |        |
| tshock.journey.time.freeze        | 用户可以在旅途界面冻结时间。                                 | 无                                                                                        |        |
| tshock.journey.time.set           | 用户可以在旅途界面设置世界时间。                               | 无                                                                                        |        |
| tshock.journey.time.setspeed      | 用户可以在旅途界面设置世界时间速度。                             | 无                                                                                        |        |
| tshock.journey.wind.freeze        | 用户可以在旅途界面冻结世界风强度变化。                            | 无                                                                                        |        |
| tshock.journey.wind.strength      | 用户可以在旅途界面设置世界风强度/种子。                           | 无                                                                                        |        |
| tshock.kill                       | 用户可以杀死他人。                                      | /kill (/slay)                                                                            |        |
| tshock.npc.butcher                | 用户可以杀死所有敌对NPC。                                 | /butcher                                                                                 |        |
| tshock.npc.clearanglerquests      | 用户可以清除当天已完成渔夫任务的用户列表。                          | /clearangler                                                                             |        |
| tshock.npc.hurttown               | 用户可以伤害城镇NPC。                                   | 无                                                                                        | 推荐开启   |
| tshock.npc.invade                 | 用户可以开始入侵. 警告：高网络使用。容易滥用。                       | 无                                                                                        |        |
| tshock.npc.maxspawns              | 用户可以编辑生物最大生成数。                                 | /maxspawns                                                                               |        |
| tshock.npc.rename                 | 用户可以重命名NPC。                                    | /renamenpc                                                                               |        |
| tshock.npc.spawnboss              | 用户可以生成Boss。                                    | /spawnboss (/sb)                                                                         |        |
| tshock.npc.spawnmob               | 用户可以生成NPC。                                     | /spawnmob (/sm)                                                                          |        |
| tshock.npc.spawnpets              | 用户可以生成宠物。警告：高网络使用。容易滥用。                        | 无                                                                                        | 推荐开启   |
| tshock.npc.spawnrate              | 用户可以编辑生物生成率。                                   | /spawnrate                                                                               |        |
| tshock.npc.startdd2               | 用户可以开始dd2（旧日军团）事件。                             | 无                                                                                        | 推荐开启   |
| tshock.npc.startinvasion          | 用户可以使用物品开始入侵（哥布林雪人等）。                          | 无                                                                                        | 推荐开启   |
| tshock.npc.summonboss             | 用户可以使用物品召唤Boss。                                | 无                                                                                        | 推荐开启   |
| tshock.partychat                  | 用户可以在游戏中使用队伍聊天。                                | /party (/p)                                                                              |        |
| tshock.projectiles.usebanned      | 玩家可以使用被禁止的弹幕。                                  | 无                                                                                        |        |
| tshock.reservedslot               | 允许您突破最大玩家数限制，最多可超过上限5个玩家数。                     | 无                                                                                        |        |
| tshock.respawn                    | 玩家可以自己用指令复活。                                   | /respawn                                                                                 |        |
| tshock.respawn.other              | 玩家可以用指令复活他人。                                   | 无                                                                                        |        |
| tshock.sendemoji                  | 玩家可以发送表情。                                      | 无                                                                                        |        |
| tshock.slap                       | 用户可以打别人。                                       | /slap                                                                                    |        |
| tshock.ssc.upload                 | 用户可以上传他们加入的角色数据作为SSC数据。                        | /uploadssc                                                                               |        |
| tshock.ssc.upload.others          | 用户可以上传其他玩家加入的数据到SSC数据库。                        | 无                                                                                        |        |
| tshock.su                         | 允许用户提升为超级管理员10分钟。                              | /su, /sudo                                                                               |        |
| tshock.superadmin.user            | 仅供超级管理员使用。                                     | /user                                                                                    |        |
| tshock.synclocalarea              | 玩家可以与服务器状态重新同步。                                | /sync                                                                                    |        |
| tshock.thirdperson                | 用户可以用第三人称说话。                                   | /me                                                                                      |        |
| tshock.tiles.usebanned            | 玩家可以放置被禁止的物块                                   | 无                                                                                        |        |
| tshock.tp.allothers               | 用户可以将所有人*传送到他那里。                               | 无                                                                                        |        |
| tshock.tp.block                   | 用户可以阻止他人传送。                                    | /tpallow                                                                                 |        |
| tshock.tp.demonconch              | 用户可以使用恶魔海螺。                                    | 无                                                                                        | 推荐开启   |
| tshock.tp.getpos                  | 用户可以获得玩家的位置。                                   | /pos                                                                                     |        |
| tshock.tp.home                    | 用户可以使用 /home.                                  | /home                                                                                    |        |
| tshock.tp.magicconch              | 用户可以使用魔法海螺。                                    | 无                                                                                        | 推荐开启   |
| tshock.tp.npc                     | 用户可以传送到NPC。                                    | /tpnpc                                                                                   |        |
| tshock.tp.others                  | 用户可以传送其他人到自己身边。                                | /tphere                                                                                  |        |
| tshock.tp.override                | 用户可以无视传送阻止。                                    | 无                                                                                        |        |
| tshock.tp.pos                     | 用户可以传送到指定物块位置。                                 | /tppos                                                                                   |        |
| tshock.tp.pylon                   | 用户可以使用晶塔进行传送。                                  | 无                                                                                        | 推荐开启   |
| tshock.tp.rod                     | 用户可以使用混沌传送杖。                                   | 无                                                                                        | 推荐开启   |
| tshock.tp.self                    | 用户可以传送到其他人。                                    | /tp                                                                                      |        |
| tshock.tp.silent                  | 用户可以在不显示通知的情况下传送到其他人那里。                        | 无                                                                                        |        |
| tshock.tp.spawn                   | 用户可以使用出生点传送 /spawn。                            | /spawn                                                                                   |        |
| tshock.tp.tppotion                | 用户可以使用传送药水。                                    | 无                                                                                        | 推荐开启   |
| tshock.tp.wormhole                | 用户可以使用虫洞药水。                                    | 无                                                                                        | 推荐开启   |
| tshock.warp                       | 用户可以使用传送点。                                     | /warp                                                                                    |        |
| tshock.whisper                    | 用户可以对其他人私聊。                                    | /reply (/r), /whisper (/w /tell /pm /dm), /wallow (/wa)                                  |        |
| tshock.world.converthardmode      | 用户可以将神圣转化为腐化，反之亦然。*                            | 无                                                                                        |        |
| tshock.world.editregion           | 允许你编辑区域。                                       | 无                                                                                        |        |
| tshock.world.editspawn            | 允许你编辑出生点。                                      | /protectspawn                                                                            |        |
| tshock.world.events               | 用户可以使用'worldevent'命令。                          | /worldevent                                                                              |        |
| tshock.world.events.bloodmoon     | 用户可以使用'worldevent'命令的'bloodmoon'（血月）子命令。       | /worldevent bloodmoon                                                                    |        |
| tshock.world.events.eclipse       | 用户可以使用'worldevent'命令的'eclipse'（日食）子命令。         | /worldevent eclipse                                                                      |        |
| tshock.world.events.fullmoon      | 用户可以使用'worldevent'命令的'fullmoon'（满月）子命令。        | /worldevent fullmoon                                                                     |        |
| tshock.world.events.invasion      | 用户可以使用'worldevent'命令的'invasion'（入侵）子命令。        | /worldevent invasion                                                                     |        |
| tshock.world.events.lanternsnight | 用户可以使用'worldevent'命令的'lanternsnight'（灯笼之夜）子命令。 | /worldevent lanternsnight                                                                |        |
| tshock.world.events.meteor        | 用户可以使用'worldevent'命令的'meteor'（陨石）子命令。          | /worldevent meteor                                                                       |        |
| tshock.world.events.rain          | 用户可以使用'worldevent'命令的'rain'（雨）子命令。             | /worldevent rain                                                                         |        |
| tshock.world.events.sandstorm     | 用户可以使用'worldevent'命令的'sandstorm'（沙尘暴）子命令。      | /worldevent sandstorm                                                                    |        |
| tshock.world.grow                 | 用户可以指令种植植物。                                    | /grow                                                                                    |        |
| tshock.world.growevil             | 用户可以指令种植邪恶生物群系的植物。                             | 无                                                                                        |        |
| tshock.world.hardmode             | 用户可以更改困难模式状态。                                  | /hardmode                                                                                |        |
| tshock.world.info                 | 用户可以获得世界信息。                                    | /worldinfo                                                                               |        |
| tshock.world.modify               | 用户可以修改世界。                                      | 无                                                                                        |        |
| tshock.world.movenpc              | 用户可以改变NPC的家。                                   | 无                                                                                        | 推荐开启   |
| tshock.world.paint                | 用户可以对物块刷漆。                                     | 无                                                                                        |        |
| tshock.world.rain                 | 用户可以开启或关闭下雨功能。                                 | 无                                                                                        |        |
| tshock.world.sandstorm            | 用户可以开启或关闭沙尘暴。                                  | 无                                                                                        |        |
| tshock.world.save                 | 用户可以保存世界。                                      | /save                                                                                    |        |
| tshock.world.setdungeon           | 用户可以设置地牢的位置。                                   | /setdungeon                                                                              |        |
| tshock.world.sethalloween         | 用户可以强制服务器进入万圣节模式。                              | /forcehalloween                                                                          |        |
| tshock.world.setspawn             | 用户可以设置世界出生点。                                   | /setspawn                                                                                |        |
| tshock.world.settleliquids        | 用户可以快速平衡液体。                                    | /settle                                                                                  |        |
| tshock.world.setxmas              | 用户可以强制服务器进入圣诞节模式。                              | /forcexmas                                                                               |        |
| tshock.world.time.bloodmoon       | 用户可以强制触发血月。                                    | /worldevent bloodmoon                                                                    |        |
| tshock.world.time.dropmeteor      | 用户可以触发陨石坠落。                                    | /worldevent meteor                                                                       |        |
| tshock.world.time.eclipse         | 用户可以强制触发日食。                                    | /worldevent eclipse                                                                      |        |
| tshock.world.time.fullmoon        | 用户可以强制触发满月。                                    | /worldevent fullmoon                                                                     |        |
| tshock.world.time.set             | 用户可以设置时间。                                      | /time                                                                                    |        |
| tshock.world.time.usemoondial     | 玩家可以使用附魔月晷物品。                                  | 无                                                                                        | 推荐开启   |
| tshock.world.time.usesundial      | 玩家可以使用附魔日晷物品。                                  | 无                                                                                        | 推荐开启   |
| tshock.world.toggleexpert         | 用户可以更改专家状态。                                    | /worldmode (/gamemode)                                                                   |        |
| tshock.world.toggleparty          | 玩家可以切换派对事件。                                    | 无                                                                                        |        |
| tshock.world.wind                 | 用户可以修改风。                                       | /wind                                                                                    |        |
| tshock.world.worldupgrades        | 用户可以使用世界永久加成的物品，例如先进战斗技术和游商背包。                      | 无                                                                                        | 推荐开启   |
