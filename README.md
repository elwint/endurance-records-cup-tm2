# EnduroCup script and XAseco2 plugin [TM2][MP4] (deprecated)

***This script/plugin is no longer maintained***

![screenshot example](https://drive.google.com/uc?export=view&id=1iemqrSLBSlt_0stk6Fe0ifcz3ybUNOOX)

## Original authors

Endurance script: TGYoshi/Tiggs

Records Eyepiece: undef.de

## Modified Records Eyepiece plugin

Works in MP4 with XAseco2.

Support for: `EnduroCup.Script.txt` & `TimeAttack.Script.txt` (and a custom shitfest script (not included))

Features: Total points system, local records, control EnduroCup settings in-game, extra commands.

## Warning

The code is old, it might contain some vulnerabilities. Don't excpect it to be 100% bug free. A lot of improvements to the original code still needs to be done.

## Installation

Put the plugin file in the XAseco2 plugin folder, the config file in the XAseco2 folder and the script in the Scripts folder of your dedicated server.

Edit your `plugins.xml` of XAseco2:

To make the plugin work properly, comment/remove these plugins:

```xml
<plugin>plugin.checkpoints.php</plugin>
<plugin>plugin.dedimania.php</plugin>
<plugin>chat.dedimania.php</plugin>
<plugin>chat.me.php</plugin>
```

(And any other plugins depending on these)

And replace:

```xml
<plugin>plugin.records_eyepiece.php</plugin>
```

with

```xml
<plugin>plugin.records_eyepiece_enduro.php</plugin>
```

A working example of `plugins.xml` can be found in the repository.

## Configuration

The config file is `records_eyepiece_enduro.xml`

**Note:** if you want to change the points, update it both in the config file and in `EnduroCup.Script.txt` to show the correct points on the scoreboard.

### Nouse Message

There is additional support for `plugin.nouse.message.php`

```xml
<infotext>General message</infotext>
<infotext>{*scriptname*}This message is only visible in the specified script</infotext>
<infotext>{TimeAttack}This message is only visible in TimeAttack</infotext>
<infotext>{Endurocup}Current Round: %current_round%/%rounds%</infotext>
<infotext>{Endurocup}Current Map: %current_map%/%maps%</infotext>
<infotext>{Endurocup}Server password: %password%</infotext>
```

## Commands

/points [Show points system]

/setrounds [Set the amount of enduro rounds (default: 3)] (ADMIN)

/setmaps [Set the amount of enduro maps (default: 1)] (ADMIN)

/setdecreaser [Set multiplication per CP (default: 0.95)] (ADMIN)

/switch [Switch to another script] (ADMIN)

/resetpoints [Reset total points] (ADMIN)

/whitelist [Manage whitelist] (ADMIN)

/kickall [Kick all players except admins and whitelisted players] (ADMIN)

/muteall [Mute public chat] (ADMIN)

/unmuteall [Unmute public chat] (ADMIN)

/save [Save current (total) points in the CSV file] (ADMIN)

/remove [Remove last (total) points in the CSV file] (ADMIN)

/fakeplayer [Connect/disconnect/simulate fakeplayer(s)] (ADMIN)(DEBUG)
