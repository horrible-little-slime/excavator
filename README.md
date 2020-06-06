# excavator

excavator is a `spadingScript` for KoLmafia (at least r20145) for collaboratively gathering data while playing the Kingdom of Loathing. It collects and stores data throughout your play into the `spadingData` property, which will then be send via kmail to the player `Excavator` once you run the `spade` command in the CLI.

Only data pertinent to the [current projects](#current-projects) are reported (outcomes from combats, state of flags or counters on your player etc) and each packet of data can be reviewed and approved before it is sent. No personal information will ever be transmitted.

These data are pulled once an hour to the [excavator-data](https://github.com/gausie/excavator-data) repository.

It is maintained by gausie (#1197090).

## Installation and Usage

Install the script using the KoLmafia CLI:

```
svn checkout https://github.com/gausie/excavator/trunk/RELEASE/
```

Set up KoLmafia to use `excavator.ash` as your spadingScript:

```
set spadingScript = excavator.ash
```

Data will be collected in the `spadingData` prop, which can be reviewed and submitted using the `spade` command:

```
spade
```

A reminder to do so appears on login and in the Daily Deeds panel.

## Current projects

* **[Guzzlr](RELEASE/scripts/excavator/projects/x_guzzlr.ash)** - Determine the relationship between Guzzlr deliveries and enchantments on the Guzzlr tablet accessory
* **[Hookah](RELEASE/scripts/excavator/projects/x_hookah.ash)** - Submit data if an effect is obtained through a hookah-like mechanic that KoLmafia thinks shouldn't be possible
* **[Mumming Trunk](RELEASE/scripts/excavator/projects/x_mumming_trunk.ash)** - Record instances of a familiar indicating that it has a previous undetected attribute through mumming trunk bonuses

## Further information

To get involved in writing a project or if you have any other queries join us on the [Ascension Speed Society Discord server](https://discord.gg/T3rqfve).