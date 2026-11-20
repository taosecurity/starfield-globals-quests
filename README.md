# Starfield Globals and Quests

This page lists every global variable and every quest in Starfield and its official add-ons. It gives their IDs, starting values and quest stages, with console commands ready to copy. The list was read from the game files (game version 1.16.244.0).

**View it here:** https://taosecurity.github.io/starfield-globals-quests/

## Example

1. Open the page and type `GameHour` in the search box.
2. The row for the global `GameHour` (Form ID `00000038`) says it is "the hour on the game clock" and that it starts at 8. It also lists the quest `MQ101` among those that use it.
3. Click the command `set GameHour to 8` to copy it.
4. In the game, press ~ (PC only), paste the command, change the 8 to the hour you want, such as 20, and press Enter.

The game clock jumps to that hour, so `set GameHour to 20` makes it evening. Click `getglobalvalue GameHour` instead to see the current hour.

## Using the console

On PC, press the **~** key (the key under Esc) to open the console, type or paste the command, and press Enter. Xbox and PlayStation have no console. Using the console turns off achievements for that save unless you use a mod that keeps them on.

## What's on the page

- The page lists 3,711 global variables. Each one shows its starting value, whether the game marks it constant, and which quests use it. Click a quest to jump to it.
- The page lists 2,727 quests, from the main story to the background quests that run companions and encounters. Each quest opens to show its stages (20,688 in all) with the developers' own note on each, and which stages complete or fail the quest.
- Every global and quest has console commands you can copy: `getglobalvalue`, `set ... to ...`, `getstage`, `setstage`, `sqs`, `startquest`, `completequest` and `resetquest`.
- The top of the page explains in plain language what globals and quests are, how players and modders can use the list, and what to watch out for before changing anything.

What's new: see the top of the [live page](https://taosecurity.github.io/starfield-globals-quests/).

## Words used here

- **Console:** the PC command line inside the game, opened with ~.
- **Global variable (global):** a named value that any quest, script or condition can read, such as `GameHour`.
- **Quest stage:** a numbered step in a quest. `setstage` moves a quest to a stage and runs that stage's script.
- **Plugin:** a mod's data file (`.esm`, `.esp` or `.esl`). It adds or changes records in the game. Each add-on is a plugin too.
- **Record:** one thing in a plugin, such as a weapon, a quest, a location or a setting.
- **Form ID:** a record's number, such as `00000038`. The first two digits depend on the load order.
- **Editor ID:** a record's readable name, such as `GameHour`, used by the Creation Kit and xEdit.
- **Load order prefix:** the first digits of a Form ID, which say which plugin the record comes from. Base game records start with `00`; an add-on's prefix depends on where it loads in your game.
- **Light plugin:** a plugin flagged to use a small slot, so it doesn't count toward the limit of about 250 full plugins. The console often can't find a light plugin's quests and globals by Editor ID, so use the Form ID for those.

## How it was made

- The globals, quests and stage notes were read from the game files, game version 1.16.244.0.
- The page shows names, IDs, values and the developers' stage notes from the game files. It contains no game code.
- The console commands were not tried in the game one by one. Save first before changing quests or globals.
- The list is regenerated after game updates.

## Thanks

Thank you to Reddit user Aggravating-Bee4846 for asking about global and quest IDs, which led to this page.

## Found a mistake?

Open an issue: https://github.com/taosecurity/starfield-globals-quests/issues

## Credits and license

Richard Bejtlich of [Richard Presents Starfield Essentials](https://www.youtube.com/@RichardBejtlich) made this page. More Starfield tools and references are on the [Richard Presents Development Hub](https://taosecurity.github.io/).

This is an unofficial list, not made or endorsed by Bethesda. Starfield is a trademark of ZeniMax Media.

The page is a single self-contained `index.html` with no external dependencies. Its code (layout and search) is under the MIT license; see [LICENSE](LICENSE).
