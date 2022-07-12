# 📝 The Remnants Camp - CHANGELOG

All notable changes to this project will be documented in this file.

## [0.7.1.0] - 2022-07-12 🍆 Weekly patch

### Added

- 24h in-game marketplace $CMP volume is now displayed in the navigation bar
- Zombies now get infected on chain faster than before. This process has been automised for the most part 🧟
- **Magic Eden API integration**. You can now visit the "Town Hall" on the map to recruit new remnants, or ditch the ones that fail at delivering proper loot! Come and test the feature with us by buying a few new recruits! 😎

### Changed

- Marketplace dialog is not closed automatically after making a purchase
- Aggregated inventory now has 3 columns on extra large screens
- "Sync Wallet" now also refreshes your bank storage

### Fixed

- Order of items in blacksmith is now fixed by item levels
- Hotkeys are now not triggered when writing down text in inputs
- Breaking an item from the bank storage now correctly updates your bank storage
- Breakdown process does not destroy gained items anymore if breakdown slot is full
- Various smaller UI/UX improvements, like fixed text overflow etc.

### Coming (relatively) soon

- Enable listing items in decimals
- Item deletion/incinerate
- Finally bringing into life discord bots that we have lying around for months... zombie infection notifications and new listings on Magic Eden
- Overhaul of resources in a way where they aren't items anymore, but a currency (like loot keys)

---

[Long period of undocumented changelog]

---

## [0.4.1.0] - 2022-03-21 🌭 Hotfix patch

### Added

- Authorization token is now automatically refreshed if user keeps visiting they app every hour or so.
- Discord notifications for infections (will stay inactive for a few more days though)
- Discord notifications for new listings (includes items the listed Remnant owns)
- Option to migrate all of your keys from one wallet to another
- Ledger support
- Our API is public and has it's first actually readable iteration. It will get even more love in the following weeks! In the following days we will also create the #DEV-talks channel for anyone interested in building plugins, browser extensions... you can check the endpoints at: https://remnants-prod-zqgkoqmdwq-uc.a.run.app/api/

### Fixed

- We have migrated from Quiknode to a public genesysgo node. Everything should work now, **but** this will be the **first time stress testing transactions on this public node**. There could be some failed transactions, but we are keeping track of all of them in our database. If gg node turns out not to be a proper solution, we will look for another one, or possibly fix our quiknode setup and rollback to it.

### Coming soon

- @Shishka will put our compensation CRON job live once he is up tonight. Which means whenever you experience a failed transactions or receive no $CMP tokens from "Claim rewards", it should be automatically compensated within 30-60 minutes.

## [0.4.0.0] - 2022-03-06 🐒 Weekly patch

### Added

- We are now subscribing to NFT transfers on the blockchain and update Remnant and Camp owners live
- "Sync wallet" button is added as a fallback which you could use to manually update your holdings (Remnants, Camps, $CMP)
- Listings search view is now live: https://camp.theremnantsnft.com/collection/remnants
- Longwood Valley Items view is now live (accessible from the crafting dialog): https://camp.theremnantsnft.com/collection/items
- If our server fails to send a transaction to you (e.g. when claiming rewards) it will automatically retry each following hour, until it succeeds

### Changed

- Transaction handling is now smarter (and faster in some cases)
- 4 loot keys are granted automatically to new players who bought from Magic Eden
- Listing on Magic Eden cancels the active loot trip and removes it from your gameplay
- Some other small UI/UX changes and improvements

### Fixed

- $CMP token value is now correctly displayed after each action (send items, buy keys, craft items)
- Loot keys are now handed out properly at midnight UTC
- Some optimizations

## [0.3.1.0] - 2022-02-24 🤯 Hotfix patch

### Changed

- There is no "Save inventory" button anymore, clicking on an item will equip/uneqip it

### Fixed

- Backpack bug fixed

## [0.3.0.0] - 2022-02-14 🥰 Weekly patch

### Added

- New Longwood Valley map (shown on homescreen)
- New inventory system
- Item crafting
- Sending items
- Buying loot keys

## [0.2.1.0] - 2022-01-27 🚀 Weekly patch

### Added

- Added option to CLAIM ALL available rewards at once. This feature is still WIP as we need to list all the items/tokens obtained
- New options in app settings: you can now enable "Advanced looting" mode which effectively skips some steps (e.g. Location Details dialog) and does some other optimizations
- Items equipped on your last loot trip are now saved so you can send your remnants on new trips faster. In the future we will also make this toggleable in app settings, and we would make it cross-device

