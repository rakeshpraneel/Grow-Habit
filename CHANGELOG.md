# Changelog

Change tracker for Grow Habit

## [V2.0.2] - 2026-04-25

> Description
> Grow Habit comes up with few new features and some major UI updates.

### New Features
* Included alarm edit feature and timer item to perform it.
* Included alarm item to inventory, store and scratch card reward.
* Updated share icon for enhanced UI.
* Improved UI.

### Bug Fixes
* Glitch with starter task and habit is fixed.
* In App update notification bug fixed.(need to check once prod deployment is done)
* Added haptic feel for task page.
* Updated all plants to carrot.

## [V2.0.1] - 2026-03-26

> Description
> Grow Habit comes up with few new features mostly on UX part and with some major security patches.

### New Features
* Starter task and habit for new users.
* Enhanced journal page.
* Added share your status option with social media integration.

### Bug Fixes
* Fixed Sound notification to timer based task.

## [V2.0.0] - 2026-02-09

> Description
> Grow Habit comes up with few new features mostly on UX part and with some major security patches.

### New Features
* Improved feedback.
* More Interactable.
* New Sound Notifications.

### Bug Fixes
* Security Update.
* Manual Volume control using media volume.
* Alarm can be silenced.
[V2.0.0] - 

## [V1.0.0] - 2025-11-06
### Added
- Initial production release of Grow Habit
- Core features:
-	This gives you a real time visualization of how far you have progressed on your goals.
-	User can create fully customizable goals as per their plan, they can be created either as task or habit.
-	Task is a onetime activity whereas habit helps to stack the daily activity. These can even be categorized based on time or simple mark as done.
-	The habits created will be converted into plants and planted in garden where user can visually see the progress they make on completing them on daily basis.
-	These can be marked as completed for the day by watering which in turn helps in growing them.
-	Plants health will reduce when you miss watering them, this varies based on plant’s level which in turn reflects how strong a user can return back to the goal even if it is left in between.
-	It also comes with Do not bother mode, which can be toggled while creating the habit, this enables a strict mode so that user won’t be able to switch apps while performing those activities.
-	Completing multiple task helps you to earn rewards which can be used to play with garden.
-	User can buy items such us shovels and potions from store using in app coins. Same can be obtained from the scratch cards earned when completing multiple task.
-	Based on the persistency the plant will grow and user can gain level such as newbie, pro, chamber and master.
-	User can also maintain streak and thereby can achieve badges based on that.

### Changed
- Show watch video option whenever user runs out of items.
- Change the message shown in dialog box when timer is completed.
- Adding habit reminder feature.
  - User won't be able to set multiple alarm at same time.
  - Whatever be the target days, all habits which have reminder configured, it will be set for first 7 days and will be renewed on basis on how user water's it.
  - If user doesn't water for 7 days then there won't be any alarm in place, it will be renewed only when user again water's it.
- Added notification manager to send out timer status of habits when the application is minimised.
- Added notification feature to intimate user when a timer is completed.
- User will get scratch card reward after achieving master status in any habit.

### Fixed
- There was bug with custom target days and custom timer, it was defaulted to 30 days and 25 minutes when user enables it but in UI selector it was showing 14 days and 20 mins
  - This is now updated to 14 days and 25 mins.
- When dead plant is revived the water icon was still visible in the task page, but in garden page it was showing plant is already watered.
  - This has been fixed now, watering option will be enabled both in garden and task page after reviving plant.
- Fixed timer issue -> timer wasn't properly running when device is locked or app is minimised, updated the counter logic to calculate the remaining time
  based on the last recorded time while app was paused/minimised.
- UI will be refreshed whenever app is resumed from sleep.
- Included flag so that user won't be able to delete plant from garden when the timer runs.
- Seperate messages will be shown for unavailability of shovel and active timer.
- Plant is not growing in garden page but its level is changing in journal page. ---> Issue fixed, updated level names were not in sync with slot manager module.
- Level was not updating properly when watered from garden page. ---> Issue fixed, Now post watering, garden display will call update method from task page.
  - Added fallback message if in case this fails, so that user can water from journal page.

### Tracker
-   Current version (27) V1.0.0
-   Closed testing stable version - (26) V1.0.0
[V1.0.0]: https://github.com/rakeshpraneel/Task-Manager/releases/tag/v1.0.0.15
testing******
