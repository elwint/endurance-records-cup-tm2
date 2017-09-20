# EnduroCup script and XAseco2 plugin [TM2][MP4]

![screenshot example](https://drive.google.com/uc?export=view&id=0B-t0hZwYZIWSVGpTc1B0QjNkdU0)

## Modified Records Eyepiece plugin

Works in MP4 with XAseco2.

Support for: `EnduroCup.Script.txt` & `TimeAttack.Script.txt`

Features: Total points system, local records, control EnduroCup settings in-game, extra commands.

## Warning

Don't excpect it to be 100% bug free. A lot of improvements of the original code still needs to be done.

## Installation

Place the plugin file in the XAseco2 plugin folder and the script in the Scripts folder of your dedicated server.

Edit your `plugins.xml` of XAseco2:

To make the plugin work, comment/remove these plugins:

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

The config file `records_eyepiece_enduro.xml` will be used for `plugin.records_eyepiece_enduro.php`

**Note:** when changing the points, change it in `EnduroCup.Script.txt` as well.

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

/save [Save current total points in the CSV file] (ADMIN)

/remove [Remove last total points in the CSV file] (ADMIN)

/fakeplayer [Connect/disconnect/simulate fakeplayer(s)] (ADMIN)(DEBUG)
