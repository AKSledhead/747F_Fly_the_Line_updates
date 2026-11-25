# 747 Fly the Line — Freighter — updates

Updates for **747 Fly the Line**, a first officer and flight engineer for
the Felis Boeing 747-200 freighter in X-Plane 12. SkunkCrafts Updater
downloads them from here.

**This is for the freighter, `747F_Felis`, only.** The Felis passenger
747-200 is a separate aircraft and is not supported yet. It will have its
own updates when it is.

This repository holds the released plugin only, not its source.

## Where it installs

In X-Plane's own plugins folder:

```
X-Plane 12/Resources/plugins/747_Fly_the_Line/
```

X-Plane loads it with every aircraft, but it stays hidden and does nothing
outside the Felis 747. Its menu appears when the Felis loads.

**Moving from an older install?** Older versions lived in
`X-Plane 12/Aircraft/747F_Felis/plugins/747_Fly_the_Line/`. Load the
freighter once with the new copy, which brings your settings across, then
quit X-Plane and delete that old folder.

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

## Your settings and log

`747_Fly_the_Line_settings.txt` and `747_Fly_the_Line.log` are in the `64`
folder. Updates never change them.

## Platforms

Windows, macOS and Linux. Most testing is on Windows.

Versions numbered `0.9.x` are pre-release.
