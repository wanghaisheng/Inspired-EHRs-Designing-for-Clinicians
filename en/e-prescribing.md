## 5

## E-Prescribing and  
Computerized Physician Order Entry (CPOE)

<div class="subheader">

E-Prescribing offers an opportunity to improve user accuracy and efficiency, a satisfying experience.

</div></div></div></div><section id="e-prescribing"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>

E-Prescribing (eRx) can be one of the most satisfying tasks of the physician because it saves the duplication of effort involved in hand-writing prescriptions, updating the list of medications, and including the changes in the office notes. E-Prescribing can also be frustrating when the EHR does not provide adequate data entry support. E-Prescribing offers the opportunity to reduce the medication errors that can result from pharmacists misreading prescriptions, dispensing an incorrect dose, or even prescribing the wrong drug because its name was similar to the name of the drug the physician actually intended.

The back-end process of e-prescribing sends discrete electronic data to a central hub, which then distributes the prescription message to the target pharmacy electronically (or via fax, if the target pharmacy lacks e-prescribing capabilities). The pharmacy can also send messages for renewal request to the prescribing physician. A new feature, not yet widely adopted, allows prescribers to send a message electronically to a pharmacy to cancel a previously prescribed medication or prescription.

<div class="scenario">
#### Clinical Scenario — New prescription for Newly Diagnosed Diabetes

Mr. Martin is a 60-year-old construction supervisor. Three months ago, he was diagnosed with diabetes by Dr. Barnes, his family physician. Despite some healthy lifestyle changes, his weight is unchanged. His fingerstick blood sugars are improving, but are still too high at around 200\. His goal is 80-140.

Dr. Barnes wants Mr. Martin to take a new medication named metformin to control his blood sugar. Together they look at the EHR screen and see that metformin is on Mr. Martin’s insurance formulary, and has the lowest-tier co-pay. Both are pleased. Mr. Martin wants to start with just a 30 day prescription from his local pharmacy in case he has any side-effects. The new prescription is sent electronically to the local pharmacy.

</div></div></div></section><section id="search"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 5.1 Searching for a New Medication

