---
id: 6014
title: 'ODK 1.4.5 released – major enhancement to ODK Collect'
date: 2015-01-13T15:01:21+00:00
author: Mitchell Sundt
layout: single
guid: https://opendatakit.org/?p=6014

---
There are new v1.4.5 versions available on each tool's releases page <a title="Downloads Page" href="https://github.com/opendatakit" target="_blank">https://github.com/opendatakit</a>

**<span style="color: #008000;">Many thanks to Survey CTO</span>** (<a title="SurveyCTO" href="http://www.surveycto.com" target="_blank">http://www.surveycto.com</a>) for working with the ODK core team to achieve vast improvements in the correctness and speed of the ODK Collect form evaluation logic — particularly in the handling of repeat groups.

**ODK Collect**

  * numerous bug fixes and extreme performance improvements to the form evaluation logic resulting from a close collaboration between the ODK core team and SurveyCTO.
  * Added Admin Setting for “Form Processing Logic” to select among different form evaluation logic implementations: 
      * Recommended form evaluation logic (default – whatever logic is the current best going forward)
      * January 2015 (fastest) form evaluation logic
      * January 2015 (safest) form evaluation logic
      * Mid 2014 form evaluation logic (ODK Collect 1.4.4 and 1.4.3)
      * Early 2014 form evaluation logic (ODK Collect 1.4.2 and earlier)
  * update to newest GME API (October 2014)
  * new function: enclosed-area() (or area()) contributed by SurveyCTO
  * new Japanese translation and numerous translation updates
  * see <a href="https://code.google.com/p/opendatakit/wiki/CollectReleaseNotes" target="_blank">https://code.google.com/p/opendatakit/wiki/CollectReleaseNotes</a> for additional changes.

**ODK Aggregate**

  * Fix: mark-as-complete on encrypted submissions (requires ODK Briefcase v1.4.5 or higher).
  * Fix: add a server preference to ignore partially inserted/deleted submissions. Logs them but ignores them so that you can access all other rows in your dataset. Disabled by default. By default, all actions fail upon encountering any malformed submission. You should not ignore these failures but should correct them as soon as is practical.
  * <span style="color: #0000ff;">incompatible 2.0 Data model and Sync protocol changes.</span> Incompatible with device releases: rev 122 and earlier. See the release notes for upgrade steps.
  * updated javarosa jar (supporting enclosed-area() and area() functions).
  * see the release notes for additional changes and upgrade steps. <a href="http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes" target="_blank">http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes</a>

**ODK Briefcase**

  * Fix: mark-as-complete on encrypted submissions (requires ODK Aggregate v1.4.5 and higher); impossible to access encrypted submissions that were marked-as-complete while running earlier ODK Aggregate releases without hand editing.
  * updated javarosa jar (supporting enclosed-area() and area() functions).
  * see the release notes for additional changes <a href="https://code.google.com/p/opendatakit/wiki/ODKBriefcase" target="_blank">https://code.google.com/p/opendatakit/wiki/ODKBriefcase</a>

**XLSForm**
  
 **xlsform.exe for Windows**
  
 **ODK Validate**
  
 **ODK FormUploader**
  
 **ODK ClearBriefcasePreferences**

  * updated javarosa jar (supporting enclosed-area() and area() functions).

**ODK CsvConverter**

  * no changes, just updating the version to 1.4.5