### Changed

- Now sorting busy Remnants by the time left on loot trip
- Auto refresh the page if user changes the wallet
- Prettified the "Loot received" dialog

### Fixed

- Fixed backpack. It's working now and if you equip it, you will be able to carry 3 items along with it

## [0.2.0.1] - 2022-01-21 😶 Hotfix patch

### Added

- Added Military base! For you lucky bastards that got Bolt Cutters, you can now access the military base location

### Changed

- Optimized API calls

### Fixed

- Fixed a bug where Solana transaction couldn't be confirmed on their part, so the request would timeout and act like transaction passed

## [0.2.0.0] - 2022-01-19 😎 Weekly patch

### Added

- Added app settings. You can now change your preferences
- Added push notifications
- **Added remnant search!** By visiting https://camp.theremnantsnft.com/search you can check out the holdings of any remnant, just by typing it's token address

### Changed

- Various optimizations

### Fixed

- Fixed the API call to retrieve the number of remnants out looting

## [0.1.1.1] - 2022-01-18 👷‍♂️ Hotfix patch

### Added

- Additional security layers were provided. Also made the server give the "🖕" response when somebody tries to attack it
- Added Bolt Cutters item to the prison trip ✂

### Changed

- Try autoconnecting wallet **only** if Phantom wallet extension is installed and app is set to trusted
- After sending a remnant on a loot trip, Remnants "drawer" now autocloses only if there are no free remnants left
- Now displaying the number of loot keys each remnant holds, in the inventory dialog

### Fixed

- Updated walkie talkie image to reflect new stats
- Prettified https://theremnantsnft.com on mobile screens a bit
- Fixed countdown timer falling out of sync

## [0.1.1.0] - 2022-01-15 🚧 Hotfix patch

### Added

- Added discord, twitter and whitepaper links to the navigation bar on initial screen
- Added flavor texts on items

### Changed

- Users without camps can now go to loot trips, but with a reduced loot trip chance. It's hard to loot while all alone in the wild!
- https://theremnantsnft.com prettified. Go give it some love and tell us your feedback so we can make it more attractive!
- Walkie talkie effect changed to decrease the loot trip time.
- Minor quality of life changes
- Updated help dialog so it's easier to read

### Fixed

- Zombie-19 is running wild in the Longwood Valley. We have put restrictions in order to stop the pandemic. No zombies can come close to you within 2 meters distance. **Actually** nerfing zombies this time
- **WALKIE TALKIE + SURVIVAL GUIDE EFFECTS NOT STACKING AT THE MOMENT. Wait for our backend guy to wake up so he can sort that out. Expect a fix today or on Monday**
- Loot keys properly decremented after sending your #Remnant on a loot trip

## [0.1.0.3] - 2022-01-13 ⛺ Weekly patch

### Added

- Toggle between camps and choose your favorite!
- Displaying total amount of remnants currently looting
- Displaying the item amount (e.g. 4 binoculars)
- "Go back" functionality added to some dialogs

### Changed

- Updated website metadata. When sharing the camp.theremnantsnft.com link, cool image will show as a link preview
- Nerfing down the "go to loot animation" duration (animation is cool, but we wanna point out how fast Azure server is)
- Lots of you sillies went on loot trips without equiping any items. We are introducing a warning "toast" message when you forget to equip max amount of items!

### Fixed

- Optimized calls to the backend (50% less API calls as of now). Preparing for the bigger traffic
- Fixed a bug which occasionally made the inventory switch between different remnants

## [0.1.0.2] - 2022-01-11 🔨 Hotfix patch

### Added

- Font and (some) images are now preloaded for smoother user experience
- Dope animation is now played while sending your remnant on a trip

### Changed

- Remnants tab will now show only available Remnants
- Made Remnants tab button a bit more obvious (might as well make it bright red at this point)
- Removed wallet auto connect attempt on the initial screen for now

### Fixed

- Remnants are now sorted by name, say goodbye to random remnant order in the Remnants tab!

## [0.1.0.1] - 2022-01-08 🩹 Hotfix patch

### Changed

- Made clearer which items are selected on the equip screen
- Made the arrow to open Remnant tab clearer to see

### Fixed

- Fixed minor spacing error when showcasing large amount of Remnants
- Fixed a bug that failed to display loot timer in the homepage when claim was still available

## **[0.1.0.0]** - 2022-01-07 🐱‍👤 Alpha Release

### Added

- The Camp screen
- Loot Trips feature
