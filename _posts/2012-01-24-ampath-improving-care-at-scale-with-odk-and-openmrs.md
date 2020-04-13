---
id: 2283
title: AMPATH Improving Care At Scale With ODK and OpenMRS
date: 2012-01-24T16:16:30+00:00
author: Yaw Anokwa
layout: single
guid: /?p=2283
aktt_notify_twitter:
  - 'no'

---
[AMPATH](http://ampathkenya.com) is the one of the largest HIV treatment programs in sub-Saharan Africa and is Kenya’s most comprehensive initiative to combat the virus. The program’s catchment area has over 2 million people and provides care to more than 130,000 HIV-positive patients across 55 urban and rural clinics. To provide care at this scale, AMPATH has invested in tools like [OpenMRS](http://openmrs.org) (an open source medical record system) and Open Data Kit, to help improve the efficiency and impact of their health providers. 

**Home-Based Counseling and Testing with ODK Collect**
  
AMPATH has an extensive home-based and counseling program where community health workers (CHWs) go house to house to identify and enroll persons in need of care (i.e., pregnant women not in antenatal care, orphaned children, persons at high risk for tuberculosis infection). The workers need mobile data collection to document socio-economic data (including GPS location of household) and to implement the counseling and testing protocol.

Before using ODK, AMPATH used Palm TX devices running Pendragon Forms. GPS information was collected using eTrex devices. Problems with this approach were outlined by Rajput et al. in their [Evaluation of an Android-based mHealth System for Population Surveillance in Developing Countries](http://jamia.bmj.com/content/early/2012/02/23/amiajnl-2011-000476.full) (AMIA 2011) paper. 

They write, “_First, although costs were significantly lower than paper-based data collection methods the costs were still substantial. Second, the data collected could not be directly integrated into the electronic medical record system [OpenMRS] which was already in use at the AMPATH clinics — integration required dedicated time by several experienced data managers. Third, the cable connection between the PDA and GPS devices was not always reliable, and GPS information had to occasionally be entered manually into the PDA devices. Fourth, the use of the proprietary Pendragon Forms Software on the PDA devices limited flexibility to incorporate some functionality into the data collection software –- some of these functionality included advanced barcode scanning and check-digit algorithms._”

In late 2009, we provided an early version of ODK Collect to AMPATH (on an HTC Dream, the first Android device). We spent a week with them in Kenya piloting the system, and based on the available functionality, AMPATH decided to switch to Open Data Kit. Below is a picture of one of the CHWs scanning a patient barcode with the phone.

<img width="524" src="//opendatakit.org/assets/wp-content/uploads/2012/01/ampath-barcode.png" alt="One of the CHWs scanning a patient barcode with the phone" />

In early 2010, AMPATH finalized the HCT form, made minor changes to the user interface, acquired Android devices, and started to scale up. It is important to note that ODK’s core developers were not involved at this stage.

Rajput et al. evaluated the ODK implementation at AMPATH a few months after and showed that “_Users of the system felt it was easy to use, and facilitated their home visits. It is more cost effective than pen-and-paper alternatives. Additionally, electronic data collection facilitated earlier reporting. We have implemented a viable solution at scale for collecting electronic data during household visits._” 

More importantly, that study also found that for the 63,000 persons encountered, “_the direct capture of electronic records greatly facilitated the expeditious performance of initial analyses and reports prior to the conclusion of the three year HCT program. Our work has highlighted … most notably that only 28% of persons we are identifying as infected with HIV are presenting for follow-up care._” AMPATH has acted on this data by launching programs to improve follow-up.

It has been almost two years since AMPATH started using ODK Collect. We recently touched base with the HCT program to see how their use of technology has scaled. Since early 2010, ODK has been used by a few hundred CHWs in over 650,000 patient encounters! The HCT program has a greater than 98% rate of acceptance into the homes it visits, and with the help of technology, has been able to lower mother-to-child transmission of HIV/AIDS to lower than 3%.

 **Mobile Clinical Decision Support with ODK Clinic**
  
We have continued our collaboration with AMPATH, and this year, we focused on tools for clinicians. We have created a new version of [ODK Clinic](https://code.google.com/p/opendatakit/wiki/ODKClinic), an Android-based application that downloads patient data like demographics, disease history, lab results, and recent medications from OpenMRS (and the [Clinical Summary Module](https://wiki.openmrs.org/display/docs/Clinical+Summary+Module)). We re-designed the entire application from our early v1 release and added features to enable correction of serious mistakes in the patient record. We also added decision support so clinicians receive patient-specific reminders when the system notices that sub-standard care is being offered. All this in near real time and at the point of care — a major improvement over AMPATH’s existing paper-based summaries.

If, for example, the system notices a scheduled lab test is overdue or a patient’s health indicators have dropped dramatically, a reminder is inserted into the patient’s record and displayed to the clinician. ODK Clinic can also enforce compliance with the reminders and can help compliance by wirelessly printing lab order test requisitions complete with all necessary patient data. We detailed our findings designing the system in our [Design of a Phone-Based Clinical Decision Support System for Resource-Limited Settings](http://cs.washington.edu/homes/yanokwa/publications/2011_ICTD_DecisionSupport_Paper.pdf) paper from ICTD 2012. The [talk slides](http://cs.washington.edu/homes/yanokwa/publications/2012_ICTD_DecisionSupport_Slides.pdf) are available and a video demo of the system is below.



Since that paper was written, the system has been used with about 7,500 patients at two adult HIV clinics. We are still evaluating the results of that deployment in a controlled trial, but very early results seem to show that clinicians using ODK Clinic deliver a higher standard of care. Moreover, clinicians enjoy using the system! As a few told us, “_[We] can’t see a patient without this phone._”

We believe that [technology only magnifies existing human intent and capacity](http://www.kentarotoyama.org/research/) and so, sustainable improvements require organizations who are dedicated to the communities they serve. With HCT and within HIV clinics, ODK and OpenMRS have helped make health care providers more efficient and through that efficiency, magnified their impact. We believe this is one of the reasons why this work was featured as one of the mHealth Alliance and Rockefeller Foundation’s [Top 11 in 2011 Innovators](//opendatakit.org/2011/12/odk-implementers-awarded-as-top-mhealth-innovators/) Challenge.

Our work at AMPATH has been in deep collaboration with many people. We want to thank Martin Were, Nyoman Ribeka, Sam Mbugua, Zeshan Rajput for their help. We also thank all our colleagues at OpenMRS and [Regenstrief](http://www.regenstrief.org/) for their support, and [Abbott Fund](http://www.abbottfund.org/) and [Google](https://google.org) for funding much of this work. Finally, we thank the CHWs and clinicians for their participation in our research. It is their hard work that is making a difference in the lives of the underserved.
