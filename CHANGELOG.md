- 1.0.0 (2024-12-01)
  * Initial version
- 1.0.1 (2024-12-01)
  * Added support for Pojav and MacOS
  * Regex filters are now limited to 1 MiB in compiled size to prevent abuse
  * Added mod logo file to jar
- 1.1.0 (2024-12-09)
  * Added integration for GregTechCEu: curvy EU cables, item and fluid pipes are automatically generated for every GTCEu material.
    They can be placed by holding the GTCEu pipe items in off-hand.
- 1.1.1 (2024-12-10)
  * Fix crash on world load caused by ID remap.
  * Fix crash on startup if items from this mod are registered after GTCEu.
- 1.1.2 (2024-12-13)
  * Energy pipes are now configurable, and will only send energy in "Extract" mode.
  * Placement preview is now transparent to avoid large pipes blocking view.
- 1.1.3 (2024-12-16)
  * Fixed translucency not working without shaders.
  * Refactored server-side ticking to prepare implementing more logistics features.
  * Slightly reduced GTCEu pipe diameter.
- 1.1.4 (2024-12-17)
  * Alleviated a lock contention issue between server thread and render thread in single player.
- 1.1.5 (2024-12-20)
  * Now compatible with GTCEu v1.6.0 (v1.5.4 will still be compatible).
- **Ported to 1.21.1** (2024-12-25)
- 1.1.6 (2024-12-29)
  * [1.21.1] Fix default recipes still using 1.20.1 tags.
- 1.1.7 (2025-01-01)
  * Fixed particle textures not randomized.
  * Fixed an edge case in GUI mouse handling.
  * Fixed default recipes IDs got mixed up.
  * [1.20.1] Fixed inconsistent shading in pipe rendering.
- **Ported to 1.12.2** (2025-01-04)
- 1.1.8 (2025-01-04)
  * [1.12.2] Fixed Java 21 (Cleanroom) compatibility.
- 1.1.9 (2025-01-04)
  * Fixed client sometimes receives pipe data from the wrong dimension.
- 1.1.10 (2025-01-05)
  * [1.12.2] Packaged per-platform native loader libraries instead of using JNA.
- **Ported to 1.7.10** (2025-01-11)
- 1.1.11 (2025-01-13)
  * [1.20.1 & 1.21.1] Fixed GregTech compat causing crash when solar panel covers are placed.
- 1.1.12 (2025-01-13)
  * [1.7.10 & 1.12.2] Fixed can't step-up stairs.
  * [1.7.10] Fixed potential crash when generating new dimension.
  * [1.7.10] Fixed when placing curvy GregTech pipes in multiplayer, normal pipes are also placed.
- 1.1.13 (2025-01-15)
  * Fixed crash caused by unexpected chunk loading caused by double-chest straddling two chunks, or similar situations.
- 1.1.14 (2025-01-16)
  * [1.12.2] Added some compatibility with OptiFine. Using OptiFine shaders may still cause issues.
- 1.1.15 (2025-01-18)
  * [1.20.1 & 1.21.1] Fixed incompatibility with Building Gadgets.
- 1.1.16 (2025-01-18)
  * [1.7.10] Do not load the GregTech integration if GT6u rather than GT5u is detected.
- 1.1.17 (2025-01-19)
  * Fixed text box cursor not blinking.
  * Optimized out some vertex format conversions that took about 37% of rendering time (measured on 1.20.1).
  * [1.12.2] Fixed GTCE being identified as GTCEu.
  * [1.12.2] Fixed incompatibility with some optimization mods.
  * [1.12.2] Now compatible with OptiFine shaders.
- 1.1.18 (2025-01-21)
  * [1.12.2] Add compat for Reach Fix mod.
- 1.1.19 (2025-01-24)
  * More rendering optimizations: reduced vertex processing time by half (measured on 1.20.1).
  * [1.12.2] Fixed more incompatibilities with optimization mods.
  * [1.7.10] Fixed damage overlay rendering at sharp angle.
