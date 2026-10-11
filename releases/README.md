# Tradewinds test patches

Use [Regional Goods v8](Tradewinds_RegionalGoods_TEST_v8.zip) to add Tea (Tanchon only), Spices (Lama Sut only), and Jade & Gemstones (Edamame only), with fluctuating prices and sales in every port. The new rows use the supplied designs and include quantity entry, Buy/Sell and Max buttons, plus warehouse Load all / Store all controls. All previous v7 shipyard, Black Dragon, cannon and warehouse changes are included.

Close the game and back up every save first. Install BOTH the executable and TW1_00.data from v8 in the original game folder, alongside its DLLs and TW1_01.data. Keep matching patch files together. To roll back, restore earlier patch files and a pre-v8 save: older executables cannot preserve the three added inventories when saving.

V8 passed 94 regression checks on the integrated executable, 16 native bridge/hook integration tests and nine x86 core tests. Engine services are stubbed; full Windows gameplay and rendering still require in-game verification. Read the ZIP's README for installation and suggested checks.

## Earlier builds

Use [Black Dragon v7](Tradewinds_BlackDragon_TEST_v7.zip) for 15,000-unit warehouses, a repair-price button that fits its frame, the enlarged combat sprite, Black Dragon 450 cargo / 45 cannons, and Junk 50 cargo / five cannons. It includes the shipyard catalog, restocking and maximum-cannon button. Cannons still require ten free cargo units and enough gold each.

Install both the executable and TW1_00.data in the original game folder. Back up all saves first. Black Dragon is a manager-registered type in v7 saves; keep the matching v7 data, or restore a pre-v7 save when rolling back.

**V4 has a disappearing-ship bug; use v7 instead.** V6 preserves native fleet grouping by using the registered type returned by the game manager, and retains indexed PNG transparency masks from v5.

V6 passed 94 x86 emulation, archive, layout and graphics checks, including native regrouping, capacity purchases and enlarged frame anchors. Full Windows gameplay and rendering still require in-game verification.
