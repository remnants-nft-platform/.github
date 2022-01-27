# 📝 The Remnants Camp - CHANGELOG

All notable changes to this project will be documented in this file.

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

- Backpack is now working and if you equip it, you will be able to carry 3 items along with it
- Various bugfixes are resolved. e.g. when "Loot received" dialog wouldn't show up

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
