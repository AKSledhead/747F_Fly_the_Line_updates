# 747 Fly the Line — Freighter — updates

Updates for **747 Fly the Line**, a first officer and flight engineer for
the Felis Boeing 747-200 freighter in X-Plane 12. SkunkCrafts Updater
downloads them from here.

**This is for the freighter, `747F_Felis`, only.** The Felis passenger
747-200 is a separate aircraft and is not supported yet. It will have its
own updates when it is.

This repository holds the released plugin only, not its source.

## Where it installs

In the freighter's own plugins folder, not in `Resources/plugins`:

```
X-Plane 12/Aircraft/747F_Felis/plugins/747_Fly_the_Line/
```

X-Plane then loads the plugin only when the freighter is loaded.

**Do not put a second copy in `Resources/plugins`.** X-Plane would load
both, and every callout and switch action would happen twice. If anything
happens twice, look for a second copy first.

## Turn off similar add-ons

The first officer and flight engineer set their own panels: fuel,
electrics, pneumatics and lights. **Turn off any other add-on that works
the same switches**, such as fuel management scripts, XFirstOfficer, or
another first officer or flight engineer add-on. Otherwise a switch the
crew set can be moved back by the other add-on.

## Crew voices

The voices are included, in `voice/<accent>/`, and are updated with the
plugin. Three accents: American (`US`), British (`UK`) and European
(`EU`). Delete an accent's folder to take it off the list; the next update
restores it.

## After a Felis update

A Felis update usually replaces the whole aircraft folder, and the plugin
is inside it. Install the plugin again afterwards. SkunkCrafts Updater
does not list it until you do.

**Before updating the Felis, back up
`747_Fly_the_Line/64/747_Fly_the_Line_settings.txt`.** It holds all your
settings, and is the one file the updater cannot restore.

## Your settings and log

`747_Fly_the_Line_settings.txt` and `747_Fly_the_Line.log` are in the `64`
folder. Updates never change them.

## Platforms

Windows, macOS and Linux. Most testing is on Windows.

Versions numbered `0.9.x` are pre-release.
