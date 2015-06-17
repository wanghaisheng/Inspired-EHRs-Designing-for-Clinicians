## 6

## Drug Alerts


Effective alerts increase patient safety while reducing physicians’ cognitive load

* * *


A[report](http://www.ahrq.gov/research/findings/factsheets/errors-safety/aderia/index.html#MedicationErrors) from the Agency for Healthcare Research and Quality estimates that adverse drug events annually result in over 770,000 injuries and deaths and cost up to $5.6 million dollars per hospital. A system that alerts prescribing physicians to medication conflicts can help reduce the number of adverse drug events. To be effective, however, a physician must notice, read, understand, and respond to the alerts. How well they do this depends, in part, on the design of the alerting system, including the alert rules and the methods used to display and interact with the alerts. An effective alerting system needs to strike a balance, alerting physicians to real safety risks without overwhelming them, causing alert fatigue and increasing their cognitive load. If the system gives too many nuisance alarms, or the alarms are hard to read and understand, physicians will quite reasonably begin to ignore the alerts. This chapter will focus on how developers can apply user interface and interaction design principles to create effective alerts. We consider two types of drug-related alerts: drug-allergy alerts and drug-drug interaction alerts.

* * *

### 6.1 Drug Allergy Alerts

Drug allergy alerts inform physicians that their patient may be allergic to whatever they’ve just prescribed. The physician may have accidentally overlooked the allergy. They’ll need to weigh the drug’s potential risks against its potential benefits, and either go forward with the prescription or cancel it. Let’s look at a simple clinical scenario.

#### Clinical Scenario — Drug Allergy Alert

Mr. Martin is a 60-year-old who, barring one exception, was in good health until a decade ago when he was hospitalized after a severe automobile accident. At that time, he had a documented allergy (generalized hives, itching, and facial swelling) to the IV drug Unasyn, an antibiotic drug combination that contains sulbactam and ampicillin, which is a member of the penicillin family.

Today he is visiting Dr. Barnes, his primary care doctor, with symptoms of acute sinusitis. The problem has been going on for almost two weeks and is not improving. Dr. Barnes’s first choice of treatment is Augmentin (clavulanate plus amoxicillin, which is also a member of the pencillin family). She glances at the allergy list in the patient header, looking for the word “penicillin” but does not see it. The term “Unasyn” did not catch her attention, perhaps because she wasn’t thinking about compounds that contained drugs closely related to penicillin. She enters an e-prescription for Augmentin, but then a drug alert interrupts her workflow. The alert identifies the patient’s allergy to Unasyn, the symptoms and severity, and Unasyn’s chemical similarity to Augmentin. Dr. Barnes reconsiders her decision and chooses doxycycline, a different antibiotic.


Alerts need to support the physician’s thinking process by addressing five questions:

1.  How serious is the problem?
2.  What is the nature of the problem?
3.  What can the physician do to avoid or mitigate the effects of the problem?
4.  If the physician does not address the problem, what will the consequences be?
5.  Where can the physician learn more about this problem?

[Figure 6.1](#fig-6-1) demonstrates how a typical alert in current EHRs address these questions. This design doesn’t direct the user’s eye to the information she needs to answer the questions. The alert contains a lot of text, but since it is all roughly the same size and none of it has been given any emphasis, it looks like all the information is equally (un)important. Some text (such as the window title, “Medication Clinical Decision Support” and “The new order has been created…”) convey little to no relevant information. The visual elements, such as the alignment of text and the arrangement of the page’s white space, do little to direct the eye. The page contains three hyperlinks, but two of these lead to the same reference information, which is unlikely to aid the decision-making process.

</div><div class="one-half column"><div class="example" id="fig-6-1"><div class="ex-title"><span class="ex-type">Figure 6.1</span><span class="ex-caption">Before: A Penicillin Family Drug-Allergy Alert</span></div>[![A Penicillin Family Drug-Allergy Alert](imagesexamples/drug-alerts/DrugAllergyAlertCerner2014_Unasyn_AugmentinRx.png)](imagesexamples/drug-alerts/DrugAllergyAlertCerner2014_Unasyn_AugmentinRx.png "Figure 6.1 - Before: A Penicillin Family Drug-Allergy Alert")</div></div><div class="one-half column"><div class="example" id="fig-6-2"><div class="ex-title"><span class="ex-type">Figure 6.2</span><span class="ex-caption">After: A Penicillin Family Drug-Allergy<span class="capt-desc">— A simplified design with fewer options and concise text.</span></span></div>[![A simplified design with fewer options and concise text](imagesexamples/drug-alerts/Um_Ehr_0000_DrugAllergyAlert-2014-c.png)](imagesexamples/drug-alerts/Um_Ehr_0000_DrugAllergyAlert-2014-c.png "Figure 6.2 - After: A Penicillin Family Drug-Allergy - A simplified design with fewer options and concise text")</div></div><div class="sixteen columns">

[Figure 6.2](#fig-6-2) is a redesigned version of the same penicillin family drug-allergy alert. It allows the physician to see at a glance that the alert indicates a serious drug allergy (as noted by the two caution icons). The alert conveys the names of the drugs involved, and key facts about the patient’s reaction. It shows the physician what actions she can take and which one is recommended ("Stop Augmentin," where “Stop” is the more prominent button). The design visually indicates the importance of key information using different font sizes, boldface, and colors to direct the user’s eye. Gray or smaller text denotes that the information written in it is less important.

The design shows what information is related by grouping related items together, and using whitespace to separate different groups of items. We eliminated much of the text that appears in the original design ([Figure 6.1](#fig-6-1)) to protect the user from cognitive overload (information overload). Clicking the 'i' (information) icon to the right of the name of the drug the patient is allergic to brings up additional information about the patient’s allergic reaction. This redesigned alert allows the user to find the important information about a drug allergy quickly. If desired, they can then learn more about less vital information, like the specific details of the patient's reaction. The 'feedback' link allows the user to provide feedback to the clinical decision support team.

* * *

### 6.2 Drug-Drug Interaction Alerts

Drug interactions are far more complex than drug allergies. A drug allergy either exists or doesn't, though there is some room for doubt about whether an allergy was truly the issue at the time, whether the allergy still persists, and what the nature of the reaction was. With drug interactions, there are more variables: the strength of scientific evidence for the interaction, the severity category for the interaction (usually 3-5 levels from mild to severe), the organizational threshold for displaying alerts based on alert severity, and patient variables (age, weight, pregnancy, and renal function).

<div class="scenario">
#### Clinical Scenario - Severe Drug Interaction

Mr. Martin, our 60-year-old who was involved in a motor vehicle accident, suffers from chronic pain. The problem requires a multi-pronged treatment approach which includes several different medications. He is taking the muscle relaxant tizanidine to treat his low back spasms. In the past two days, Mr. Martin has needed to urinate frequently and urgently, and urination has been painful. Dr. Barnes diagnosed him with a bladder infection. As she started to order the antibiotic ciprofloxacin, a passive, non-intrusive alert appeared in the corner of the screen ([see Figure 6.3](#fig-6-3)). Rather than completing the prescription details and selecting the pharmacy, she stopped and chose a different antibiotic for which there were no drug interactions.

</div><div class="example" id="fig-6-3"><div class="ex-title"><span class="ex-type">Figure 6.3</span><span class="ex-caption">A Passive Alert</span></div>[![A Passive Alert](imagesexamples/drug-alerts/Um_Ehr_0009_passive-alert.png)](imagesexamples/drug-alerts/Um_Ehr_0009_passive-alert.png "Figure 6.3 - A Passive Alert")</div>

The passive alert appears in the corner of the EHR screen, but does not interrupt the physician’s workflow. The yellow bar with an alert icon that appears in the user's peripheral vision is a salient visual signal because it is based on preattentive attributes. Without reading it, the physician can detect both the alert's existence and it's degree of severity.

If the physician completes the order, selects a pharmacy, and sends an e-prescription, an interruptive alert will pop up to ensure patient safety. The interruptive alert stops the physician’s workflow completely, demanding the physician’s full attention. The physician must select one of the three available choices before the system activates the “Continue” button to allow the physician to move forward ([Figure 6.4](#fig-6-4)). After making a selection, the physician confirms her choice by hitting the keyboard “Enter” key or clicking the aforementioned “Continue” button ([Figure 6.5](#fig-6-5)). This additional step allows the physician a chance to correct a mistake.

Interruptive alerts annoy physicians and reduce the overall effectiveness of such alerts, which causes physicians to miss alerts that truly are important. Interruptive alerts can be used sparingly. Some EHRs allow users to customize what alerts appear to what healthcare providers. Thus the EHR might use interruptive alerts only for truly serious alerts when a physician is working with it and use both serious and mild alerts when the dispensing pharmacist is working with it. One empirical study of alerting systems suggests that physicians are more likely to comply with a tiered alert system (passive for lower risk and interruptive for higher risk alerts)<sup>1</sup>.

<div class="example" id="fig-6-4"><div class="ex-title"><span class="ex-type">Figure 6.4</span><span class="ex-caption">An Interruptive Alert<span class="capt-desc">— Requires the user to make a choice before dismissing the alert.</span></span></div>[![Interruptive Alerts Require a choice before dismissing the alert.](imagesexamples/drug-alerts/Um_Ehr_0004_drug-drug-interaction-unselected-annotated.png)](imagesexamples/drug-alerts/Um_Ehr_0004_drug-drug-interaction-unselected-annotated.png "Figure 6.4 - An Interruptive Alert - Requires the user to make a choice before dismissing the alert.")</div><div class="example" id="fig-6-5"><div class="ex-title"><span class="ex-type">Figure 6.5</span><span class="ex-caption">Once the Physician Makes a Choice, the System Enables the 'Continue' Button<span class="capt-desc">— Giving users a chance to confirm their choice, but also adds an extra step, so it is best used when overriding higher severity alerts and can be customized with user preferences.</span></span></div>[![Once a choice is made, the system enables the 'Continue' button](imagesexamples/drug-alerts/Um_Ehr_0005_drug-drug-interaction-selected.png)](imagesexamples/drug-alerts/Um_Ehr_0005_drug-drug-interaction-selected.png "Figure 6.5 - Once the physician makes a choice, the system enables the 'Continue' button")</div></div></div></section><section id="user-preferences"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 6.3 User Preferences to Dismiss Future Alerts

When users are presented with a high frequency of low-value alerts, they develop alert fatigue and begin to dismiss the alerts before they fully read them or consider their implications.

Alert fatigue can be mitigated in a variety of ways:

1.  Prevent alerts where possible:
    1.  Offer only choices that will not trigger alerts (for instance, only offer available dosage forms)
    2.  Provide cognitive support to help physicians make decisions that will not trigger alerts
    3.  Adjust alert thresholds to present users with only the most important alerts
2.  [Use a tiered alerting system](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2605599/): make lower risk alerts passive and less visually obtrusive. Use interruptive alerts only for those with the[highest risk](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3628052/).
3.  Present passive alerts as early as possible during decision making. For example, by providing a visible indication of drugs that conflict with patient allergies or current drugs while the physician is choosing from a list or typing in a drug.
4.  Allow users to customize their alert settings and turn off alerts that are of no value to them.
5.  Make alerts easier to read. Write concise descriptions, put important words first, and use visual features (font size, emphasis, color, whitespace, alignment, and spatial grouping) to indicate the importance and relationships among the information.

</div></div></section><section id="customizing"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 6.4 Customizing Alerts for Individual Physicians

Some alerts will be predictably and safely dismissed 100% of the time, and can reasonably be eliminated. Perhaps a patient has been taking a medication for a long time without incident, but an alert still appears every time the prescription is renewed. Here are some common examples:

<div class="scenario">
#### Clinical Scenario &emdash; Patient Can Tolerate Medications Related to an Allergy

The patient is allergic to sulfa, but has been taking a distant chemical relative of sulfa drugs, such as the diuretics hydrochlorothiazide or chlorthalidone (both very commonly prescribed), without incident for some time. In this context, the EHR need never again warn the physician about this particular patient’s allergy to sulfa.

Lisinopril (an ACE inhibitor) gives this patient a cough, and an alert appears when the physician tries to prescribe an ARB such as losartan or valsartan, because these two classes of drugs are somewhat related. However, ARBs are known to never cause the cough that ACE inhibitors may cause. The EHR need never again warn the physician about this particular side-effect for any patient.

</div>

It would be safe to allow physicians to permanently suppress alerts in the two circumstances above ([Figure 6.6](#fig-6-6)). It is more challenging to define rules for drug interactions or drug-disease interactions when the dosing or disease severity can vary over time.

<div class="example" id="fig-6-6"><div class="ex-title"><span class="ex-type">Figure 6.6</span><span class="ex-caption">Allow Users to Customize Certain Drug Alerts</span></div>[![Customize Certain Drug Alerts](imagesexamples/drug-alerts/Um_Ehr_0001_DrugAllergyAlert-2014c-w-details.png)](imagesexamples/drug-alerts/Um_Ehr_0001_DrugAllergyAlert-2014c-w-details.png "Figure 6.6 - Allow Users to Customize Certain Drug Alerts")</div><div class="quicktip" id=""><div class="sidebar cf">
#### Collecting Feedback about the Usefulness of Alerts

Let data drive the rules for alerts. Currently, EHRs can collect structured data about the reason for alert overrides, but no EHR<span class="elipsis">..<span class="a">Read more</span></span>

<div class="qt-content show">

Let data drive the rules for alerts. Currently, EHRs can collect structured data about the reason for alert overrides, but no EHR we know of can systematically collect data about whether prescribers consider particular alerts useful.

Only a handful of companies provide data that fuels drug allergy and drug interaction alerts. These companies don’t receive direct feedback from clinician users: their relationship is mediated by their EHR vendor. If EHR vendors could tell drug data vendors that nearly all users found a particular alert to be unhelpful, then the vendors could reassess that particular data element. Figure 6.7 shows how an EHR could unobtrusively collect feedback from physicians.

Legal teams may feel that more warnings amount to greater safety, but the situation is more complicated than that. Physicians need to practice medicine efficiently, and too many alerts can cause alert fatigue and even put patients at risk.

</div></div></div><div class="example" id="fig-6-7"><div class="ex-title"><span class="ex-type">Figure 6.7</span><span class="ex-caption">Allow Users to Offer Feedback about the Usefulness of Particular Drug Alerts</span></div>[![Offer Feedback about the Usefulness of Particular Drug Alerts](imagesexamples/drug-alerts/Um_Ehr_0002_DrugAllergyAlert-2014-c-leave-feedback.png)](imagesexamples/drug-alerts/Um_Ehr_0002_DrugAllergyAlert-2014-c-leave-feedback.png "Figure 6.7 - Allow Users to Offer Feedback about the Usefulness of Particular Drug Alerts")</div></div></div></section><section id="multiple-alerts"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
#### 6.5 Multiple Drug Alerts

Sometimes an EHR needs to present multiple alerts to the user. These may be multiple alerts for a single medication, or several alerts for a number of different medications. Would the EHR display these alerts one at a time, or all at once? If they’re displayed all at once, physicians can see the big picture: all of the drug-allergies and drug-drug interactions in play. Without having to navigate to read each alert, physician’s can run down the list and make decisions for each item. Showing all the alerts simultaneously, however, may visually overwhelm the users. It might also be difficult to simultaneously show both all the alerts and the clinical information that physicians need to act on these alerts.

[Figure 6.8](#fig-6-8) shows one possible way of presenting multiple alerts on a single screen. This design shows each alert’s severity using small icons in the left column. New drug orders and either the allergy or interacting drug are displayed just after the severity icons. The rightmost column shows the actions that a physician can take to address each alert. The action buttons include both the actions and the drug names (e.g., Stop Augmentin) to help the physician understand what each button does. The design uses bold text on action buttons to show recommended actions for each alert.[Figure 6.9](#fig-6-9) shows the display after the user has made decisions about the first two alerts. The Continue button activates after the user addresses all the alerts ([Figure 6.10](#fig-6-10)).

It’s more challenging to display multiple alerts on small mobile devices.[Gallery 6.1](#gal-6-1) shows a way to displayed and address multiple alerts on a mobile phone. The first screen presents an overview of all of the alerts, grouped by type. Tapping an alert brings up details about it, as well as possible actions the physician can take.

<div class="example" id="fig-6-8"><div class="ex-title"><span class="ex-type">Figure 6.8</span><span class="ex-caption">Presenting All Alerts in a Single Screen<span class="capt-desc">— Bold type indicates preferable, safer choices</span></span></div>[![All alerts in a list, safer choices indicated](imagesexamples/drug-alerts/Um_Ehr_0006_multiple-alerts.png)](imagesexamples/drug-alerts/Um_Ehr_0006_multiple-alerts.png "Figure 6.8 - Presenting all alerts in a single screen. Bold type indicates preferable, safer choices")</div><div class="example" id="fig-6-9"><div class="ex-title"><span class="ex-type">Figure 6.9</span><span class="ex-caption">Multiple Alert Screen<span class="capt-desc">— After the physician has made some choices, the system visually shows his selections</span></span></div>[![Multiple alert screen visually shows selections](imagesexamples/drug-alerts/Um_Ehr_0007_multiple-alerts-some-selected.png)](imagesexamples/drug-alerts/Um_Ehr_0007_multiple-alerts-some-selected.png "Figure 6.9 - Multiple alert screen - After the physician has made some choices, the system visually shows his selections")</div><div class="example" id="fig-6-10"><div class="ex-title"><span class="ex-type">Figure 6.10</span><span class="ex-caption">Multiple Alert Screen<span class="capt-desc">— Once the physician has addressed all alerts, the system activates the Continue button</span></span></div>[![Once all alerts are addressed, Continue button is activated.](imagesexamples/drug-alerts/Um_Ehr_0008_multiple-alerts-all-selected.png)](imagesexamples/drug-alerts/Um_Ehr_0008_multiple-alerts-all-selected.png "Figure 6.10 - Multiple Alert Screen - Once the physician has addressed all alerts, the system activates the Continue button.")</div>

This gallery shows a design option for displaying multiple drug alerts on a smartphone.

<div class="example" id="gal-6-1"><div class="ex-title"><span class="ex-type">Gallery 6.1</span><span class="ex-caption">Displaying Multiple Drug Alerts on a Smartphone</span></div><div id="cbp-fwslider" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">6.1 a</span> One Allergy Alert and Three Drug-Drug Interactions</div>[![One allergy alert and three drug-drug interactions](imagesexamples/drug-alerts/UM_EHR_0000_main.png)](imagesexamples/drug-alerts/UM_EHR_0000_main.png "Gallery 6.1 a - One allergy alert and three drug-drug interactions")</div>
*   <div><div class="caption"><span class="ex-type">6.1 b</span> More Detailed Display<span class="capt-desc">— Allows the physician to address the allergy alert</span></div>[![More Detailed Display](imagesexamples/drug-alerts/UM_EHR_0001_allergy-1.png)](imagesexamples/drug-alerts/UM_EHR_0001_allergy-1.png "Gallery 6.1 b - More Detailed Display - Allows the physician to address the allergy alert")</div>
*   <div><div class="caption"><span class="ex-type">6.1 c</span> Physician Taps the “Stop” Button<span class="capt-desc">— The display moves on, bringing up the next alert screen</span></div>[![Tap the Stop Button, bring up the next alert](imagesexamples/drug-alerts/UM_EHR_0006_allergy-2-touch.png)](imagesexamples/drug-alerts/UM_EHR_0006_allergy-2-touch.png "Gallery 6.1 c - Physician Taps the “Stop” Button - The display moves on, bringing up the next alert screen")</div>
*   <div><div class="caption"><span class="ex-type">6.1 d</span> A Drug-Drug Interaction Alert with Three Possible Actions<span class="capt-desc">— Stop the first drug, stop the second, or continue both.</span></div>[![A Drug-Drug Interaction Alert with Three Possible Actions](imagesexamples/drug-alerts/UM_EHR_0003_dd1.png)](imagesexamples/drug-alerts/UM_EHR_0003_dd1.png "Gallery 6.1 d - A Drug-Drug Interaction Alert with Three Possible Actions - Stop the first drug, stop the second, or continue both.")</div>
*   <div><div class="caption"><span class="ex-type">6.1 e</span> Stopping Cipro Calls Up the Next Drug-Drug Alert.</div>[![Stopping Cipro calls up next drug-drug alert.](imagesexamples/drug-alerts/UM_EHR_0007_dd2-touch.png)](imagesexamples/drug-alerts/UM_EHR_0007_dd2-touch.png "Gallery 6.1 e - Stopping Cipro calls up the next drug-drug alert.")</div>
*   <div><div class="caption"><span class="ex-type">6.1 e</span> After the Physician Has Addressed All the Alerts<span class="capt-desc">— He can use the final review screen to look over and modify his decisions.</span></div>[![After Addressing All Alerts, have a final chance to review and modify decisions](imagesexamples/drug-alerts/UM_EHR_0005_final.png)](imagesexamples/drug-alerts/UM_EHR_0005_final.png "Gallery 6.1 f - After the Physician Has Addressed All the Alerts - He can use the final review screen to look over and modify his decisions.")</div>

</div></div></div></div></section><section id="summary"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 6.6 Summary

1.  An effective alert is one that physicians notice, read, understand, and respond to. We can facilitate this process by designing alert systems that use sound human factors principles.
2.  Alerts interrupt users to different degrees. Passive alerts appear when triggered, but do not require the user to attend to them immediately. Interruptive alerts stop the user’s workflow and require the user to respond before continuing his work.
3.  Make only high-risk alerts interruptive.
4.  Reduce users’ cognitive load by simplifying the visual presentation of drug alerts.
5.  Use preattentive attributes (like color, size, shape, alignment) to draw users’ attention to the most important information in Drug Alerts.
6.  Treat alerts differently depending on their severity. Low-risk alerts can be passive. They offer the physician decision support without interrupting his workflow, unless he chooses to stop and attend to them. High-risk alerts could initially generate passive notices, but these can be followed by an active notice if the physician fails to attend to the issue. Physicians should be notified about possible issues via passive notices as early as possible.

* * *

*   [<span class="ch-name">E-Prescribing</span>](./e-prescribing.php)[<span class="ch-name">Human Factors</span>](./human-factors.php)

