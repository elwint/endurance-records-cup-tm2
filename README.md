# Modified Records Eyepiece for Endurance(Cup) [TM2]

## Warning

Don't excpect it to be 100% bug free

Code is kinda garbage, I modified the files a long time ago and updated it recently in a really short time

But at least it works :)

## Installation

Place the files in the correct folders

Edit your `plugins.xml`:

Remove:

```xml
<plugin>plugin.checkpoints.php</plugin>
<plugin>plugin.dedimania.php</plugin>
<plugin>chat.dedimania.php</plugin>
```

(And any other plugins depended on these)

Replace:

```xml
<plugin>plugin.localdatabase.php</plugin>
<plugin>plugin.records_eyepiece.php</plugin>
```

with

```xml
<plugin>plugin.localdatabase_enduro.php</plugin>
<plugin>plugin.records_eyepiece_enduro.php</plugin>
```

A working example of `plugins.xml` can be found in the repository

## Configuration

The config file `records_eyepiece_enduro.xml` will be used for `plugin.records_eyepiece_enduro.php`

Your config file `localdatabase.xml` will be used for `plugin.localdatabase_enduro.php`

You can change the points in `plugin.localdatabase_enduro.php`
