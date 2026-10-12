# Tradewinds test patches

**Latest test: [v22 — Spices](Tradewinds_Spices_TEST_v22.zip).** Adds Spices buying only in Lama Sut, selling anywhere, fluctuating prices, shared market/warehouse controls, supplied icon and a global paid-round hint. Tea and all prior upgrades remain; Jade disabled. Includes the confirmed v21.1 selection fix and Tea-only save migration. Replace both files and back up saves. Regression/integration checks passed; Windows gameplay pending.

**Latest repair: [v21.1 — market purchases](Tradewinds_MarketFix_TEST_v21_1.zip).** Fixes Tea refresh discarding the original four selected quantities before Buy/Sell. Skips empty Tea trades and restores original selections after mixed trades. All v21 features/data/save format retained; Spices remains paused and is excluded. Replace both files and test a small original commodity purchase. Regression reproduces failures on v21 and passes on this fix; existing checks passed. Windows trade confirmation pending.

**Latest: [v21 — Tea warehouse layout, icon and alehouse tip](Tradewinds_TeaWarehouse_TEST_v21.zip).** Market note replaced with a random paid-round tip in all alehouses; Tea icon enlarged to 24px; warehouses align Tea Value/Qty and include lower quantity controls using the normal Transfer button. All previous features retained. Replace both files and back up saves. 94 regressions, 18 Tea, eight Fair Wind, eight diagnostic, five market and four warehouse checks passed; source rebuild matches exactly. Windows gameplay/rendering pending.

**Latest: [v19 — clean marketplaces in all ports](Tradewinds_CleanMarkets_TEST_v19.zip).** Removes the upper Tea shortcut row, shortens the panel and retains a 20-pixel gap to Buy/Sell/Leave. Tea trades through the lower window and still buys only in Tanchon. Shared UI applies everywhere. Only the UI resource changes; EXE is identical to v18 and logs still say v18. Replace both files. 94 regressions and five lower Tea tests passed; Windows rendering pending.

**Latest: [v18 — Tea in the lower Buy/Sell window](Tradewinds_TeaTrade_TEST_v18.zip).** Tea has a lower quantity row with minus/plus/Max, participates in main Buy/Sell and Sell All, and remains second in both lists. Includes v17 spacing and all ship upgrades. No new command registrations. Replace BOTH files; back up saves. 94 regressions, 18 Tea integration tests, eight Fair Wind, eight diagnostic checks and five lower-trade tests passed. Windows playtest pending.

**Latest layout: [v17 — Tea market layout](Tradewinds_TeaLayout_TEST_v17.zip).** Tea sits between General Merchandise and Arms. Item rows evenly spaced; Tea controls have their own wider row below Dream Dust; Buy/Sell/Leave and native trade window move lower. Tea still buys only in Tanchon. Only one UI resource changes; EXE is identical to v16 and logs still say v16. Replace both files. 94 regressions and Tea command-binding check passed; Windows rendering pending.

**Latest test: [v16 — Tea only](Tradewinds_TeaOnly_TEST_v16.zip).** Tea buys exclusively in Tanchon, sells elsewhere, fluctuates in price and supports warehouse/save inventory. Spices/Jade remain disabled. Reuses an existing command instead of adding global command registrations; fleet initialization guarded. All ship upgrades retained. Back up v15 files and saves; replace both patch files. Test startup, Tea buying/selling, warehouse transfer and save/reload; send the v16 startup log if it crashes. 94 regressions, 18 Tea integration checks, eight Fair Wind and eight diagnostic checks passed. Windows playtest pending.

**Current isolation test: [v15 — new commodities disabled](Tradewinds_NoRegionalGoods_TEST_v15.zip).** Restores v7 native market/warehouse code and UI while retaining Black Dragon, Fair Wind and all shipyard/warehouse upgrades. Startup logging retained. Back up saves, replace both patch files and report whether Constructing buildings completes; send the v15 log if it still crashes. Saving in this test drops inventories of the three disabled goods. 94 regressions, eight diagnostic checks and four Fair Wind checks passed. Windows startup pending.

**Latest diagnostic: [v14](Tradewinds_StartupDiagnostic_TEST_v14.zip).** V13 reached all constructor entry points but did not identify the failing caller. V14 corrects access-violation parameter logging and adds thread IDs, mapped DLL names and a longer bounded stack trace. All gameplay/data remain unchanged. This is a diagnostic build, not a confirmed fix. Replace both patch files and send the v14 startup log. 94 regressions and eight diagnostic checks passed.

**Current crash investigation: [v13 diagnostic](Tradewinds_StartupDiagnostic_TEST_v13.zip).** The v12 report confirms UI loading completed before an access violation in a Windows library. V13 adds building-constructor markers and the exception register/stack details needed to identify the caller. Gameplay/data remain unchanged. Replace both files, run, and send the new `Tradewinds-startup.log` (first line must say v13). This is not a confirmed Windows crash fix. 94 regressions and eight diagnostic checks passed; all 11 building constructor markers were also exercised by real Wine/QEMU startup.

