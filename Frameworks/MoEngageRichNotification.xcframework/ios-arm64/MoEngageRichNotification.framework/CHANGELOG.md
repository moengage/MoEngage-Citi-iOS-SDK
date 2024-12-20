# MoEngageRichNotification
===========================

## Change Log:
### Version 7.16.1 *(12th June 2024)*
-------------------------------------------
* Handled environment update with same installation.

### Version 7.16.0 *(8th April 2024)*
-------------------------------------------
* Handled UserDefault storage limit

### Version 7.15.0 *(27th February 2024)*
-------------------------------------------
* Refactored network layer.
* Refactored data tracking.
* Refactored logging.
* BugFix - Fixed threading issue when downloading the resources.

### Version 7.14.1 *(7th February 2024)*
-------------------------------------------
* BugFix - Fixed the unnecessary new line rendering.

### Version 7.14.0 *(23rd January 2024)*
-------------------------------------------
* Added privacy manifest file
* Added Code signature support for XCFrameworks.

### Version 7.13.0 *(30th November 2023)*
-------------------------------------------
* Updated hashing algorithm usages to SHA256.

### Version 7.12.0 *(15th November 2023)*
-------------------------------------------
* Added notification impression and click API.
* BugFix - Refactored public APIs that can cause name collision.

### Version 7.11.1 *(26th September 2023)*
-------------------------------------------
* BugFix - MOEN-26967: Fixed `setImage` and `setGIF*` extension methods name collision.
* BugFix - MOEN-27001: Fixed invalid gif data not falling back to static image.
* BugFix - MOEN-27000: Fixed gif getting duplicated in carousal.
* Updated the dependency to MoEngage-iOS-SDK 9.12.0.

### Version 7.11.0 *(30th August 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.11.0.
* Internal Code Optimization

### Version 7.10.0 *(18th July 2023)*
-------------------------------------------
* iOS breakpoint issue fix by changing the config settings.

### Version 7.9.0 *(20th June 2023)*
-------------------------------------------
* iOS breakpoint issue fix by creating framework from Xcode 14.3.1.

### Version 7.8.0 *(4th May 2023)*
-------------------------------------------
* Updated the deployment target to 11.0.
* Added support for API and Storage Encryption.

### Version 7.7.0 *(17th April 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.7.0.

### Version 7.6.0 *(11th April 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.6.0.

### Version 7.5.0 *(22nd February 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.5.0.

### Version 7.4.0 *(6th February 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.4.0.

### Version 7.3.0 *(25th January 2023)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 9.3.0.

### Version 7.2.0 *(28th December, 2022)*
-------------------------------------------
* Bugfix - Fixed Carousel image not displaying multiple images.

### Version 7.1.0 *(13th December, 2022)*
-------------------------------------------
* Bugfix - Carousel Image Order Mismatch in collapsed mode for rich notifications.

### Version 7.0.0 *(7th December, 2022)*
-------------------------------------------
* All the classes and modules are prefixed with `MoEngage`.

### Version 6.4.0  *(18th October, 2022)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 8.4.0

### Version 6.3.2  *(3rd October, 2022)*
-------------------------------------------
*  BugFix - Handled updating of badge count

### Version 6.3.1  *(1st August, 2022)*
-------------------------------------------
*  BugFix - Handled downloading of resources for Basic notification.

### Version 6.3.0  *(20th July, 2022)*
-------------------------------------------
*  Updated the dependency to MoEngage-iOS-SDK 8.3.0.
*  Campaign stats tracking was missed in some cases from the Notification Service extension.

### Version 6.2.1  *(22nd June, 2022)*
-------------------------------------------
*  Fixed the lldb issue when integrating MoEngage-iOS-SDK to Swift application.

### Version 6.2.0  *(7th June, 2022)*
-------------------------------------------
* Updated the dependency to MoEngage-iOS-SDK 8.2.0.
* Renamed the module to MoEngageRichNotification.
* Provided  Swift Package manager support to install the SDK.

### Version 5.2.0  *(23rd September, 2021)*
-------------------------------------------
* iOS 15.0 Guidelines followed for Custom Push Templates.

### Version 5.3.0  *(31st January 2022)*
-------------------------------------------
* Added `Capacitor` integration type.
* Fixed height for the message in the notification.

### Version 5.2.1  *(29th December 2021)*
-------------------------------------------
* Fixed pageControl UI issue as it was not appearing in iOS 15 devices.

### Version 5.2.0  *(23rd September, 2021)*
-------------------------------------------
* iOS 15.0 Guidelines followed for Custom Push Templates.

### Version 5.1.0  *(27th August, 2021)*
-------------------------------------------
* Releasing module as XCFramework.

### Version 5.0.2  *(5th August, 2021)*
-------------------------------------------
* Image/media resources links are percentage encoded if not already and then processed.

### Version 5.0.1  *(16th July, 2021)*
-------------------------------------------
* Handled an exception while setting attachments to Notification Content instance.

### Version 5.0.0  *(18th January, 2021)*
-------------------------------------------
* Changes to support  MoEngage-iOS-SDK 7.0.0

### Version 4.1.0  *(17th December, 2020)*
-------------------------------------------
* Changes to support  `enableSDK()` and `disableSDK()` methods for blocking/unblocking SDK features

### Version 4.0.1  *(2nd November, 2020)*
-------------------------------------------
* Xcode 12 Build settings changes to exclude arm64 architecture for Simulator.

### Version 4.0.0  *(6th September, 2020)*
-------------------------------------------
* Push Templates Support Added(Stylized Basic and Simple Image Carousel)
* Changes to support Inbox for multiple apps with same App Group ID.(with MoEngage-iOS-SDK version 6.2.0)

### Version 3.1.1  *(18th March, 2020)*
-------------------------------------------
* Support for India cluster and fixes in impression tracking.

### Version 3.1.0  *(21st February, 2020)*
-------------------------------------------
* Minor optimizations and bug fixes.

### Version 3.0.2  *(30th October, 2019)*
-------------------------------------------
* Network Module optimizations.
* Event local time was getting tracked according to the Calendar and locale set in the device, have made it device setting independent now.

### Version 3.0.0  *(4th January, 2019)*
-------------------------------------------
* SDK now supports updating notification badge count.
* MORichNotification is now being used for saving the received notifcations, to list the same in the Core SDK Inbox feature.

### Version 2.0.0  *(23rd April, 2018)*
-------------------------------------------
* SDK was changed to dynamic framework

### Version 1.3.0  *(17th August, 2017)*
-------------------------------------------
Network calls optimized.

### Version 1.2.1  *(2nd August, 2017)*
-------------------------------------------
Changed event name used to track notification received.

### Version 1.2.0  *(1st June, 2017)*
-------------------------------------------
Fixed an issue where impression was not tracked in Swift as type casting was failing in handleRichNotification method.

### Version 1.1.1  *(3rd January, 2017)*
-------------------------------------------
Fixed a bug where attachment was not shown in Notification if App Group ID was not provided.

### Version 1.1.0  *(24th November, 2016)*
-------------------------------------------
Enabled tracking of push delivery using Notification Service Extension and AppGroups.

### Version 1.0.0  *(5th October, 2016)*
-------------------------------------------
Support for standard rich notifications with image/gif/video/audio supported for Notification Service Extension.



