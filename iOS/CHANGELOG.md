### v1.3.2 released on January 21, 2016

* New Webhook class and delegate methods. See the updated Admin Console for including Webhook parameters.
* Example app updated to include Summary Card, Photo Card and Page Card UI

### v1.3.1 released on January 7, 2016

* Fixed issues with geo-fence monitoring for reliable sync when changes are made on the admin console

### v1.3 released on December 17, 2015

* Added support for syncing and showing notifications associated with cards or created as a standalone action
* Added a method to enable/disable background ranging

### v1.2 released on December 9, 2015

* Added compatibility for background beacon ranging on iOS9
* Added a new delegate method which is triggered when Rule sync with server completes
* Performance improvement in rule triggering
* Cleanup all data on destroying Beaconstac shared instance

### v1.1.1 released on August 12, 2015

* Rules assigned to Tags will trigger callbacks when camped on the tagged beacon
* Added a property in MSBeaconManager to get the currently campedOnBeacon
* Fixed a bug which prevented Exit Rules to not trigger if there were multiple Exit Rules on same beacon

### v1.1 released on August 4, 2015

* Added MSTags class to enable grouping beacons by tags
* Start/Stop Geo-fence api changed 
* Added delegate callback if SDK fails to sync rule with the server
* Shows error in Console if an invalid UUID is entered

### v1.0 released on June 4, 2015

* Added MSPlace class to enable grouping beacons by places
* Ability to add Geo-fences around MSPlace with entry/exit callbacks 
* Version number dropped from framework name

### v0.9.16 released on April 29, 2015

* Added ability to track sessions based on change in time and location

### v0.9.15 released on April 27, 2015

* Added ability to reset a Beaconstac sharedInstance in case of switching user accounts

### v0.9.14 released on Apr 15, 2015

* Rule processor Action type webhook - webhook parameters now contain more contextual information

### v0.9.13 released on Apr 9, 2015

* Delegate method names updated to include sender object as the first parameter in Beaconstac, MSBeaconManager and MSRuleProcessor classes
* Added more fields to event log packet like campon duration on a beacon
* Added a description property to MSBeacon class
* Major improvement in beacon campon and exit behavior
* Minor bug fixes and improvements

### v0.9.12 released on Feb 9, 2015

* Added more fields to event logger
* Added support for Beaconstac delegates to be optional
* Major bug fix - First time beacon detection bug fixed
* Minor bug fixes

### v0.9.11 released on Jan 7, 2014

* Added GET, POST, PUT, DELETE methods to MSNetwork class
* Deprecated postToServer and fetchDataForURL methods in MSNetwork class
* Added MSUIAction enum for action type in MSAnalytics. Deprecated MSActionType in MSAnalytics
* Added created, modified and status properties to MSAction class
* Added MSCard and MSMedia classes to Beaconstac for handling card action type and media in card action type
* Fixed bug - Ranging and monitoring beacons specific to region
* Fixed bug - Removed ambiguity with class name for Reachability.h
* Fixed bug - webhook action type post parameters
* Fixed bug - Added Dwell time implementation to exit beacon event

### v0.9.10 released on Dec 18, 2014

* Added sharedInstanceWithOrganizationId: developerToken method for creating a Beaconstac shared instance
* Added method for start ranging beacons with UUID and identifier in Beaconstac and MSBeaconManager classes
* Added support for filter options while ranging beacons 
* Added method for stopping beacon ranging in Beaconstac and MSBeaconManager classes
* Added support for triggering rules based on exit beacon event
* Deprecated setUpOrganizationId: userToken: beaconUUID: beaconIdentifier method from Beaconstac class
* Deprecated sharedInstance method in Beaconstac class
* Modified initUserIdentity method to setUserIdentity in Beaconstac class

