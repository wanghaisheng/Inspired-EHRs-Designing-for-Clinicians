## 4

## Allergy List


Streamline data entry and create clear, uncluttered displays to highlight important allergies.

* * *


Medication Allergy Lists (or simply Allergy Lists) currently include a patient’s known medication allergies, but they could include more.

Historically, physicians, nurses, patients, and pharmacists have included patients’ true drug allergies, other adverse drug reactions (also known as side-effects or adverse effects) such as nausea or drowsiness, and allergic reactions in their allergy lists. In this chapter, we will focus on true drug allergies and adverse drug reactions. Physicians often also include patients’ allergies to substances other than medications (such as latex, adhesive tape, peanuts and other foods) in Allergy Lists.

#### Other Kinds of Allergies

Inhalant allergies (such as asthma, hay fever, or allergies to dust and mold) are usually not included in the Allergy List, but rather<span class="elipsis">...<span class="a">Read more</span></span>


Inhalant allergies (such as asthma, hay fever, or allergies to dust and mold) are usually not included in the Allergy List, but rather in the Problem List. Very few food allergies could have an effect on prescriptions. A few injectable medications use peanut oil, glucosamine tablets may be derived from shellfish, and patients with egg or soy allergies should not be prescribed propofol.


In one way, the Allergy List is the safety net that supports the Medication List. Physicians check the medication list against this list of allergies in order to ensure patient safety. Allergic reactions can range from minor to fatal, so the Allergy List needs to be kept current to prevent these events. Good design can simplify correcting errors in the Allergy List.

* * *

### 4.1 Three Main Tasks


Developers might design Allergy Lists keeping in mind a user's three main tasks: glancing, exploring, and changing the list.

**Glancing at the list** may reveal that a patient has “no known medication allergies” – or that he’s deathly allergic to the medication the physician is about to order for him. Often, ideally every time they prescribe or administer a new medication, doctors and nurses will need to quickly refer to the Allergy List.

**Exploring the details** may help a physician decide whether a drug’s benefits outweigh the risks.

**Adding new entries** to the list can be quick and straightforward.**Editing the list** can be fast, assured, and flexible, requiring minimal details.

Let's consider the clinical scenarios prompting our three tasks, and some design makeovers that better address the needs of these scenarios and tasks.

* * *

### 4.2 Glancing at the Allergy List


#### Clinical Scenario — Considering a New Prescription

A young woman visits Dr. Barnes with what seems to be a simple bladder infection. Dr. Barnes would normally prescribe the antibiotic sulfamethoxazole / trimethoprim (or Bactrim) for this complaint, but a quick glance at the allergy list in the patient's demographic banner reveals that this patient is allergic to sulfa drugs such as Bactrim. Instead, Dr. Barnes prescribes ciprofloxacin, a suitable and equally inexpensive drug.


Every time they prescribe new medication, doctors will need to quickly refer to the Allergy List and may ask patients if they are allergic to the drugs in question.

For this task, physicians need to be able to glance at a short list that only contains the names of the drugs a patient is allergic to. This list could be clearly visible when physicians are prescribing or administering, but they don't need to see it when performing unrelated tasks, such as documenting the visit in a note. The list could be included in the patient demographic banner, where it would always be visible even while physicians do tasks that don't require it.

Developers can work to minimize physicians' cognitive loads, or the mental effort they must expend to perform this task, by making the information physicians need easy to find, and by not over-burdening them with unnecessary details. Navigating through the EHR requires time and effort, and remembering where they need to look increases the cognitive load on often already-overburdened health care providers.

We've mocked-up "before and after" versions of an allergy list ([Figures 4.1](#fig-4-1) and[4.2](#fig-4-2)) to illustrate what we mean.