- 1.2.0 (2025-02-04)
  * Optimized server-side ticking.
  * Made tick-intervals of pipes configurable. Newly placed pipes will process every 20 ticks by default, but can still be set to process every tick if needed.
  * Added tooltip to some GUI elements.
  * [1.7.10 & 1.12.2] Fixed default recipes for fluid pipe up/down conversion.
  * [1.7.10] Fixed incompatibility with the original (non-NH) NEI.
  * [1.21.1] Fixed crafter slots not being filled in the correct order.
- 1.2.1 (2025-02-06)
  * [1.20.1] Fixed crash when over-volting machines with EU cables.
  * [1.20.1] Fixed crash introduced in 1.2.0 that occurs when pipes are broken by non-players.
  * [1.20.1] Added compatibility with older versions of GTM.
- 1.2.2 (2025-02-11)
  * Optimized pipe rendering by eliminating most of CPU and bandwidth bottlenecks. It now performs about 20x better than previous versions (measured on a 1.20.1 test world).
  * [1.12.2] Fixed pipes sometimes not following light level.
  * [1.7.10] Fixed fluid filtering at passive ends sometimes not working.
- 1.2.3 (2025-02-13)
  * [1.7.10] Fixed crash introduced in 1.2.0 that occurs when item pipe from a large chest loops back onto itself.
  * [1.12.2] Fixed fluid icons in fluid filter not rendered since 1.2.0.
- 1.2.4 (2025-02-14)
  Fixed a rare client-side crash introduced in 1.2.2.
- 1.3.0 (2025-02-23)
  * Added AE2 integration: curvy variants of ME glass/covered/smart/dense covered/dense smart cables and quartz fiber.
  * Pipes now allow sharper angle between branches of pipe joints.
  * Improved GUI rendering performance.
  * Log instead of crash on unexpected chunk loading caused by multiblocks.
- 1.3.1 (2025-02-24)
  * [1.20.1] New channel overlay texture for curvy ME smart cables (already done for other MC versions in 1.3.0).
- 1.3.2 (2025-02-24)
  * [1.7.10] Now compatible with GTNH nightly as of 2/24/2025. Still works with GTNH 2.7.2.
- 1.3.3 (2025-02-25)
  * Fixed various mipmap related rendering artifacts.
- 1.3.4 (2025-02-26)
  * [1.7.10] Fixed incompatibility with the original (non-NH) AE2.
  * [1.7.10] Fixed incompatibility with ChromatiCraft.
- 1.4.0 (2025-03-11)
  * Pipe placement now allows inserting nodes into already placed pipe sections.
  * Fixed a chunk loading crash caused by AE2 integration.
- 1.4.1 (2025-03-12)
  * Fixed wrong side is connected when attaching curvy AE cable to a full block. (Already fixed in 1.4.0 for 1.7.10)
- 1.4.2 (2025-03-22)
  * Log instead of crash when cross-mod integration fails to load.
- 1.4.3 (2025-03-23)
  * [1.7.10] Fixed incompatibility with Backhand 1.6.11.
- 1.5.0 (2025-03-30)
  * Added radial menu for editing existing nodes. Existing nodes can now be moved or deleted. By inserting / moving / deleting nodes, curve shape of already placed pipes can be freely edited without needing to break the pipes.
- 1.5.1 (2025-03-30)
  * [1.20.1 & 1.21.1] Fixed some client-side curve validity checks not applied.
  * [1.20.1 & 1.21.1] Fixed radial menu input on high DPI screen.
- 1.5.2 (2025-03-30)
  * [1.7.10 & 1.12.2] Fixed radial menu not rendering on some GPU
  * Fixed a potential crash running on Apple Silicon
- 1.5.3 (2025-04-04)
  * [1.7.10] Fixed GT integration with the new GT5u version that renamed `getThickNess`.
- 1.6.0 (2025-04-06)
  * Pipes can now be harvested directly into inventory by using other mods' wrenches.
  * Drops from breaking pipes now have the standard pickup delay.
  * Breaking pipes in creative mode no longer drops items.
  * [1.20.1] Updated GT integration for an upcoming GTM change that will break it.
  * [1.20.1 & 1.21.1] Now compatible with Radium's entity collision optimization.
- 1.7.0 (2025-04-08)
  * Changed to a more permissive algorithm for checking pipe intersection.
  * Branch angle limit now has its own error message rather than showing "pipes can't intersect".
  * When placement fails due to intersection, the location of the intersection will be indicated.
  * Holding sprint now also prevents targeting nodes.
