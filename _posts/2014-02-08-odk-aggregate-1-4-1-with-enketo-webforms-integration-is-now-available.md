---
id: 4595
title: ODK Aggregate 1.4.1 with Enketo Webforms integration is now available
date: 2014-02-08T06:36:32+00:00
author: Mitchell Sundt
layout: single
guid: /?p=4595

---
ODK Aggregate 1.4.1 is now available for download:

<a href="https://github.com/opendatakit/aggregate/releases" title="Download page" target="_blank">https://github.com/opendatakit/aggregate/releases</a>

The [ODK Aggregate VM](http://gum.co/odk-aggregate-vm) (maintained by Nafundi) is available as well.

Our <a href="http://opendatakit.appspot.com" title="opendatakit.appspot.com" target="_blank">opendatakit.appspot.com</a> site now has Enketo Webforms enabled. Click on the “Enketo Webforms” button at the top of the Submissions page to open a webform to enter submissions online.

See the release notes for details:

<a href="http://code.google.com/p/opendatakit/wiki/AggregateReleaseNotes" title="ODK Aggregate Release Notes" target="_blank">ODK Aggregate Release Notes</a>

Highlights:

  1. <a href="https://enketo.org/" title="Enketo" target="_blank">Enketo</a> Webforms integration. You can now use Enketo’s browser-based Webforms to fill-in and publish submissions directly into ODK Aggregate. This feature was developed and donated by <a href="http://sdrc.co.in/" title="SDFC India" target="_blank">SDRC India</a>. To enable Enketo integration, go to the `Site Admin / Preferences` tab and click on `Enketo API Configuration`.
  2. fix the `Z-ALPHA JSON` publisher and the `JSON File` export to emit an array of zero or more objects, one object per submission, with proper treatment of embedded quotes, no missing comma, etc. Confirmed that the output passes JSLint.
  3. fix the `CVS File` export functionality to double-up all occurrences of double-quotes in a field before surrounding that field with double quotes (per RFC 4180). This should correct problems with importing text containing double quotes.
  4. clean up date and time handling in `REDCap` publisher and enforce GMT time zone interpretation when rendering date and time strings.
