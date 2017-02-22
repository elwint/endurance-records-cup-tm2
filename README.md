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

/setrounds [Set the amount of endurance rounds (default: 3)]

/setmaps [Set the amount of endurance maps (default: 1)]

/resetpoints [Reset total points]

/switch [Switch to another script]
