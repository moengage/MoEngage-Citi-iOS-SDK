
# 06-09-2024

## MoEngage-iOS-SDK - 9.19.0
-------------------------------------------

### Core
#### Whats New
* Cards fetch on login support added.
* Multiple self handled inapps support.

#### Improvements
* Expose app install/update API without appId input
* Revamp storage access
* Refactor threading and queueing
#### Fixes
* Fixed previous instance deinitialization when default instance changed.
* in-memory data not getting cleared on disable data tracking
* Source tracking happening before flush
* Device type not getting tracked after data tracking re-enabled from disabled
* Analytics batch data migration from 8.7.0
* User getting reset while on disabled state
* API calls not happening when application is killed and relaunched with SDK state enabled from disabled state.
* No data tracked post tracking restricted unique id
* No data tracked post tracking invalid timestamp or location
* Inconsistency with unique id validation    

### Analytics
#### Whats New
* Cards fetch on login support added.
#### Improvements
* Cleaned remoteconfig whitelisted events.
* Added push opt-in device attribute tracking.

### Messaging
#### Whats New
* Added support for Provisional Push.
#### Improvements
* Refactor threading and queueing
* Added push opt-in device attribute and events tracking and navigate to settings page API.

### RichNotification
#### Improvements
* Refactor threading and queueing
    
# 01-08-2024  

## Version 9.18.1
-------------------------------------------
* Fixed Swift Package Resolution

# 31-07-2024

### Version 9.18.0
-------------------------------------------
* Internal improvements

#### Core
* Added secondary domain config when primary domain blocked.
* Deprecated SDK provided SSL Pinning in favour of [OS provided one](https://developer.apple.com/documentation/bundleresources/information_property_list/nsapptransportsecurity/nspinneddomains).

# 03-07-2024

## MoEngage-iOS-SDK - 9.17.5
-------------------------------------------
* Fixed crash in decryption.
* Updated the SDK to v9.17.5. Refer to [release notes](https://developers.moengage.com/hc/en-us/articles/4404198236564-Changelog#01HSGCGGR02V0PS58JT86NQ2RP) for more details.

## MoEngaeRichnotification - 7.16.1
-------------------------------------------
* Updated the SDK to v7.16.1. Refer to [release notes](https://developers.moengage.com/hc/en-us/articles/4404198236564-Changelog#01HP1ZFYYM7AFTJMBQ7CDYW5ZK) for more details.

# 06-05-2024

## MoEngage-iOS-SDK - 9.15.1
-------------------------------------------
* Fixed the app rejection issue due to privacy manifest

# 23-01-2024

## MoEngage-iOS-SDK - 9.15.0
-------------------------------------------
* Added privacy manifest file
* Added Code signature support for XCFrameworks.
* Updated the deployment target to 14
* Added support for new domain.


## MoEngageRichNotification - 7.14.0
-------------------------------------------
* Added privacy manifest file
* Added Code signature support for XCFrameworks.
* Updated the deployment target to 14
