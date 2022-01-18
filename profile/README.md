# 📝 The Remnants Camp - CHANGELOG

All notable changes to this project will be documented in this file.

## [0.1.1.1] - 2022-01-18 👷‍♂️ hotfix patch

### Added

- Additional security layers were provided. Also made the server give the "🖕" response when a specific person tries to repeat the attack.

### Changed

- Try autoconnecting users **only** if Phantom wallet extension is installed and app is set to trusted
- After sending a remnant on a loot trip, Remnants "drawer" now autocloses only if there are no free remnants left
- Now displaying the number of loot keys each remnant holds, in the inventory dialog

### Fixed

- Updated walkie talkie image to reflect new stats

## [0.1.1.0] - 2022-01-15 🚧 Hotfix patch

### Added

- Added discord, twitter and whitepaper links to the navigation bar on initial screen
- Added flavor texts on items

### Changed

- Users without camps can now go to loot trips, but with a reduced loot trip chance. It's hard to loot while all alone in the wild!
- https://theremnantsnft.com prettified. Go give it some love and tell us your feedback so we can make it more attractive!
- Walkie talkie effect changed to decrease the loot trip time.
- Minor quality of life changes


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
