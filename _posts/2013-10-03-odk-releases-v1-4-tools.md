---
id: 4102
title: ODK Releases v1.4 tools
date: 2013-10-03T10:10:10+00:00
author: Mitchell Sundt
layout: single
guid: /?p=4102

---
Version 1.4 updates to the ODK tools are now available:

### ODK Collect 1.4 rev 1037

  * Fix to prevent corruption during encryption. See notes for details.
  * new ‘placement-map’ appearance for geopoint widget. Allows the user to move the location marker on the map.
  * Now uses Android 3.x and 4.x look-and-feel when running on those devices.
  * Several functions have been added for use in calculations.
  * Numerous other bug fixes and enhancements.



See [ODK Collect Release Notes](http://code.google.com/p/opendatakit/wiki/CollectReleaseNotes) for details.

### ODK Aggregate 1.4

  * New Google Maps Engine publisher. See [Google Maps Engine Instructions](http://code.google.com/p/opendatakit/wiki/GoogleMapsEngineInstructions) for details.
  * Changed behavior: **Z-Alpha JSON Server** has changed.
  * PostgreSQL fix for issue preventing some form definitions from being uploaded to the server.



See [ODK Aggregate Release Notes](http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes) for details and upgrade instructions.

### ODK Validate 1.4

Improve reporting of errors and eliminate some inappropriate warnings.

### ODK Briefcase 1.4

Automatically recover submission data when the encrypted submission has been corrupted (partial fix).  See [ODK Briefcase Release Notes](http://code.google.com/p/opendatakit/wiki/ODKBriefcase) for details.

### ODK FormUploader 1.4

Unchanged.
