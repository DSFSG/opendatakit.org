---
id: 3687
title: Updated ODK Tools Released (versions 1.3 and 2.0 alpha)
date: 2013-04-12T22:57:09+00:00
author: Waylon Brunette
layout: single
guid: /?p=3687

---
The ODK Team is pleased to announce a new release that includes many new exciting features such as the ability to have Collect use an external Bluetooth printer.  This release includes bug fixes and new features for the 1.3 version of the tools as well as an introduction of some of the ODK 2.0 tool set. The goal is to include some of the functionality from 2.0 series in the 1.0 series of tools when practicable.  Here is a summary of the changes:

### **Collect 1.3**

  * Added printer support on Android 3.1 and higher systems. See <a href="https://docs.opendatakit.org/printer-widget" rel="nofollow">example printing widget</a> for more information
  * configurable display and use of ‘back’ and ‘next’ buttons, and the enabling or disabling of swipe treatment within form pages (contributed work by Nafundi).
  * configurable background transmission of submissions when network connections are detected (contributed work by Nafundi).
  * application settings can now be saved to disk and loaded from disk (makes configuring device fleets easier). (contributed work by Nafundi).
  * [issue 401](http://code.google.com/p/opendatakit/issues/detail?id=401 "Show bigger box for 'long text' fields ") – string prompts now can render a configurable-height text entry box, via the <tt>rows</tt> attribute on their <tt><input></tt> tag.
  * [issue 751](http://code.google.com/p/opendatakit/issues/detail?id=751 "enable text-based Grid widget") – compact (a.k.a. grid view) select-one and select-multiple prompts now can render text label arrays or icon arrays.
  * compact (a.k.a. grid view) select-one and select-multiple prompts, if given a fixed column width (e.g., compact-4), will rescale the images so that they exactly fit the natural width of the device. Images are not rescaled when the device is then rotated 90 degrees.
  * if a meta/instanceName field is defined in a form, the non-empty value of that field will be used as the instanceName when the form is saved (and the user will be unable to alter it). Otherwise, the pre-1.3 instance naming treatment will be used. By defining this as a calculated field, the form designer can control the naming of the submission instances.
  * if itext contains constraintMsg or requiredMsg forms, then these will be used for the constraint failure and required-but-missing error messages.

### **Aggregate 1.3.1**

  * Improved Fusion Tables publisher  that will batch submissions to move the data to Fusion Tables much faster (a reduction in speed occurred when Aggregate 1.3 moved away from Fusion Tables deprecated API to Fusion Tables API v1).
  * Automatically create a Fusion Tables View that includes all first-level repeats.
  * change watchdog to run more frequently if there is an active publisher. Provide a ‘disable’ button on the Site Admin / Preferences page to restore older behavior (to conserve GAE quota).
  * [issue 794](http://code.google.com/p/opendatakit/issues/detail?id=794 "Error handling in FormParserForJavaRosa.guardedInitHelper() could use improvement") – form upload failed for some forms on MySQL with stack exhaustion.
  * [issue 761](http://code.google.com/p/opendatakit/issues/detail?id=761 "Publish to JSON Server fails and crashes Aggregate UI") – Fix to simple JSON publisher. had caused instability when used.
  * [issue 697](http://code.google.com/p/opendatakit/issues/detail?id=697 "Problematic placement of Aggregate's delete-form pop-up") – popups don’t show centered in screen when displayed on top of scrolling regions.
  * [issue 786](http://code.google.com/p/opendatakit/issues/detail?id=786 "Aggregate: can't upload revisions to forms with repeat groups") – forms with repeat groups cannot be versioned.
  * [issue 768](http://code.google.com/p/opendatakit/issues/detail?id=768 "Rows-per-page value keeps being reset") – rows-per-page value keeps getting reset on refresh..

### Sensors Framework 2.0 ALPHA

  * Initial ALPHA release
  * The Sensors framework simplifies the development of sensor-based mobile applications by creating a common abstraction point that enables all sensors to be accessed through a unified interface. To access an external sensor you need a driver (such as Zebra Printer Driver) for the external device. See [documentation](https://docs.opendatakit.org/odk2) for more details

### Zebra Printer Driver 2.0

  * Tested on Zebra MZ220 and Zebra MZ320 printers.
  * For installation, configuration, and usage please see: <a href="https://docs.opendatakit.org/printer-widget/" rel="nofollow">example printing widget</a>