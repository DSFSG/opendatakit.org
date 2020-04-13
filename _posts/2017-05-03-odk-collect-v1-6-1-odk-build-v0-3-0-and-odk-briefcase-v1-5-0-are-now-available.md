---
id: 8331
title: ODK Collect v1.6.1, ODK Build v0.3.0, and ODK Briefcase v1.5.0 are now available
date: 2017-05-03T14:14:58+00:00
author: Yaw Anokwa
layout: single
guid: https://opendatakit.org/?p=8331

---
April’s updates to Collect, Build, and Briefcase are now available, and if you care about offline data collection at scale, there is a lot to be excited about!

We’ve made Collect much smaller to download and improved date handling, Build is about 100x faster for big forms and can now be used entirely offline, and Briefcase de-duplicates exports to save disk space and reduce data cleaning.

Across all three tools, we had more 25 individual contributors adding features, fixing bugs, and improving the quality of the code. We’ve put the highlights below, but be sure to check out the full release notes!

ODK improves a lot faster if you contribute! If you are a user, please file issues when you find them. If you are a developer, join us on <http://slack.opendatakit.org> and help fix those issues for the next release. Together, we can make ODK even better!

**ODK Collect v1.6.1**

  * APK size reduced by 65% for faster app updates
  * Change app language to one of 47 languages from settings
  * Date/time widgets with no-calendar appearance allow null and are centered for accuracy
  * Google Drive/Sheets now supports video/audio uploads
  * Save sorting order on every form screen

Use: <https://play.google.com/store/apps/details?id=org.odk.collect.android>
  
Read full release notes: <https://github.com/opendatakit/collect/releases>
  
Report any issues: <https://github.com/opendatakit/collect/issues>

**ODK Build v0.3.0**

  * Build can now be used completely offline!
  * Performance improvements increase large-form performance by 100x
  * Freeform language options: you can name your languages whatever you want
  * Drag questions between two Build documents open in different windows
  * Hold Shift or Ctrl/Cmd (Win/Mac) to select multiple questions and move them around together
  * New help pane gives more help and information than before

Use online: <https://build.opendatakit.org>
  
Use offline: [https://github.com/opendatakit/build/releases](https://github.com/opendatakit/build/releases)
  
Read full release notes: <https://github.com/opendatakit/build/releases>
  
Report any issues: <https://github.com/opendatakit/build/issues>

**ODK Briefcase v1.5.0**

  * Pulls from Collect are de-duplicated
  * CSV exports are sorted chronologically and de-duplicated
  * Invalid encrypted instances no longer block exports

Use: [https://github.com/opendatakit/briefcase/releases](https://github.com/opendatakit/briefcase/releases)
  
Read full release notes: <https://github.com/opendatakit/briefcase/releases>
  
Report any issues: <https://github.com/opendatakit/briefcase/issues>
