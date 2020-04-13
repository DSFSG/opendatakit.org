---
id: 3320
title: Metadata, outputs and calculates in Build
date: 2013-01-14T05:08:57+00:00
author: Yaw Anokwa
layout: single
guid: /?p=3320

---
We are excited to announce that ODK Build now has support for metadata prompts, outputs in captions, and calculates on prompts! As explained below, these features enable users to build higher quality forms. 

**Metadata**
  
Metadata prompts are hidden prompts in the ODK form that the data collector does not see. In Build, there is now support for metadata like timestamps for when the form was started and finished as well as metadata that uniquely identifies the device. These new prompt types are at the bottom of screen in Build and can be treated like any other prompt type (drag and drop as needed). Build also now automatically includes a special kind of metadata called instanceID. instanceIDs uniquely identify the completed form and help ensure that no duplicate forms end up in the final dataset.

**Outputs**
  
Build now supports the ${/data/dataName} output syntax for referring to previous answers in captions and hints. For example, users can now have a caption that reads:
  
_Your device ID is ${/data/deviceID}. Your first name is ${/data/firstName}._ 

When a data collector sees this caption on the device, it can be filled in with the answers previously given. In this case, if a form designer had a metadata prompt called “deviceID” and a text prompt called “firstName” that was previously answered, the caption would read:
  
_Your device ID is 12:34:56:78:90. Your first name is Yaw._

Below is an image of an output prompt showing the answer from a metadata prompt.
  
<img src="/assets/wp-content/uploads/2013/01/outputExample.png" width="538" alt="An output prompt showing the answer from a metadata prompt" />

**Calculates**
  
Calculates are an advanced technique for running a calculation using a prompt’s answers. Because they are complex to use, they are found under the advanced section of Build’s prompt properties. Find out more about how to use calculates in the [form design guide](https://docs.opendatakit.org/form-logic).
  

  
Metadata, outputs, and calculates are available because [CartONG](http://www.cartong.org) hired the ODK consultants at [Nafundi](http://nafundi.com) to work with ODK Build creator [Clint Tseng](http://www.linkedin.com/in/clinttseng) on these features. Thanks to CartONG for funding these contributions to the community! 

Try these changes today at <http://build.opendatakit.org>. If you need a sample form, download, unzip and load this [Demo-Form.odkbuild.zip](/assets/wp-content/uploads/2013/01/Demo-Form.odkbuild.zip) into ODK Build.
