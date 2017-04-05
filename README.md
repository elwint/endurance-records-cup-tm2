# Modified Records Eyepiece for Endurance(Cup) [TM2]

Support for: `Endurance.Script.txt` & `EnduranceCup.Script.txt`

Working: Local Records (+ points system)

To make use of the points system, use `EnduranceCup.Script.txt`

## Warning

Don't excpect it to be 100% bug free. A lot of improvements of the original code still needs to be done.

## Installation

First place the files in the correct folders of XAseco2 and the script in the Scripts folder of your dedicated server.

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

You can also change the points settings in `records_eyepiece_enduro.xml`

## Commands

/points [Show points system]

/switch [Switch to another script] (ADMIN)

/resetpoints [Reset total points] (ADMIN)

/whitelist [Manage whitelist] (ADMIN)

/kickall [Kick all players except admins and whitelisted players] (ADMIN)

/setrounds [Set the amount of endurance rounds (default: 3)] (ADMIN)

/setmaps [Set the amount of endurance maps (default: 1)] (ADMIN)

/setdecreaser [Set multiplication per CP (default: 0.95)] (ADMIN)

/fakeplayer [Connect/disconnect fakeplayer(s)] (ADMIN)(DEBUG)