This example ([Figure 4.1](#fig-4-1)) uses some of its limited space to list symptoms. The total number of items in this potentially long list is not visible unless the user hovers over the list with a mouse. The user may, however, be using a touch interface, and touch interfaces don't allow users to hover. Thus information stored in this format isn't easily accessible to some users; making use of a click or tap instead of hover will help. Listing additional substances here would actually help physicians out more. Physicians need to know, at a glance, if they're seeing all the substances on the Allergy List, or if what they're looking at has been truncated.

</div><div class="one-half column"><div class="example" id="fig-4-1"><div class="ex-title"><span class="ex-type">Figure 4.1</span><span class="ex-caption">Before: Glancing at the List<span class="capt-desc">— A design that hides key details</span></span></div>[![A design that hides key details](./assets/images/examples/allergy-list/Um_Ehr_0001_med-list-bad.png)](./assets/images/examples/allergy-list/Um_Ehr_0001_med-list-bad.png "Figure 4.1 - Before: Glancing at the List – A design that hides key details")</div></div><div class="one-half column"><div class="example" id="fig-4-2"><div class="ex-title"><span class="ex-type">Figure 4.2</span><span class="ex-caption">After: Glancing at the List<span class="capt-desc">— A design that brings key details to the forefront</span></span></div>[![Bring key details to the forefront of the design](./assets/images/examples/allergy-list/UM_EHR_0002_med-list-better.png)](./assets/images/examples/allergy-list/UM_EHR_0002_med-list-better.png "Figure 4.2 - After: Glancing at the List - A design that brings key details to the forefront")</div></div><div class="sixteen columns">

In our "after" example ([Figure 4.2](#fig-4-2)), by not listing the symptoms we were able to show more substances. The "5 more" indicator is more obvious and helpful than the hover-function it replaces, clearly telling users that the patient has five more drug allergies which are not displayed in this concise view. The number without the word “more” could be confusing. At first glance, our minds will try to jump to a conclusion about what the number means (Is it a “total of 5,” or are there “5 more” to be seen?).

Including the Allergy List in the patient demographic banner, as we've chosen to do, is one means of incorporating this list into the workflow. The Allergy List could only pop up in the workflow when the physician enters a new medication prescription or renewal ([Figure 4.3](#fig-4-3)). This would still make the Allergy List readily available to a physician making prescriptions. Most other workflows such as reviewing lab results or vital signs or reading reports, don’t require that the physician be aware of a patient's medication allergies.

<div class="example" id="fig-4-3"><div class="ex-title"><span class="ex-type">Figure 4.3</span><span class="ex-caption">Add Prescriptions</span></div>[![Add Prescriptions](./assets/images/examples/allergy-list/Um_Ehr_0003_add-orders.png)](./assets/images/examples/allergy-list/Um_Ehr_0003_add-orders.png "Figure 4.3 - Add Prescriptions")</div></div></div></section><section id="exploring-the-details" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 4.3 Exploring the Details

</div>

Sometimes a physician wants to know a bit more detail about a drug allergy on the list. How accurate is the information? Are the potential risks of using the drug outweighed by strong benefits, such as increased effectiveness or significantly lower costs?

<div class="scenario">
#### Clinical Scenario — Reviewing Allergy Details

Dr. Barnes is seeing a 38-year-old father of four. For the last two days, the patient's throat has been getting increasingly sore. Five days ago, one of his children came home from school with a fever and headache. The patient’s rapid strep test indicates that he has strep throat.

Dr. Barnes would usually prescribe penicillin because it's cheap and effective. A few years ago, however, the patient had a severe reaction to penicillin, which included hives and a swelling of the lips. The physician's next choice would be cephalexin (Keflex). Because penicillin and cephalexin are chemically similar, if the patient's allergic reaction to penicillin was truly severe, he might also have an allergic reaction to cephalexin. Other times it may perfectly safe to prescribe.

Cephalexin can be perfectly safe for people with a mild penicillin allergy. However people with a severe penicillin allergy should avoid cephalexin. The third-choice alternatives would be clindamycin or azithromycin (Z-Pak), both of which are more expensive.

</div>

Glancing at the patient demographic banner ([Figure 4.4](#fig-4-4)), the physician can see some information, but she still needs more details. What exactly happened when the patient took this drug? Was the patient's reaction severe?

<div class="example" id="fig-4-4"><div class="ex-title"><span class="ex-type">Figure 4.4</span><span class="ex-caption">Patient Demographic Banner<span class="capt-desc">— Shows only medication names.</span></span></div>[![Patient banner shows only medication names.](./assets/images/examples/allergy-list/UM_EHR_0013_patient-banner.png)](./assets/images/examples/allergy-list/UM_EHR_0013_patient-banner.png "Figure 4.4 - Patient Demographic Banner - Shows only medication names.")</div>

To get this additional information, the physician will have to use the detailed table view ([Figure 4.5](#fig-4-5)).

<div class="example" id="fig-4-5"><div class="ex-title"><span class="ex-type">Figure 4.5</span><span class="ex-caption">Medication Allergy List<span class="capt-desc">— Table view shows details.</span></span></div>[![Allergy table shows details.](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0000_allergies.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0000_allergies.png "Figure 4.5 - Medication Allergy List - Table view shows details.")</div>

With this list ([Figure 4.5](#fig-4-5)), the physician or nurse can see the information they need. More important information is on the left, and less important information is on the right. The table is simple and effective. It shows limited information and reduces the visual load on the user. By drilling a step deeper, the user can access further details.

<div class="example" id="fig-4-6"><div class="ex-title"><span class="ex-type">Figure 4.6</span><span class="ex-caption">Users Can Click Rows to Either Edit Them or to See More Details</span></div>[![Click Rows to Edit or See More Details](./assets/images/examples/allergy-list/Um_Ehr_0005_allergies-details.png)](./assets/images/examples/allergy-list/Um_Ehr_0005_allergies-details.png "Figure 4.6 - Users Can Click Rows to Either Edit Them or to See More Details")</div><div class="quicktip" id="important-details"><div class="sidebar cf">
#### What Allergy List details are important to physicians?

Know your user and their needs. We sent a convenience-sample survey to mostly academic health center physician faculty members<span class="elipsis">...<span class="a">Read more</span></span>

<div class="qt-content show">

Know your user and their needs. We sent a convenience-sample survey to mostly academic health center physician faculty members and residents at several institutions, asking what they felt was important to include in a Medication Allergy List. We had 52 responses. Our survey didn't consider regulatory requirements, which might change over time.

<div class="example" id="fig-4-7"><div class="ex-title"><span class="ex-type">Figure 4.7</span><span class="ex-caption">What Allergy List Details are Important to You?</span></div>[![Priority of Allergy List Details](./assets/images/examples/allergy-list/chart.png)](./assets/images/examples/allergy-list/chart.png "Figure 4.7 - What Allergy List Details are Important to You?")</div>

These users don't often need to know about inactive allergies, allergies' dates of onset, or the source of the EHR's information about these allergies. It's safe to hide this information in the course of regular usage.

</div></div></div></div></div></section><section id="changing-the-allergy-list" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 4.4 Changing the Allergy List (Adding and Editing)

</div><div class="scenario">
#### Clinical Scenario — Modifying the Allergy List

Dr. Barnes is seeing an adult patient who has had a sinus infection for the past two weeks. Dr. Barnes would like to prescribe the antibiotic Augmentin. As she prepares to do so, she asks the patient whether he has any drug allergies, while simultaneously glancing at the patient's allergy list in the demographic banner.

The patient's allergy list currently includes Augmentin, but gives no details about his reaction to the drug. Dr. Barnes decides to take advantage of this opportunity to add some detail to the medication allergy list.

The patient reports that he took Augmentin years ago and became nauseated. During their conversation, the patient reveals that, since then, he has taken amoxicillin with no ill effects. Augmentin and amoxicillin are both in the penicillin family, and thus Augmentin should be safe to prescribe.

To correct the allergy list, Dr. Barnes will recategorize the Augmentin allergy as a side effect.

</div>
#### 4.4.1 Editing the Allergy List

Our physician wants to quickly edit two parts of the EHR's entry for the patient's reaction to Augmentin. She wants to provide information about the patient's symptom, nausea, and to change the reaction's category from allergy to side-effect. The doctor wants to work quickly, because other clinical tasks demand her attention. The developer’s task is to make adding and removing substances from the Allergy List quick and intuitive. Here are some details for developers to keep in mind while creating EHRs that meet physicians' needs:

*   Physicians often take on new patients and need to add several allergies to their lists, so make adding entries quick and effortless.
*   Younger patients often have no known medication allergies, so make it equally quick and effortless to record, “No known medication allergies.”
*   Make recording the details of a reaction (the symptoms, date and severity) optional. Patients may not know or remember the details, and just recording the drug name can be enough to ensure the patient's safety.
*   Include an optional comment field for further information.
*   Make it easy to correct erroneous information.
*   Make it easy to find out who made entries or edits to the Allergy List. This field can be auto-populated with the active user’s name. Trustworthiness of the given information can vary depending on the source.
*   Allow drug allergies on the list to be inactivated and removed. Otherwise, physicians will need to repeatedly override drug-allergy alerts while prescribing medications, even when no allergies or adverse effects exist.

Take a look at how these two displays enable users to add allergies ([Figures 4.8](fig-4-8) and[4.9](#fig-4-9)). Which one looks easier? Why? Are they both equally safe?

</div><div class="one-half column"><div class="example" id="fig-4-8"><div class="ex-title"><span class="ex-type">Figure 4.8</span><span class="ex-caption">Before: Adding an Allergy to a Visually Busy Dialog</span></div>[![Visually busy dialog when adding an allergy](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png "Figure 4.8 - Before: Visually busy dialog when adding an allergy")</div></div><div class="one-half column"><div class="example" id="fig-4-9"><div class="ex-title"><span class="ex-type">Figure 4.9</span><span class="ex-caption">After: Simplified Dialog Requires Only Key Details<span class="capt-desc">— Removes less important information to a box in the lower screen.</span></span></div>[![Simplified dialog requires only key details](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy_2.png)](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy_2.png "Figure 4.9 - After: Simplified dialog requires only key details (removes less important information to a box in the lower screen)")</div></div><div class="sixteen columns">

The “after” example looks more straightforward, but is it as safe as the “before” example? Let’s look at the design details.

In the following screenshot ([Figure 4.10](#fig-4-10)), only the highlighted areas are essential to the task of adding a substance to the Allergy List. The information we haven't highlighted is optional, but physicians trying to complete this task still have to look at it, evaluate it, and ignore it. This unnecessary information overwhelms the physician, leading to[information overload](./human-factors.php#info_chaos).

</div><div class="one-half column"><div class="example" id="fig-4-10"><div class="ex-title"><span class="ex-type">Figure 4.10</span><span class="ex-caption">Before: Essential Data Elements Are Highlighted for Adding a Drug Allergy</span></div>[![Essential data elements are highlighted](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0005_highlighted2.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0005_highlighted2.png "Figure 4.10 - Before: Essential Data Elements Are Highlighted for Adding a Drug Allergy")</div></div><div class="one-half column"><div class="example" id="fig-4-11"><div class="ex-title"><span class="ex-type">Figure 4.11</span><span class="ex-caption">After: Simple, Sequential Design for Adding a Drug Allergy</span></div>[![Simple, Sequential Design for Adding a Drug Allergy](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy.png)](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy.png "Figure 4.11 - After: Simple, Sequential Design for Adding a Drug Allergy")</div></div><div class="sixteen columns">

Our "after" example (Figure 4.11) only includes the necessary data fields. The shaded section at the bottom offers physicians the ability to enter optional details. Our "after" design exemplifies the[principle of least effort](./human-factors.php#how-people-perceive).

#### 4.4.2 Adding to the Allergy List

When adding new entries to the Allergy Lists, nurses and physicians might:

1.  Find the name of the drug or substance from a list of possible choices.
2.  Find the symptoms that characterized the patient's reaction from a list of symptom choices.
3.  If desired, add additional details such as the type of reaction, the dates it occurred on, the source of this information, etc.

Compare two examples of ways to add new allergies to lists below ([Gallery 4.1](#gal-4-1)):

<div class="example" id="gal-4-1"><div class="ex-title"><span class="ex-type">Gallery 4.1</span><span class="ex-caption">Make It Simple to Add New Allergies</span></div><div id="cbp-fwslider" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">4.1 a</span> Before: First, Find the Name of the Drug or Substance</div>[![impossible to find the name of the drug or substance](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0002_visual-queries-1.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0002_visual-queries-1.png "Gallery 4.1 a - Before: First, Find the Name of the Drug or Substance")</div>
*   <div><div class="caption"><span class="ex-type">4.1 b</span> Before: Next, Add the Reaction Symptoms</div>[![Adding reaction symptoms is difficult](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0003_visual-queries-2.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0003_visual-queries-2.png "Gallery 4.1 b - Before: Next, Add the Reaction Symptoms")</div>
*   <div><div class="caption"><span class="ex-type">4.1 c</span> After: Simplified Visual Path with Fewer Fields when Adding Allergies</div>[![Simplified Visual Path with Fewer Fields](./assets/images/examples/allergy-list/Um_Ehr_0007_add-allergy-visual.png)](./assets/images/examples/allergy-list/Um_Ehr_0007_add-allergy-visual.png "Gallery 4.1 c - After: Simplified Visual Path with Fewer Fields when Adding Allergies")</div>

</div></div>

The simplified example's design (see[Gallery 4.1 c](#gal-4-1-c)) can be faster and easier to use. It has a clear visual sequence, which makes it easier to navigate and thus more likely to be completed.

#### 4.4.3 Predictive Search Fields

Predictive search fields can substantially reduce the mental effort and time it takes physicians to add entries to an Allergy List. Pushing the most likely results to the top of the list of predictive search results will make it easier for users to find what they're looking for. Users are far more likely to want to enter a simple description, like "cough," than they are to want to enter a more detailed result, such as "whooping cough" or "smoker's cough."

</div><div class="one-half column"><div class="example" id="fig-4-12"><div class="ex-title"><span class="ex-type">Figure 4.12</span><span class="ex-caption">Before: Searching Symptoms to Add a New Allergy<span class="capt-desc">— The search result listing shows the primary term, "cough," far down a visually busy list.</span></span></div>[![searching symptoms results in a visually busy list](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png "Figure 4.12 - Before: Searching Symptoms to Add a New Allergy - The search result listing shows the primary term, 'cough,' far down a visually busy list.")</div></div><div class="one-half column"><div class="example" id="fig-4-13"><div class="ex-title"><span class="ex-type">Figure 4.13</span><span class="ex-caption">After: Searching Symptoms to Add a New Allergy<span class="capt-desc">— List displays fewer results and pushes simpler, more frequently-chosen results to the top.</span></span></div>[![simpler search results pushes fewer, frequently-chosen results to the top](./assets/images/examples/allergy-list/Um_Ehr_0008_add-allergy-after.png)](./assets/images/examples/allergy-list/Um_Ehr_0008_add-allergy-after.png "Figure 4.13 - After: Searching Symptoms to Add a New Allergy - List displays fewer results and pushes simpler, more frequently-chosen results to the top.")</div></div><div class="sixteen columns">

As you can see, it is difficult to find the simple term "cough" in our "before" example ([Figure 4.12](fig-4-12)). The term is about a third of the way down the list, buried among many other terms.

In our "after" example ([Figure 4.13](fig-4-13)), the simple cough is at the top of the list. Other options are listed alphabetically further down the list, after a visual break.

</div></div></section><section id="summary" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 4.5 Summary

</div>
1.  Consider the users and their tasks. This will help you decide what details and functions to incorporate in a particular Allergy List view.
2.  Create a clear, uncluttered navigation path through the form physicians use to input allergy information.
3.  Reduce information chaos by eliminating unnecessary details and amount of reading users must do to accomplish the targeted task.
4.  Reduce cognitive load and reduce errors by offering a predictive search function.
5.  Make adding the details of reactions (such as symptoms, dates and severity) optional.
6.  Make recording that a patient has "no known medication allergies" effortless.
7.  Make correcting erroneous information from previous entries easy.

</div></div></section></section>