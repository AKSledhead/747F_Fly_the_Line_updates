# 747 Fly the Line — Freighter — updates

The SkunkCrafts Updater depot for **747 Fly the Line**, a plugin that flies
the First Officer and Flight Engineer of the Felis Boeing 747-200 in
X-Plane 12.

**This depot is for the FREIGHTER, `747F_Felis`.** The Felis passenger
747-200 is a separate aeroplane and will have its own build and its own
depot; this one will not drive it. Nothing here is wired to the passenger
airframe yet.

This repository holds released binaries only. It is not the source.

## Where it installs

Inside the aircraft, not in `Resources/plugins`:

```
X-Plane 12/Aircraft/747F_Felis/plugins/747_Fly_the_Line/64/win.xpl
```

That location is deliberate — X-Plane loads a plugin kept in an aircraft's
own `plugins` folder only when that aircraft is loaded, so the plugin costs
nothing in every other aeroplane.

**Never leave a second copy in `Resources/plugins`.** X-Plane does not
de-duplicate plugins, so a stray global copy means the Felis loads both:
two flight loops, two stage machines, doubled callouts. If anything happens
twice, look for a second `.xpl` before anything else.

## Disable similar add-ons

This plugin's first officer and flight engineer work their own panels: the
fuel panel, the electrics, the pneumatics, the lights. **Any other add-on
that does the same job must be disabled for the Felis**, or the two will
fight over the same switches — one sets a crossfeed, the other sets it back.

That includes automatic fuel management scripts, XFirstOfficer, and any
other first officer or flight engineer add-on for this aircraft.

## The crew's voices

The voices ship in this depot, in `voice/<accent>/`, and the updater keeps
them current along with the plugin. Three accents: `US`, `UK` and `EU`.
Delete a folder you don't want and it disappears from the plugin's list;
the next update puts it back.

## A Felis update will remove this plugin

Aircraft updates often replace the whole aircraft folder, and this plugin
lives inside it. After updating the Felis you will need to reinstall, and
SkunkCrafts will not see the add-on until you do — its `skunkcrafts_updater.cfg`
is removed along with everything else.

**Back up `64/747_Fly_the_Line_settings.txt` before updating the aeroplane**,
or every preference returns to its default. That one small file is the only
thing the updater cannot give you back.

## Your own files are left alone

`747_Fly_the_Line_settings.txt` and `747_Fly_the_Line.log` sit beside the
`.xpl`. Neither is managed by the updater — both are named in
`skunkcrafts_updater_blacklist.txt` so an update cannot overwrite your
settings.

## Platforms

Windows is developed and flown on. macOS and Linux are built by CI.

Anything in this repo at a `0.9.x` version is pre-release.