- 1.7.1 (2025-04-08)
  * Fixed intersection marker being placed too far away when branches are almost collinear.
- 1.7.2 (2025-04-27)
  * [1.21.1] Fixed pipe items sometimes not rendering or functioning due to a client/server desync.
- 1.8.0 (2025-04-28)
  * Added an optional grid system that helps aligning pipes to regularly spaced points. It can be enabled by middle-clicking empty space.
- 1.8.1 (2025-05-12)
  * [1.7.10 & 1.12.2] Fixed overlay rendering on AMD cards.
  * Rewrote some immediate mode rendering code to use avx2 or avx512 if available.
- 1.8.2 (2025-05-21)
  * Grid no longer shows points that are inside existing pipes.
  * [1.12.2] Fixed AE2 integration causing "AE2 Stuff" tile data to not load.
  * [1.7.10 & 1.12.2] Fixed some issues with non-English lang display & regex filtering.
- 1.8.3 (2025-05-26)
  * Added 2 more grid patterns.
  * Grid pattern can now be cycled backwards by holding sneak.
- 1.8.4 (2025-05-31)
  * Grid pattern is now cycled on any failed pick block in additional to aiming at air (so that it plays nicer with Quark's long-range pick block feature).
- 1.8.5 (2025-06-03)
  * Fixed another crash caused by reentrant chunk loading.
- 1.8.6 (2025-06-04)
  * Fixed energy pipes sometimes don't transfer at full rate into GTM energy converter (and other machines that handle energy in a similar way).
- 1.8.7 (2025-06-08)
  * Fluid pipes now work with vanilla cauldrons.
- 1.9.0 (2025-06-16)
  * Fluid pipes can now regulate fluid amount (both per-type and total), similar to item pipes.
- 1.9.1 (2025-06-22)
  * Item pipes now fill inventory slots in the forward order.
  * [1.7.10] Fixed curvy GT++ pipes missing textures.
- 1.10.0 (2025-06-27)
  * Added "Force Joint" to the node menu, which allows creating sharp corners without needing to create a branch.
- 1.10.1 (2025-07-01)
  * [1.20.1 & 1.21.1] Added support for FreeBSD.
- 1.11.0 (2025-07-08)
  * Pipe ends that are attached to blocks can now be moved using the curve editing radial menu: you can now either reattach a pipe to another block while preserving its configurations, or detach a pipe from block.
  * Adjusted the texture mapping of pipe joints.
- 1.11.1 (2025-07-11)
  * Fixed a rare case where pipes in a chunk won't tick if the chunk got loaded too early.
  * Fixed pipes sometimes fade out into sky's color as if they're near render distance.
- 1.11.2 (2025-07-12)
  * [1.12.2] Fixed glitchy HUD rendering when StellarCore's HUD caching is enabled.
  * [1.20.1] Fixed pipes sometimes don't render when Cosmic Horizons is installed.
- 1.11.3 (2025-07-16)
  * AE2 integration changes: now allows attaching cables to the lateral sides of parts (buses & terminals) rather than just the back sides of them.
  * Fixed pipes can't attach to some oddly shaped blocks.
  * Grid patterns now exclude points that are too close to blocks, to prevent accidentally placing pipes touching a block but not actually attached to it.
- 1.11.4 (2025-07-17)
  * Adjusted the visibility threshold of grid pattern points.
- 1.11.5 (2025-07-17)
  * [1.20.1] Fixed pipes sometimes don't have shader shadows since version 1.11.2.
- 1.11.6 (2025-07-19)
  * [1.21.1] Fixed crash after updating to NeoForge version 21.1.193.
- 1.11.7 (2025-07-25)
  * [1.7.10] Better compatibility with shaders on 1.7.10.
- 1.12.0 (2025-08-03)
  * New textures for all the pipes. Note that the UV mappings changed, so existing custom textures will no longer work. Existing custom configs also need to be updated to use the new texture names (tiny/small/huge pipe variants now have their own sprites).
- 1.12.1 (2025-08-05)
  * Adjusted the hue of the new item pipe textures.
  * Added a section to the config file for automatically generating pipe up/down conversion recipes.
- **Ported to 1.16.5** (2025-08-14)
  * Including integration with AE2, and compat with JEI, REI and Iris (Oculus)
- 1.12.3 (2025-08-21)
  * Fixed pipe breaking particle mapped incorrectly since version 1.12.0
  * Slightly increased the scale of pipe items in GUI.
- 1.12.4 (2025-08-21)
  * Fixed crash at startup on Linux since the last update.
- 1.12.5 (2025-08-22)
  * [1.21.1] Workaround for a Scena (from Chisels & Bits) issue (https://github.com/Communi-Suggestu/Scena/issues/8) that's causing crash with Curvy Pipes.
- 1.12.6 (2025-08-25)
  * Fixed crash caused by an edge case in pipe graph topology.
- 1.12.7 (2025-08-27)
  * [1.7.10] Fixed incompatibility with the new Backhand version.
- 1.13.0 (2025-09-18)
  * Added redstone cable that conducts weak redstone signal just like vanilla redstone wires, but uses Curvy Pipes' grid-free system.
  * Middle-click now prefers selecting grid pattern over picking blocks (no longer need to aim at empty space).
- 1.13.1 (2025-09-20)
  * Fixed crash introduced in 1.13.0 that happens when extraction or insertion causes block update.
  * [1.12.2 & 1.7.10] Fixed pipes not attaching to Forestry blocks.
  * [1.12.2] Fixed connecting curvy to normal dense ME cable causes its bounding box method to throw.
  * [1.12.2] Fixed curvy pipe items missing from creative tab search tab.
  * [1.7.10] Fixed incompatibility with Beddium.
- 1.13.2 (2025-09-21)
  * [1.21.1] Fixed the redstone cable not having a recipe.
- 1.13.3 (2025-09-27)
  * Fixed some markings in curve editing HUD aren't showing when looked from certain angles.
  * Fixed destroying curvy AE cables sometimes causes crash since 1.13.0
  * [1.7.10] Fixed incompat with FluidLogged
- 1.13.4 (2025-10-01)
  * [1.21.1] Fixed incompat with the "Roots" mod's HUD rendering.
- **Ported to 1.18.2** (2025-10-12)
  * Including integration with AE2, and compat with JEI, REI and Iris (Oculus)
- 1.13.5 (2025-11-20)
  * A large amount of code (rendering, physics and ticking) has been refactored since the last version. Please reach out if you're seeing any new bugs or perf regressions.
  * [1.7.10] Fixed pipes not attaching to some blocks from NTM since 1.11.3.
  * [1.16.5 - 1.20.1] Item pipes now support vanilla composter (1.21.1 NeoForge has this built in).
  * [1.16.5 - 1.18.2] Fixed pipe data sometimes not synced to player after teleport.
  * All modes of transfer now prefer closer destination in additional to paths with higher throughput.
  * Fixed inserting into StorageDrawers sometimes voids excess items.
- 1.14.0 (2026-02-24)
  * Item pipes can now be made transparent by right-clicking with glass. Items still transfer instantly: the traveling items displayed in-world only serve as a visual indication of past transfers. Item rendering is currently unoptimized so do not overuse transparency.
  * Added more detailed tooltips for pipe items. Item transfer rate now shows in per-second rather than per-tick.
  * Fixed regex not accepting dot wildcards.
  * Optimized curve shape preview.
  * [1.20.1] GT integration now works with GTM v7.5.0. Still compatible with older GTM versions.
  * [1.7.10] GT integration now works with GT5u 5.09.52.392. Still compatible with older GT5u versions.
  * [1.7.10] Fixed incompat with ShoulderSurfing.
  * [1.7.10] Fixed incompat with recent Angelica versions.
  * [1.12.2] Fixed pipes not preventing blocks from being placed over them.
- 1.14.1 (2026-03-18)
  * Fixed items entering transparent item pipes that are partially outside render distance causing client hang.
- 1.14.2 (2026-04-04)
  * [1.12.2] Fixed traveling items being rendered twice.
- 1.15.0 (2026-04-09)
  * Added CC: Tweaked (ComputerCraft) integration (curvy networking cable).
- 1.15.1 (2026-04-12)
  * [1.12.2] Fixed redstone cable not powering opaque blocks when FluidLoggedAPI is installed.
