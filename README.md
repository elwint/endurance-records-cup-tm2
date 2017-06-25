# EnduroCup script and XAseco2 plugin [TM2][MP4]

![screenshot example](https://drive.google.com/uc?export=view&id=0B-t0hZwYZIWSVGpTc1B0QjNkdU0)

## Modified Records Eyepiece plugin

Works in MP4 with XAseco2.

Support for: `EnduroCup.Script.txt` & `TimeAttack.Script.txt`

Features: Local records + Total points system

## Warning

Don't excpect it to be 100% bug free. A lot of improvements of the original code still needs to be done.

## Installation

Place the plugin file in the XAseco2 plugin folder and the script in the Scripts folder of your dedicated server.

Edit your `plugins.xml` of XAseco2:

Remove:

```xml
<plugin>plugin.checkpoints.php</plugin>
<plugin>plugin.dedimania.php</plugin>
<plugin>chat.dedimania.php</plugin>
```

(And any other plugins depended on these)

Replace:

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

/switch [Switch to another script] (ADMIN)

/resetpoints [Reset total points] (ADMIN)

/whitelist [Manage whitelist] (ADMIN)

/kickall [Kick all players except admins and whitelisted players] (ADMIN)

/save [Save current total points in a CSV file] (ADMIN)

/setrounds [Set the amount of enduro rounds (default: 3)] (ADMIN)

/setmaps [Set the amount of enduro maps (default: 1)] (ADMIN)

/setdecreaser [Set multiplication per CP (default: 0.95)] (ADMIN)

/fakeplayer [Connect/disconnect fakeplayer(s)] (ADMIN)(DEBUG)
