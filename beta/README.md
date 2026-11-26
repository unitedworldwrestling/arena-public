# UWWtiming 2.0 — beta

**Version 2.0.0.34**, 26 November 2026. Signed installer: `UWWtimingSetup_2.0.0.34.msi`
(SHA1 `EAC8754EA3DAC99C32C42B0D346A942CAF33969A`).

This is a **beta**: it is **not** distributed by the automatic update. Scoreboards stay on the official version
(1.3.20.231) until this version is installed by hand. The official 2.0 versions will follow.

## What is new

- New design of the operator screens: PC screen, tablet mode, menu and every window, in the dark UWW design. The
  screens grow with the window and stay readable on any screen size; no scroll bar.
- The current period is highlighted (Round 1, Break, Round 2, Overtime…), and the break stays visible between two
  rounds.
- MMA and pankration: judges' scorecards in a table (J1, J2, J3 × rounds, overtime, total), a highlighted cell when a
  judge's scorecard has no winner, and a dedicated layout in tablet mode.
- End of match: victory types readable whatever their number and length.
- Public scoreboard: logo full now works in MMA and belt wrestling; an empty match switches the public screen to the
  waiting screen.
- Empty match for every sport: Matches > Empty match settings… (sport, age, weight category); Load Empty Match then
  loads it at once, with the rounds, times, points and victory types of the Arena configuration. The configuration is
  refreshed from Arena at start-up when Arena can be reached.
- Judges are written J1, J2, J3.
- New UDP request for broadcast graphics: `status` (match loaded, started, time over, result confirmed, accepted by
  Arena). Existing UDP messages are unchanged.

## Install

Run the installer on the scoreboard PC; it replaces the installed version.

## Go back to the official version

Uninstall UWWtiming, then install `../UWWtimingSetup_1.3.20.231.msi`.
