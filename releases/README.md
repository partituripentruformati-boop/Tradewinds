# Tradewinds test patches

Use [Black Dragon v5](Tradewinds_BlackDragon_TEST_v5.zip) for the dragon artwork, shipyard catalog and maximum-cannon button. Install both the executable and TW1_00.data in the original game folder.

**V4 has a disappearing-ship bug; use v5 instead.** V5 selects artwork only in display objects and preserves the native ship type pointer used to group the fleet. It also converts transparency masks to the original indexed PNG format.

V5 passed 78 x86 emulation, archive and graphics checks. These include reproducing the v4 bug in the native fleet grouping routine and confirming v5 keeps the ship after repeated display refreshes. Full Windows gameplay and rendering still need in-game testing.

Back up all saves before installing. If Black Dragon is absent after loading, try a save from before the v4 disappearance. No save files are modified by this package.
