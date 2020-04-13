---
id: 3399
title: ODK Aggregate 1.3.0 Released
date: 2013-02-02T16:32:55+00:00
author: Mitchell Sundt
layout: single
guid: /?p=3399

---
ODK Aggregate 1.3.0 Production Release is now available for download. In many small ways, this is a complete update to the publishing capabilities of the server.

**This release breaks all publishers. See the [release notes](http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes) for recommended upgrade steps.**

Significant fixes and features:

  * Three new Alpha-stage publishers have been added – 1 REDCap compliant XML publisher, 2 JSON publishers. See [Publisher Details](http://code.google.com/p/opendatakit/wiki/AggregateToJSonXmlREDCapPublishers) for information about the new publishers.
  * Most links open a new tab, rather than switching you off the page. Added and enabled links for repeat groups in Fusion Tables publishers and for the Google Spreadsheet publisher.
  * The Fusion Tables publisher now automatically constructs a flattened view (left outer join) of the top-level table and the first repeat group in the table.
  * Added a ‘Published Through’ and an ‘Owner’ column to the ‘Published Data’ table to communicate the progress of the publisher and who is receiving the data (really, the initial owner).
  * [Issue 718](http://code.google.com/p/opendatakit/issues/detail?id=718), [Issue 730](http://code.google.com/p/opendatakit/issues/detail?id=730) – some large forms cause table subdivision algorithm to fail, preventing the form from loading into ODK Aggregate. This change affects what tables are constructed and what they contain.
  * JSON file export – remove extra trailing comma from exported dataset (e.g., in repeat groups). Multiple-choice selects are now emitted as an array of string values.
  * Forms are now listed alphabetically by title.
  * Installer now supports migrated AppEngine instance (for Master-Slave -to- High-Replication Datastore migration).
  * Webserver configuration has been revised to enable reference VM images to be constructed for, e.g., AWS deployments.
  * Moved the periodic ‘watchdog’ worker to the UI thread, which should lead to a reduction in quota usage.
  * Annual jar update and transition to OAuth 2.0 for all Google publishers.

[Read the release notes](http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes) and then [download Aggregate v1.3](https://github.com/opendatakit/aggregate/releases) to try it out.