**Building-loading crash investigation: [v12 diagnostic](Tradewinds_StartupDiagnostic_TEST_v12.zip).** It keeps v11 resources/gameplay and adds a local `Tradewinds-startup.log`. Replace both files, run the game, and send that log if it closes. This is not a confirmed Windows crash fix. All 94 regressions and five logging checks passed; real building/port UI loading also completed under Wine/QEMU. That runner later encountered a graphics-mode failure.

**Use [Fair Wind v11](Tradewinds_FairWind_TEST_v11.zip).** It corrects the XML declarations that produced multiple startup alerts such as `assets/xml/ships.txt: quoted string expecting ..., line 0`. All four affected XML files are corrected. V10's Windows executable-layout fix and all prior ship/economic features are retained.

Close the game, back up saves, and replace BOTH the executable and TW1_00.data in the original game folder alongside its DLLs and TW1_01.data. The EXE matches v10 exactly; only the four serializer headers were removed from the data archive.

Five XML-format regression checks and 94 existing gameplay/artwork/layout checks passed. Native engine services are stubbed; full Windows startup/rendering requires in-game testing. V8, v8.1, v9 and v10 are superseded.

## Superseded packages

**V8 and v9 contain an executable-layout defect that can cause Windows to show "This app can’t run on your PC". Use the corrected packages below.**

Use [Fair Wind v10](Tradewinds_FairWind_TEST_v10.zip) for the latest changes, including Fair Wind art, 250 cargo / 25 cannons / 60 maximum hull and all regional economic features. For just the v8 feature set, use [Regional Goods v8.1](Tradewinds_RegionalGoods_TEST_v8_1.zip).

These packages correct the virtual-section gap in the EXE without changing game code or data. Layout regression checks reproduce the old defect and validate the repaired image. V10 also passes 94 gameplay regression checks, 16 regional tests and eight Fair Wind tests. Actual Windows launch/gameplay still requires testing.

Close the game, back up saves, and copy BOTH EXE and TW1_00.data into the original game folder alongside its DLLs and TW1_01.data. Keep matching versions together.

## Superseded packages

Use [Fair Wind v9](Tradewinds_FairWind_TEST_v9.zip) for Douglas McGowan's blue-and-gold ship artwork, 250 cargo / 25-cannon maximum and 60 maximum hull. Combat frames are 95×72, between the ordinary one-master (87×72) and two-master (103×72). It includes all regional goods and previous patch features.

Back up saves, then install BOTH the executable and TW1_00.data in the original game folder. V9 saves require matching v9 data. Existing Fair Wind ships upgrade once and preserve damage proportion; ordinary sloops stay unchanged.

V9 passed 94 prior regression checks, 16 regional integration tests, eight Fair Wind tests and nine x86 core tests. Windows gameplay/rendering still needs in-game verification.

Use [Regional Goods v8](Tradewinds_RegionalGoods_TEST_v8.zip) to add Tea (Tanchon only), Spices (Lama Sut only), and Jade & Gemstones (Edamame only), with fluctuating prices and sales in every port. The new rows use the supplied designs and include quantity entry, Buy/Sell and Max buttons, plus warehouse Load all / Store all controls. All previous v7 shipyard, Black Dragon, cannon and warehouse changes are included.

Close the game and back up every save first. Install BOTH the executable and TW1_00.data from v8 in the original game folder, alongside its DLLs and TW1_01.data. Keep matching patch files together. To roll back, restore earlier patch files and a pre-v8 save: older executables cannot preserve the three added inventories when saving.

V8 passed 94 regression checks on the integrated executable, 16 native bridge/hook integration tests and nine x86 core tests. Engine services are stubbed; full Windows gameplay and rendering still require in-game verification. Read the ZIP's README for installation and suggested checks.

## Earlier builds

Use [Black Dragon v7](Tradewinds_BlackDragon_TEST_v7.zip) for 15,000-unit warehouses, a repair-price button that fits its frame, the enlarged combat sprite, Black Dragon 450 cargo / 45 cannons, and Junk 50 cargo / five cannons. It includes the shipyard catalog, restocking and maximum-cannon button. Cannons still require ten free cargo units and enough gold each.

Install both the executable and TW1_00.data in the original game folder. Back up all saves first. Black Dragon is a manager-registered type in v7 saves; keep the matching v7 data, or restore a pre-v7 save when rolling back.

**V4 has a disappearing-ship bug; use v7 instead.** V6 preserves native fleet grouping by using the registered type returned by the game manager, and retains indexed PNG transparency masks from v5.

V6 passed 94 x86 emulation, archive, layout and graphics checks, including native regrouping, capacity purchases and enlarged frame anchors. Full Windows gameplay and rendering still require in-game verification.