Typically, physicians will have a particular medication in mind when they write prescriptions. In that case, choosing from a “favorites” list or searching for the drug are the quickest routes to new prescription. An EHR can help physicians make the right choices and enter the correct details. In most cases, having the EHR pre-populate the prescription forms will save physicians time and mental effort ([cognitive load](./human-factors.php#cognitive-load)), and will reduce the risk of errors. It will help the physicians’ search speed and accuracy if the EHR pre-populates the search results from the drug database as the physician types. A predictive algorithm that uses data from the Problem List or Diagnosis List is able to promote likely matches farther up the search result list.

<div class="example" id="gal-5-1"><div class="ex-title"><span class="ex-type">Gallery 5.1</span><span class="ex-caption">Making Prescription Search Results Robust</span></div><div id="cbp-fwslider" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">5.1 a</span>Typing Causes the List to Pre-Populate<span class="capt-desc">— User favorites can jump to the top of the list.</span></div>[![Type-ahead for results, favorites moving to the top of the list](./assets/images/examples/eRx/search_results_1.png)](./assets/images/examples/eRx/search_results_1.png "Gallery 5.1 a - Typing Causes the List to Pre-Populate - User favorites can jump to the top of the list")</div>
*   <div><div class="caption"><span class="ex-type">5.1 b</span>Typing More Characters Produces a Closer Match<span class="capt-desc">— Additional details (tablet strength “500”) may be added to the search string.</span></div>[![Additional details can narrow the search](./assets/images/examples/eRx/search_results_2.png)](./assets/images/examples/eRx/search_results_2.png "Gallery 5.1 b - Typing More Characters Produces a Closer Match - Additional details (tablet strength 500) may be added to the search string")</div>
*   <div><div class="caption"><span class="ex-type">5.1 c</span>Allow Users to Type a Portion of the Drug Name, and Then Skip to Additional Details<span class="capt-desc">— Here the physician added the dosing frequency “bid.”</span></div>[![Type Partial drug queries](./assets/images/examples/eRx/search_results_3.png)](./assets/images/examples/eRx/search_results_3.png "Gallery 5.1 c - Allow Users to Type a Portion of the Drug Name, and Then Skip to Additional Details - Here the physician added the dosing frequency bid.")</div>
*   <div><div class="caption"><span class="ex-type">5.1 d</span>Adding the Number of Tablets Makes the Top Choice Exactly What the Doctor Ordered</div>[![Search the Number of Tablets](./assets/images/examples/eRx/search_results_4.png)](./assets/images/examples/eRx/search_results_4.png "Gallery 5.1 d - Adding the Number of Tablets Makes the Top Choice Exactly What the Doctor Ordered")</div>

</div></div><div class="credit">

From Cerner PowerChart. © 2014 Cerner Corporation. Reproduced by permission of Cerner Corporation.

</div><div class="sectionStart">
* * *

</div>
#### 5.1.1 Prescribing a New Medication

Once a physician finds the medication she's looking for, she needs to manage additional details like adding or reviewing the dosage strength, instructions, quantity to dispense, and number of refills to authorize. A thoughtful design will pre-populate fields associated with the medication with, possibly, the instructions for the usual starting dose. The EHR system could recommend a physician’s frequently-used choices or favorites. For a returning patient, it could recommend their chosen pharmacy.

In the United States, health insurance plans often include drug formularies, which are a list of prescription drugs that will be covered by the insurance plan. Within the formulary, the drugs are grouped into a tier assignment that determines the patient’s portion of the drug cost. A typical plan includes 3 or 4 tiers:

*   Tier 1 usually includes generic medications (the least expensive)
*   Tier 2 usually includes “preferred” brand name medications
*   Tier 3 usually includes “non-preferred” brand name medications
*   Tier 4 usually includes specialty medications (the most expensive)

If the system knows the patient’s pharmacy benefit plan, it can display the associated formulary information, indicating the tier information at a glance. Also, the system can allow the prescriber to view more detail on demand.

An EHR that provides these details reduces the mental effort a physician needs to expend to accomplish this task, and thus reduces their cognitive load. This EHR can also enhance patients' safety by eliminating physicians' distractions and reducing the margin for error.

<div class="quicktip" id="considerations"><div class="sidebar cf">
#### Prescription Details

Some of the details of the prescription will depend on a patient’s preferences<span class="elipsis">..<span class="a">Read more</span></span>

<div class="qt-content show">

Some of the details of the prescription will depend on a patient’s preferences:

<table class="sidebar-table" id="challenges"><thead><tr><th>Physician Considerations</th><th>Developer Challenges</th></tr></thead><tbody><tr><td>**30 or 90 day supplies?**</td><td>Patients will choose larger or smaller supplies of drugs depending on what a drug costs, how convenient it is to refill their prescription, or whether they’re new to the drug and want to try out first to determine their tolerance for it and its effectiveness.</td><td>Insurance companies typically offer 30 or 90 day supplies of medications. The EHR can calculate the amount of medication to order based on the medication's dosage requirements and the number of days' supply a physician orders. This mathematical decision support is particularly helpful for performing more complicated calculations including: weight-based pediatric dosing, calculating the amount to be dispensed for liquids, and the amount to be dispensed for inhalers (a single inhaler often, but not necessarily, comes with a 30 day supply).</td></tr><tr><td>**Which pharmacy does the patient wish to use?**</td><td>Patients may have one or several preferred pharmacies. Some people use a combination of suppliers to meet their needs: a mail-order pharmacy that offers them a good deal on a certain drug, a favorite local pharmacy, and another local pharmacy with some logistical advantage (one closer to work, home or the doctor’s office, or one with more convenient hours).</td><td>An EHR may allow at least three patient-preferred pharmacies. Allow the physician to remove a pharmacy that the patient no longer prefers, because insurance plans (in the U.S.) change almost annually, and the patient's preferred pharmacies may need to change with them.</td></tr><tr><td>**Are there dose limitations to consider?**</td><td>Patients may be taking other drugs that contain the new drug being prescribed. This is particularly common with pain relievers. People may be taking Tylenol (acetaminophen) alone, in combination with cough and cold remedies, or in prescription combination analgesics like Vicodin or Percocet.</td><td>Consider providing dose-limit calculations to help physicians avoid overdosing their patients. Add warnings to the patient that advise, for example, not to exceed the acetaminophen maximum total daily dose (4 grams/day). If the EHR flags this issue, then the physician can also call the patient’s attention to it.</td></tr><tr><td>**Are there formulary limitations to consider?**</td><td>Patient’s out-of-pocket prescription drug costs are rising at an alarming rate in the U.S. Formulary information can help physicians give patients some advance warning about what to expect at the pharmacy cash-register. That information empowers the patients and physicians, where possible, to find affordable alternatives for expensive medications before the office visit ends. If a patient first discovers the high cost of a given medication at the pharmacy, this can cause them to delay filling a prescription, and cause extra effort for the patient, pharmacy, and physician down the line.</td><td>At a minimum, show whether the drug is on-formulary. Show the tier, the amount of the co-pay (if available), and whether there are prescription quantity limits (it is common for proton-pump inhibitors like Prilosec or Nexium to have a limit of 30 tablets a month; not 60). Show if prior authorization will be required before allowing the pharmacy to dispense, and when possible include the criteria for prior authorization approval, including the contact number for obtaining prior authorization.</td></tr></tbody></table></div></div></div>
#### 5.1.2 Review the New Prescription Order before Sending It Out

The physician will need to review the final configuration of the new prescriptions. The EHR can flag missing elements. The physician may still need to make last minute modifications after verbally reviewing the prescriptions with the patient.

Instructions for tapering doses need to be clearly worded and can be available as preconfigured text. Here is an example of instructions for tapering doses of prednisone 10 mg tablets for poison ivy/oak/sumac: “4 tablets once daily for 3 days, then 3 tablets once daily for 3 days, then 2 tablets daily for 3 days, then 1 tablet daily for 3 days, then stop.” If there are transition instructions (stopping another medication a few days before or after starting the new one), the physician can add these.

The EHR can display drug alerts passively before the physician gives the final order. Interruptive alerts appear before the final order is submitted.

#### 5.1.3 Changing the dose

Most medications have a range of possible doses, so modifying a dose is a very common prescriber activity. It can be as simple as switching from the current dose to a new dose, or as complicated as titrating upward using different tablet sizes over an extended period of time. Sometimes the change will involve splitting tablets (if it’s safe to do), using multiple tablets of the prior dose, or spreading the dose out through the day (2 in the morning, 1 at lunch, 2 at bedtime) to achieve a more even therapeutic effect or to reduce an adverse effect. The physician can convert from one prescription strength to another using the EHR. The system can preserve the order details, such as quantity, number of refills, pharmacy, and associated diagnoses.

<div class="scenario">
#### Clinical Scenario — Increasing the Dose

A few years later, Mr. Martin’s diabetes is well controlled, but he has developed high blood pressure (BP). Three months ago, he started on lisinopril 10 mg daily for his high blood pressure (it also protects the kidneys in people with diabetes). Today his BP is at 153/96, which is still just a little high (the readings of his BP he's taken at home are likewise high). Mr. Martin is tolerating the medication well, so his physician wants to increase the dose to 20 mg daily. Mr. Martin has just received a 90 day supply in the mail last week, so he asks if he may use up his current supply of 10 mg tablets by taking 2 tablets daily for a while.

Mr. Martin is afraid that he’ll get a new bottle of 20 mg pills six weeks before he really needs them. He asks his doctor how he can avoid that. Can he take a printed prescription to submit later? Can the EHR send a message to the pharmacist instructing her not to fill the prescription until the patient makes contact to request that it be filled? Can Mr. Martin just call later for the new prescription? (Note: His physician’s office prefers to avoid the later calls, because it would be an inefficient use of office staff and physician time.)

</div>
#### 5.1.4 Changing the Current Order to a New Order

Discarding an old prescription and starting over can require a lot of time and mental effort, and can introduce the risk of error. Often, the physician only needs to change the strength of the tablet. An EHR that allows users to pick from a list of the strengths for a medication can save time. A physician may also need to adjust the number of tablets she has prescribed. Occasionally, the patient may choose to use a different pharmacy, or may request a two to four week prescription that they can fill locally while awaiting a mail-order 90 day supply.

<div class="example" id="fig-5-1"><div class="ex-title"><span class="ex-type">Figure 5.1</span><span class="ex-caption">Allow Physicians to Modify the Display Quickly by Offering the Most Common Detail Choices for a Particular Medication<span class="capt-desc">— These include strength, instructions, quantity, and number of refills.</span></span></div>[![Bring up the Most Common Medication Details](./assets/images/examples/eRx/UM_EHR_0001_med-list-expand.png)](./assets/images/examples/eRx/UM_EHR_0001_med-list-expand.png "Figure 5.1 - Allow Physicians to Modify the Display Quickly by Offering the Most Common Detail Choices for a Particular Medication - These include strength, instructions, quantity, and number of refills.")</div>
#### 5.1.5 Allow Association of a Diagnosis or Chronic Problem

Users often want to filter and sort medication list displays by diagnosis. Some medications are prescribed to alleviate multiple problems, and an EHR thus may need to be able to associate medications with multiple diagnoses. The 'multiple diagnosis' function also helps patients understand the roles of multi-purpose medications in their care plan. It also informs a variety of caregivers of all the reasons someone prescribed this medication. If a subsequent physician is considering changing a medication's dose or stopping it entirely, they'll need to know this information.

<div class="quicktip" id="therapeutic-class"><div class="sidebar cf">
#### Why Automatically Assigning a Therapeutic Class Won’t Work

Some EHR vendors may be tempted to use a drug’s therapeutic class instead of relying on physician-assigned diagnoses.<span class="elipsis">..<span class="a">Read more</span></span>

<div class="qt-content show">

Some EHR vendors may tempted to use a drug’s therapeutic class instead of relying on physician-assigned diagnoses. They may be concerned that physicians won’t be willing to assign diagnoses to medications, which may be true if there is no return on the time investment for the physician. However, if the physicians receive a benefit (better sorting and filtering of medication lists, better clinical decision support fueled by that data, and better patient awareness of the reason for the medication) then physicians have an incentive to make the diagnosis assignment.

Using a therapeutic class (instead of the actual diagnosis selected for the individual patient) does not achieve the desired result. The physician and patient need to know why**this medication** has been prescribed for**this particular patient**. Knowing that a drug is a beta-blocker (the therapeutic class) is not sufficient, because a beta-blocker might be used for any of these diagnoses: hypertension, angina, coronary artery disease, atrial fibrillation, supraventricular arrhythmias, tremor, migraine, and portal hypertension. The therapeutic class will often be meaningless to the patient.

</div></div></div><div class="example" id="fig-5-2"><div class="ex-title"><span class="ex-type">Figure 5.2</span><span class="ex-caption">Allow Association of One or More Diagnoses per Medication</span></div>[![Associate One or More Diagnoses per Medication](./assets/images/examples/eRx/UM_EHR_0002_change-priority.png)](./assets/images/examples/eRx/UM_EHR_0002_change-priority.png "Figure 5.2 - Allow Association of One or More Diagnoses per Medication")</div>
#### 5.1.6 Stopping a Medication

Removing a medication from the list can be easy. It could also be easy (though optional) for a user to record why a physician or patient stopped a medication. Common reasons for stopping a medication include:

1.  The medication's high cost, which can take the form of coverage, co-pays, or cash out-of-pocket
2.  The medication's inefficacy
3.  The medication's side-effects
4.  The medication's side effects outweighing its benefits
5.  Patients don't understand the medication's possible benefits
6.  Patients or physicians don't trust whoever prescribed the medication

Medication timelines are richer and more informative when they capture why medications were stopped. Timelines that give users insight into patients' history with given medications can eliminate the need for time-consuming searching, paging through progress notes, or laboriously exploring historical medication list entries.

<div class="example" id="fig-5-3"><div class="ex-title"><span class="ex-type">Figure 5.3</span><span class="ex-caption">Medication Timeline Shows Details Like “Reason for Stopping” When User Selects a Timeline Bar</span></div>[![Show Details Like Reason for Stopping](./assets/images/examples/medication-list/UM_EHR_0013_tap1.png)](./assets/images/examples/medication-list/UM_EHR_0013_tap1.png "Figure 5.3 - Medication Timeline Shows Details Like “Reason for Stopping” When User Selects a Timeline Bar")</div>
#### 5.1.7 Renewing Medications

<div class="scenario">
#### Clinical Scenario — Renewing Medications Due before the Next Appointment

Mr. Martin has been seeing his family physician every three to six months, but his medications often come due for annual renewal before his upcoming appointments. Because of this disparity, Mr. Martin sometimes doesn't get his refills in time, and has to go without some of his medications for several days. Mr. Martin's refills also come in at different times throughout the month, and so he has to make several trips to the pharmacy to pick up his various prescriptions. Mr. Martin wishes his 'medication procurement' schedule could be simplified and consolidated, so that he only had to make one trip.

Mr. Martin's physician also finds the situation frustrating. If the patient came in before the renewals came due, the physician could determine whether the medication was effective, and whether the dose was right before signing off on the next round of pills. The physician feels the out-of-sync schedule they've established is a time-wasting hassle, inefficient, unsafe, inaccurate, inconvenient and pointless.

</div>

An EHR can allow a physician to renew multiple medications at the same time. This saves time and reduces the margin for error. Designing an EHR that can sort and filter the medication list by “renewal due date,” “pharmacy” and “prescribing physician” will minimize physicians' cognitive load and allow them to provide better patient-centered service.

Patients with multiple prescriptions and prescribers are often burdened with poor refill synchronization. Their refills come in on several different dates each month, and their annual renewal due dates are scattered throughout the calendar year. If physicians could easily discern which prescriptions require renewal before the next planned appointment, the physicians could consolidate their patients' prescriptions. This would reduce the physicians' workload and would be more convenient for the patients<sup>1</sup>.

Designers could allow users to easily modify existing prescriptions, preserving existing details and offering easy access to common alternative details where users might need to make changes (changing from 10 mg to 20 mg, from 1 tablet to 2 tablets, or from 30 days to 90 days, etc.).

<div class="example" id="gal-5-2"><div class="ex-title"><span class="ex-type">Gallery 5.2</span><span class="ex-caption">Allow Sorting and Filtering to Efficiently Facilitate Renewals</span></div><div id="cbp-fwslider-2" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">5.2 a</span> Sorting the List by Renewal Due Date<span class="capt-desc">— Makes it easier to group and manage the medications due for renewal.</span></div>[![Sort by Renewal Due Date](./assets/images/examples/eRx/UM_EHR_0012_sort-renew.png)](./assets/images/examples/eRx/UM_EHR_0012_sort-renew.png "Gallery 5.2 a - Sort the List by Renewal Due Date - Makes it easier to group and manage the medications due for renewal")</div>
*   <div><div class="caption"><span class="ex-type">5.2 b</span> Filtering the List by Prescriber<span class="capt-desc">— Makes it even easier to focus only on the selected medications, eliminating distracting items.</span></div>[![Filter by Prescriber](./assets/images/examples/eRx/UM_EHR_0013_filter-physician.png)](./assets/images/examples/eRx/UM_EHR_0013_filter-physician.png "Galery 5.2 b - Filtering the List by Prescriber - Makes it even easier to focus only on the selected medications, eliminating distracting items")</div>

</div></div>

A bar graph data visualization ([Figure 5.4](#fig-5-4) below) displaying “renewal due dates” reduces users' cognitive load.. It allows physicians to note which items need to be managed during the current visit by doing a quick visual scan. The physicians recognize what medications they need to focus on by picking out preattentive attributes, such as color and line length, rather than by having to do complex mental calculations involving reading dates, quantities, and number of refills.

<div class="example" id="fig-5-4"><div class="ex-title"><span class="ex-type">Figure 5.4</span><span class="ex-caption">Icons for “Refills Remaining”<span class="capt-desc">— Icons use preattentive attributes to reduce cognitive load during the medication renewal process</span></span></div>[![Icons for Refills Remaining](./assets/images/examples/eRx/RenewalDue_Icons_PCTouchCerner.png)](./assets/images/examples/eRx/RenewalDue_Icons_PCTouchCerner.png "Figure 5.4 - Icons for Refills Remaining - Icons use preattentive attributes to reduce cognitive load during the medication renewal process")<div class="credit">

From Cerner PowerChart Touch. © 2014 Cerner Corporation. Reproduced by permission of Cerner Corporation.

</div></div></div></div></section><section id="cpoe"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 5.2 Computerized Physician Order Entry (CPOE)

A CPOE (also sometimes referred to as_Computerized**Provider** Order Entry_) is an electronic entry of patient care orders that electronically transmits itself to the departments (lab, radiology, etc.) or outside organizations that will fulfill it. CPOE orders can be distributed more quickly than their predecessors. They eliminate errors based on hand-writing, and can prevent duplicate orders by checking new orders against existing orders.

<div class="scenario">
#### Clinical Scenario — Placing Future Lab Orders

Mr. Martin has achieved good control of his diabetes, blood pressure, and lipids. For the past year, he's been on stable doses of his medications, and his lab results have been stable as well. He can now settle into a more predictable routine, and won't need to visit the office or undergo lab tests as frequently. In about six months, Mr. Martin will need to come in for a hemoglobin A1c lab test, and then a visit. Another six months after that, he'll need to come in for further tests (another hemoglobin A1c a fasting lipid profile and a urine microalbumin test, both for his diabetes), and then another office visit.

</div>
#### 5.2.1 Display Pre-Existing Orders to Prevent Duplication

A patient's EHR often contains unfulfilled orders. Patients forget tests, or can't find the time to get them done. If physicians can't see patients' existing future orders or recent lab results, they may accidentally order tests that have already been done or ordered, or very similar tests. This would duplicate their colleagues' work and spend resources wastefully.

When users place new orders, they can simultaneously be able to see the work that's already been done, without navigating away from their own unfinished orders and losing their work.

</div><div class="one-half column"><div class="example" id="fig-5-5"><div class="ex-title"><span class="ex-type">Figure 5.5</span><span class="ex-caption">Before: Interruptive Dialog Box<span class="capt-desc">— Doesn’t allow the physician to see existing prescription orders</span></span></div>[![Dialog doesn’t allow the physician to see existing orders](./assets/images/examples/eRx/UM_EHR_0004_new-medication-bad.png)](./assets/images/examples/eRx/UM_EHR_0004_new-medication-bad.png "Figure 5.5 - Before: This interruptive dialog box doesn’t allow the physician to see existing prescription orders")</div></div><div class="one-half column"><div class="example" id="fig-5-6"><div class="ex-title"><span class="ex-type">Figure 5.6</span><span class="ex-caption">After: Non-interruptive Dialog Box<span class="capt-desc">— Allows users to see existing orders using a separate panel, or by making the dialog box non-interruptive.</span></span></div>[![See Existing Orders in a separate panel, or a non-interruptive dialog box](./assets/images/examples/eRx/UM_EHR_0003_new-medication.png)](./assets/images/examples/eRx/UM_EHR_0003_new-medication.png "Figure 5.6 - After: Allow Users to See Existing Orders - This can be done in a separate panel, or by making the dialog box non-interruptive.")</div></div><div class="sixteen columns">
#### 5.2.2 Make It Easy to Find the Right Orders

Naming orders can be a challenge, because tests and procedures can have several commonly-used names. Different organizations may use different names for the same test. The physician ordering procedures might not be familiar with precise names listed in the EHR order catalog. The EHR might formally call a chest x-ray "XR chest". A physician, however, might look for it under:

*   chest x-ray (or variant spellings like “xray”)
*   chest XR
*   XR chest
*   X-ray chest
*   Chest x-ray 2 views
*   Chest x-ray PA and Lateral
*   CXR (fastest way to hand-write the order)

These are all correct ways to name a chest x-ray. Thus, the interface could allow physicians to find tests and procedures listed under their various commonly-used designations.

#### 5.2.3 Preconfigure Orders with as Much Detail as Possible

Tests physicians order in ER or urgent care scenarios are often high priority and need done STAT. Routine tests physicians order in primary care settings will almost always be lower-priority. They'll need completed today, in the near future, or at some specified future time. An EHR that could be easily configured to a specific care setting, one that established default "priority" settings for the orders it processed, would be a powerful support tool.

<div class="quicktip" id="fuzzy-date"><div class="sidebar cf">
#### Setting the Date for Orders: Using Fuzzy Dates

Sometimes orders demand a precise date and time.<span class="elipsis">..<span class="a">Read more</span></span>

<div class="qt-content show">

Sometimes orders demand a precise date and time. Repeating a Prothrombin Time (PT) lab test in exactly 3 days helps assure safe dosing of warfarin, a clot-preventer.

Other times, less precise dates would be more helpful. If a physician orders a lab for "one year from now," but the patient shows up eleven months later, telling the patient she's too early and sending her home would be counterproductive. The EHR needs to allow its users to set somewhat flexible "fuzzy dates." This will allow healthcare organizations to be adaptable, and to work with patients to find times and dates convenient for them.

</div></div></div></div><div class="one-half column"><div class="example" id="fig-5-7"><div class="ex-title"><span class="ex-type">Figure 5.7</span><span class="ex-caption">Before:<span class="capt-desc">The physician needs to expend a lot of effort to fill in the many missing details. There are many opportunities for error.</span></span></div>[![More effort is required to fill in missing details](./assets/images/examples/eRx/UM_EHR_0006_new-medication-unfilled.png)](./assets/images/examples/eRx/UM_EHR_0006_new-medication-unfilled.png "Figure 5.7 - Before: The physician needs to expend a lot of effort to fill in the many missing details. There are many opportunities for error.")</div></div><div class="one-half column"><div class="example" id="fig-5-8"><div class="ex-title"><span class="ex-type">Figure 5.8</span><span class="ex-caption">After:<span class="capt-desc"> The EHR pre-completes key fields. Less frequently needed details are displayed less prominently.</span></span></div>[![Pre-complete key fields and Display less frequently needed details less prominently](./assets/images/examples/eRx/UM_EHR_0005_annotated.png)](./assets/images/examples/eRx/UM_EHR_0005_annotated.png "Figure 5.8 - After: The EHR pre-completes key fields. Less frequently needed details are displayed less prominently.")</div></div><div class="sixteen columns">
#### 5.2.4 Assign the Correct Diagnosis for an Order or Prescription

The EHR can make the problem and diagnosis lists readily available to physicians entering orders. It could also allow users to add new diagnoses on the fly, without having to exit the ordering tool to add them.

The EHR can provide clinical decision support by suggesting probable diagnoses based on patients' list entries and lab results.Some orders are almost exclusively associated with a single diagnosis, and in these cases the system could assign this diagnosis to these orders by default. For instance an order for a A hemoglobin A1c lab test will almost always be associated with a diagnosis of diabetes or hyperglycemia.

#### 5.2.5 EHRs Can Adapt to Users, Not Users to EHRs

An adaptable EHR can let physicians “add to the shopping cart” ([Figure 5.9](#fig-5-9)), then “continue shopping” without checking out right away. This allows the physicians and patients to make preliminary decisions, and act on them immediately, but also allows them to make adjustments as the visit unfolds.

<div class="example" id="fig-5-9"><div class="ex-title"><span class="ex-type">Figure 5.9</span><span class="ex-caption">New Order Workflow<span class="capt-desc">— EHRs must offer users the option of building sets or collections of orders to facilitate their workflow.</span></span></div>[![Build sets or collections of orders to facilitate workflow](./assets/images/examples/eRx/neworders.png)](./assets/images/examples/eRx/neworders.png "Figure 5.9 - EHRs must offer users the option of building sets or collections of orders to facilitate their workflow.")</div>
#### 5.2.6 Building Groups of Related Orders Function like Checklists

EHRs must offer users the option of building sets or collections of orders to facilitate their workflow. This offers users personalized clinical decision support and frees them from having to depend on their memories or external reference materials to complete involved tasks. Well Child Visits, for example, follow predictable patterns. They involve immunizations at regular, predetermined intervals, specific counseling (anticipatory guidance), and set follow-up visits.

A four-month-old's Well Child Visit would include:

*   scheduling the next visit, at six months
*   administering several specific vaccines
    *   hemophilus B
    *   rotavirus
    *   pneumococcal 13-valent
    *   combination of diphtheria / hepatitis B / pertussis - acellular / polio / tetanus.

</div></div></section><section id="summary"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

</div>
### 5.3 Summary

EHRs can:

1.  Make it easy for users to select new orders by offering a predictive search function that suggests appropriate results.
2.  Fill in the blanks with probable default settings (such as 30 or 90 day prescription supplies) where possible.
3.  Remember patients’ pharmacy preferences, and allow users to remove pharmacies patients no longer prefer from the list.
4.  Use preattentive attributes, such as color and typographic emphasis to enable physicians to find the results that are more likely to be relevant quickly. Use color iconography to graphically display medication renewal due-dates.
5.  Let physicians review e-prescriptions before sending so that they can correct any errors.
6.  Allow users to sort and filter medication lists to speed up the renewal process.
7.  Allow users to modify existing orders without forcing them to start over from scratch.
8.  Allow users to personalize the interface and build detail-rich collections of related orders that function like checklists.
9.  Allow users to select specific or flexible dates for new lab orders.

</div></div></section></section>