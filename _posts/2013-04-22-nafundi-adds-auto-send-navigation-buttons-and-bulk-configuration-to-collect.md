---
id: 3714
title: Nafundi adds auto send, navigation buttons, and bulk configuration to Collect
date: 2013-04-22T17:56:30+00:00
author: Yaw Anokwa
layout: single
guid: /?p=3714

---
At [Nafundi](http://nafundi.com), we have made a commitment to improving ODK Collect, and for this new v1.3 release, we are excited to add features that make data collection easier for users. These features include auto sending of finalized forms, forward/backward buttons for navigation, and bulk configuration of devices.

**Auto sending of finalized forms**
  
In our consulting work, we’ve had a few clients request that we change ODK Collect so it automatically sends finalized forms to the server. This feature is needed because it ensures data is immediately available for reports. Auto send also reduces training requirements. Thanks to [eHealth Nigeria](http://ehealthnigeria.org), we are now able to provide this feature to the ODK community. 

To enable auto send, go to the main screen, tap the menu button, and then tap General Settings. Scroll to the Auto Send section, and choose to auto send with Wi-Fi or the cell network or both.

Once enabled, auto send will try to send all finalized forms whenever any form is saved and finalized. It will also try to send finalized forms whenever a Wi-Fi or cell network connection becomes available. This feature works even while ODK Collect is not running.

**Forward/backward buttons for navigation**
  
Historically, ODK Collect has used swipes to move between form entry screens. This is because when the ODK project started, Android devices were small and so there was little screen real estate for buttons. While swipes required more training, that design saved precious on-screen space.

Today, Android devices are getting larger and we saw an opportunity to make form navigation more intuitive for novice users. To do this, we added an option for placing forward and backward buttons on the bottom of the form entry screens. 

To try this feature, tap the menu button while on the main screen. Tap General Settings and scroll to the User Interface section. Tap on Navigation to choose between horizontal swipes (the default), forward/backward buttons, or both. We think you’ll find that the buttons make navigation easier for users. Thanks to [The Taskforce for Global Health](http://taskforce.org) for making this feature possible.

**Bulk configuration of devices**
  
Nafundi supports a number of ODK deployments with thousands of devices, and as you can imagine, configuring that many devices can be a chore! To improve that process, we created a feature that makes bulk configuration of many devices easier.

From the main screen, tap the menu button. Tap Admin Settings, tap the menu button again, tap Save Settings to Disk. This will save your general and admin settings to /odk/settings/collect.settings. Copy this settings file to /odk/collect.settings of any other device running ODK Collect v1.3, and when you re-launch ODK Collect, it will automatically load those settings, and delete that file.
  

  
Upgrade to [ODK Collect v1.3](https://play.google.com/store/apps/details?id=org.odk.collect.android) today to start using auto send, navigation buttons, and bulk configuration. And remember, you can hide any of these options from your users using [admin mode](/2012/11/admin-mode-arrives-in-odk-collect-1-2-2) — a feature we added only a few months ago.
