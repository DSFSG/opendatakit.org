---
id: 5660
title: ODK v1.4.4 tools now available
date: 2014-08-29T16:24:38+00:00
author: Mitchell Sundt
layout: single
guid: /?p=5660

---
There are new v1.4.4 versions of:

##### ODK Aggregate

  * Installer now asks for an ODK Aggregate username and uses that as the super-user (rather than a gmail account). Eliminates problems with Google OpenID logins by avoiding/obsoleting them.
  * IE 6 and IE 7 are no longer supported.
  * Fix for column naming bug that sometimes impacted tables with 60+character-long field names
  * Many updates to 3rd party libraries
  * Incompatible ODK Tables changes — if you have tried ODK Tables, see the [release notes](http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes) for upgrade steps.

##### ODK Collect

  * New feature: delete-after-submit capability and setting. Contributed by Nafundi
  * New feature: saveIncomplete() functionality. Contributed by Nafundi
  * New feature: access form definitions off of Google Drive and publish forms to Google Maps Engine and Picassa (jointly). Contributed by Nafundi
  * New: Czech and Polish translations
  * Fix: when user credentials are changed, the old credentials were not cleared. Contributed by SurveyCTO.
  * Fix: changing user settings were not reflected in user property values referenced by subsequent forms.
  * Fix: crash due to bad french translation
  * Fix: crash when two or more forms referenced the same external itemset
  * Fix: internationalization issue in external itemsets

##### XLSForm
  
xlsform.exe

  * Most documentation has moved to [here](http://xlsform.org/)
  * New prompt type: “select one external” Documentation coming shortly…

##### ODK Validate

  * Fix: recognizes property(‘propertyname’) function and detects typos in property names
