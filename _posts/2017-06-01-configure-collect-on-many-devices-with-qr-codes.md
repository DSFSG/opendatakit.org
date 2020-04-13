---
id: 8402
title: Configure Collect on many devices with QR codes
date: 2017-06-01T15:11:15+00:00
author: Hélène Martin
layout: single
guid: https://opendatakit.org/?p=8402

---
One major challenge faced by organizations that use Open Data Kit at scale is configuring Collect across many devices.

QR code configuration, available starting in Collect v1.7.0, makes it quick and easy to share settings between devices. This feature was developed by Shobhit Agarwal with input from several other community members. We hope you find it useful!

The first step to using QR code configuration is to choose one device to be the reference. On that device, set up the general and admin settings as desired. Once the reference device is set up, go to Admin Settings > Import/Export settings. You should see a QR code representing all the settings on that device.

<img class="wp-image-8404 size-medium aligncenter" src="/assets/wp-content/uploads/2017/06/Screenshot_1496350807.png" alt="A QR code from the Import/Export settings feature." width="225" height="400" />

The most common next step will be to take all of the devices that need to be configured and open up Admin Settings > Import/Export settings > Scan code. This will show a QR code scanner that you can use to scan the code from the reference device. Once the code is successfully scanned, Collect will return to the landing screen with a message saying settings were successfully loaded.

Another option is to share the generated barcode as an image. For example, one person could generate the code and then send it to several different data collection sites to make sure all devices are configured in the same way. To share a barcode from a reference devices, go to Admin Settings > Import/Export settings and tap on the three dots at the upper right corner. Tap on Share and select how you would like to share it.

<img class="aligncenter wp-image-8406 size-medium" src="/assets/wp-content/uploads/2017/06/Screenshot_1496350856.png" alt="Share an image of the QR code." width="225" height="400" />

The barcode contains all of the settings in clear text. That means that if passwords are included, anyone with access to the code could have access to the passwords. If you need to share settings in a public way, consider excluding passwords by tapping the bottom of the screen.

<img class="aligncenter wp-image-8405 size-medium" src="/assets/wp-content/uploads/2017/06/Screenshot_1496350811.png" alt="Select whether or not passwords should be included in the code." width="225" height="400" />

If you find this feature useful, please [leave a review in the Play Store](https://play.google.com/store/apps/details?id=org.odk.collect.android&hl=en). Thanks to all who were involved in describing, developing and testing this feature.

We have some great extensions in mind such as generating codes on the server side. This would make it possible to include server usernames and passwords specific to a particular user. Stay tuned for that!
