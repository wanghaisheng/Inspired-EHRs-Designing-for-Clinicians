## 5

## 电子处方和计算机辅助医嘱录入 E-Prescribing and  Computerized Physician Order Entry (CPOE)

电子处方能够改善用户的准确率、效率和用户体验

E-Prescribing offers an opportunity to improve user accuracy and efficiency, a satisfying experience.

* * *

由于能够减少手写处方、更新用药列表以及变更诊疗记录的工作量，电子处方eRx成为了医生最满意的工具之一。但如果电子病历系统辅助数据录入的功能不够强大的话，
电子处方也会令人失望。电子处方能够减少由于药剂师误解处方、配出错误的剂量、或是与医生想要开的药品名十分相似的错误药品等引起的用药过失。

E-Prescribing (eRx) can be one of the most satisfying tasks of the physician because it saves the duplication of effort involved in hand-writing prescriptions, updating the list of medications, and including the changes in the office notes. E-Prescribing can also be frustrating when the EHR does not provide adequate data entry support. E-Prescribing offers the opportunity to reduce the medication errors that can result from pharmacists misreading prescriptions, dispensing an incorrect dose, or even prescribing the wrong drug because its name was similar to the name of the drug the physician actually intended.

电子处方的后台程序会发送片段的电子化数据到中心节点，由中心节点把处方信息以电子化的方式发送给待接收的药房(如果药房不支持电子处方的话可通过传真)。
药房也可以发送续药请求到下达医嘱的医生。还未广泛应用的新功能能够让下达处方的医生发送电子化的消息给药房来取消之前下达的处方。

The back-end process of e-prescribing sends discrete electronic data to a central hub, which then distributes the prescription message to the target pharmacy electronically (or via fax, if the target pharmacy lacks e-prescribing capabilities). The pharmacy can also send messages for renewal request to the prescribing physician. A new feature, not yet widely adopted, allows prescribers to send a message electronically to a pharmacy to cancel a previously prescribed medication or prescription.

>### 临床场景—针对新诊断出的糖尿病的新处方

>马丁先生是一名60岁的施工主管。三个月前，他被他的家庭医生Dr Barnes 诊断出患有糖尿病。尽管生活方式变得健康了一些，但体重仍未变化。他的手指针刺的血糖有所改善，但始
终过高，在200左右。他期望能达到80-140.

>Mr. Martin is a 60-year-old construction supervisor. Three months ago, he was diagnosed with diabetes by Dr. Barnes, his family physician. Despite some healthy lifestyle changes, his weight is unchanged. His fingerstick blood sugars are improving, but are still too high at around 200\. His goal is 80-140.

>Dr. Barnes 医生想让马丁先生服用一种名为盐酸二甲双胍的药物来控制血压。他们一起查看了电子病历系统，发现盐酸二甲双胍在马丁先生的保险范围之内，而且
自付率很低。双方对此都恨满意。为了避免出现副作用，马丁先生想一开始先从本地的药店拿30天的用量。下达的新处方以电子化的方式发送给当地的药店。

>Dr. Barnes wants Mr. Martin to take a new medication named metformin to control his blood sugar. Together they look at the EHR screen and see that metformin is on Mr. Martin’s insurance formulary, and has the lowest-tier co-pay. Both are pleased. Mr. Martin wants to start with just a 30 day prescription from his local pharmacy in case he has any side-effects. The new prescription is sent electronically to the local pharmacy.

* * *

### 5.1 查找新处方

一般而言，医生在写处方时脑子里会有某种特定的药物。这种情况下，从最惯用的列表中选择或查询该药物是添加新处方的最佳路径。电子病历系统可以帮助医生做出正确的选择，帮助录入正确的信息。
在大多数情况下，电子病历系统预先填好处方单能够省下医生的时间和脑力劳动 ([cognitive load](./human-factors.php#cognitive-load)),而且能够降低过失的风险。
如果在医生输入的时候，电子病历系统能够从药品知识库中预先拿到检索结果，能够提高医生的速度和准确率。使用源自问题列表或诊断列表中数据的预测性算法能够进一步提高查询结果列表中的匹配项。

Typically, physicians will have a particular medication in mind when they write prescriptions. In that case, choosing from a “favorites” list or searching for the drug are the quickest routes to new prescription. An EHR can help physicians make the right choices and enter the correct details. In most cases, having the EHR pre-populate the prescription forms will save physicians time and mental effort ([cognitive load](./human-factors.php#cognitive-load)), and will reduce the risk of errors. It will help the physicians’ search speed and accuracy if the EHR pre-populates the search results from the drug database as the physician types. A predictive algorithm that uses data from the Problem List or Diagnosis List is able to promote likely matches farther up the search result list.

Gallery 5.1 **Making Prescription Search Results Robust**

*   5.1 a **Typing Causes the List to Pre-Populate**— User favorites can jump to the top of the list.

![Type-ahead for results, favorites moving to the top of the list](./assets/images/examples/eRx/search_results_1.png)

*   5.1 b **Typing More Characters Produces a Closer Match**— Additional details (tablet strength “500”) may be added to the search string.

![Additional details can narrow the search](./assets/images/examples/eRx/search_results_2.png)

*   5.1 c **Allow Users to Type a Portion of the Drug Name, and Then Skip to Additional Details**— Here the physician added the dosing frequency “bid.”

![Type Partial drug queries](./assets/images/examples/eRx/search_results_3.png)

*   5.1 d **Adding the Number of Tablets Makes the Top Choice Exactly What the Doctor Ordered**

![Search the Number of Tablets](./assets/images/examples/eRx/search_results_4.png)

From Cerner PowerChart. © 2014 Cerner Corporation. Reproduced by permission of Cerner Corporation.

* * *

#### 5.1.1 下新处方

一旦医生找到他想找的药品，就需要添加相应的详细信息，回顾药品的规格、使用说明、配药的数量、授权续药的次数等。考虑周全的设计会预先根据药品给这些字段赋值，
可能是最常见的开始剂量。电子病历系统会为医生推荐一些经常使用的选项或已收藏。对于复诊病人，会推荐他们已经选过的药房。

Once a physician finds the medication she's looking for, she needs to manage additional details like adding or reviewing the dosage strength, instructions, quantity to dispense, and number of refills to authorize. A thoughtful design will pre-populate fields associated with the medication with, possibly, the instructions for the usual starting dose. The EHR system could recommend a physician’s frequently-used choices or favorites. For a returning patient, it could recommend their chosen pharmacy.

在美国，医疗保险计划常常包括了处方集(drug formularies),也就是医保所覆盖的处方药的集合。在处方集范围内，药品根据患者自付的比例被分为不同的等级。
一般的医保包含4个等级：

*   第一级通常包括了最便宜的常用药物
*   第二级包括了优先选择的品牌药物
*   第三级通常包括了非优先选择的品牌药物
*   第四级通常包括了最昂贵的专科用药

In the United States, health insurance plans often include drug formularies, which are a list of prescription drugs that will be covered by the insurance plan. Within the formulary, the drugs are grouped into a tier assignment that determines the patient’s portion of the drug cost. A typical plan includes 3 or 4 tiers:

*   Tier 1 usually includes generic medications (the least expensive)
*   Tier 2 usually includes “preferred” brand name medications
*   Tier 3 usually includes “non-preferred” brand name medications
*   Tier 4 usually includes specialty medications (the most expensive)

如果系统了解患者的药房福利方案，就能够显示相应的处方集信息，并在浏览过程中提示属于哪一级。同时，系统可以按用户所需显示更多详细信息。

If the system knows the patient’s pharmacy benefit plan, it can display the associated formulary information, indicating the tier information at a glance. Also, the system can allow the prescriber to view more detail on demand.

电子病历系统所提供的这些信息能够减少医生完成此项工作所需的脑力劳动，从而降低了认知负载。这样的电子病历系统也能够通过杜绝医生分析和减少医疗过失来提高患者安全。

An EHR that provides these details reduces the mental effort a physician needs to expend to accomplish this task, and thus reduces their cognitive load. This EHR can also enhance patients' safety by eliminating physicians' distractions and reducing the margin for error.

>#### 处方详情 Prescription Details


>处方详情中的一部分内容取决于患者的喜好

>Some of the details of the prescription will depend on a patient’s preferences:

><table class="sidebar-table" id="challenges"><thead><tr><th>医生的考虑因素</th><th>开发人员面临的挑战</th></tr></thead><tbody><tr><td>**
30天还是90天的用量?**</td><td>根据药品的费用，重新拿药的便利程度，是否是新接触的药品，想要先试试效果和适应程度，这些都会影响患者选择更多或者更少的用量.</td><td>
一般而言，保险公司提供30天或90天的药品用量。电子病历系统根据药品的剂量要求和医生指定的用药天数计算出要下达的药品数量。尤其是在进行更加复杂的计算时，
此类计算型的决策支持特别有用：比如基于体重的儿科用药剂量，计算要配发的液体药物的数量，要配发的吸入器的数量(通常只是单一的吸入器，30天的用量，但也不一定，).</td></tr><tr><td>
**患者想要选择哪家药房?**</td><td>患者可能会有1到多个喜欢的药房，一些人选择多家供应商来满足他们的需要：订单邮寄类的药房常常某种药比较便宜，最喜欢的本地药房和其他有物流优势的本地药房(一个离家、工作地点或者离诊所近，另一家则营业时间更方便)</td><td>由于保险基本上每年都会变化，电子病历系统可能至少要能够选择三家患者常用的药房，允许移除患者不再常用的药房，药房也要能够随着保险的变化而调整</td></tr><tr><td>
**是否要考虑一些剂量的限制?**</td><td>患者正在服用的其他药物可能会包含将要下达的新药品。尤其在止疼药中颇为常见。人们可能单独服用 Tylenol (acetaminophen) ，
也可能在处方中就使用如Vicodin or Percocet的复合镇痛药。</td><td>计算时考虑剂量限制能帮助医生避免患者服药过量，比如给患者增加acetaminophen每天最大剂量(4克/天)的
提醒。如果电子病历系统能够标记处此类问题，医生也就能够令患者注意这些内容。</td></tr><tr><td>**要不要考虑处方表?**</td><td>
美国患者自付的处方药成本在急剧升高。处方表能够提醒医生药房划价时会遇到的问题。这些信息最大程度上使得医生和患者能够在诊疗结束之前找到昂贵药品的能够负担的起的替代物。
如果患者是在药房发现某种药物费用很高，这会导致他们延迟拿药，给患者、医生、药房带来额外的工作.</td><td>至少要显示该药物是否属于处方表。显示层次，自付的比例，是否存在处方数量的限制
(对于proton-pump inhibitors like Prilosec or Nexium的药物，每月只能配30片而不是60是很常见的)。显示是否在配药之前需要授权，以及何种情况下需要预授权，以及要得到预授权的联系方式.</td></tr></tbody></table></div></div></div>
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

<div class="example" id="fig-5-1"><div class="ex-title"><span class="ex-type">Figure 5.1 **Allow Physicians to Modify the Display Quickly by Offering the Most Common Detail Choices for a Particular Medication**>— These include strength, instructions, quantity, and number of refills.</span>![Bring up the Most Common Medication Details](./assets/images/examples/eRx/UM_EHR_0001_med-list-expand.png)](./assets/images/examples/eRx/UM_EHR_0001_med-list-expand.png "Figure 5.1 - Allow Physicians to Modify the Display Quickly by Offering the Most Common Detail Choices for a Particular Medication - These include strength, instructions, quantity, and number of refills.")</div>
#### 5.1.5 Allow Association of a Diagnosis or Chronic Problem

Users often want to filter and sort medication list displays by diagnosis. Some medications are prescribed to alleviate multiple problems, and an EHR thus may need to be able to associate medications with multiple diagnoses. The 'multiple diagnosis' function also helps patients understand the roles of multi-purpose medications in their care plan. It also informs a variety of caregivers of all the reasons someone prescribed this medication. If a subsequent physician is considering changing a medication's dose or stopping it entirely, they'll need to know this information.

<div class="quicktip" id="therapeutic-class"><div class="sidebar cf">
#### Why Automatically Assigning a Therapeutic Class Won’t Work

Some EHR vendors may be tempted to use a drug’s therapeutic class instead of relying on physician-assigned diagnoses.<span class="elipsis">..<span class="a">Read more</span></span>

<div class="qt-content show">

Some EHR vendors may tempted to use a drug’s therapeutic class instead of relying on physician-assigned diagnoses. They may be concerned that physicians won’t be willing to assign diagnoses to medications, which may be true if there is no return on the time investment for the physician. However, if the physicians receive a benefit (better sorting and filtering of medication lists, better clinical decision support fueled by that data, and better patient awareness of the reason for the medication) then physicians have an incentive to make the diagnosis assignment.

Using a therapeutic class (instead of the actual diagnosis selected for the individual patient) does not achieve the desired result. The physician and patient need to know why**this medication** has been prescribed for**this particular patient**. Knowing that a drug is a beta-blocker (the therapeutic class) is not sufficient, because a beta-blocker might be used for any of these diagnoses: hypertension, angina, coronary artery disease, atrial fibrillation, supraventricular arrhythmias, tremor, migraine, and portal hypertension. The therapeutic class will often be meaningless to the patient.

</div></div></div><div class="example" id="fig-5-2"><div class="ex-title"><span class="ex-type">Figure 5.2 **Allow Association of One or More Diagnoses per Medication![Associate One or More Diagnoses per Medication](./assets/images/examples/eRx/UM_EHR_0002_change-priority.png)](./assets/images/examples/eRx/UM_EHR_0002_change-priority.png "Figure 5.2 - Allow Association of One or More Diagnoses per Medication")</div>
#### 5.1.6 Stopping a Medication

Removing a medication from the list can be easy. It could also be easy (though optional) for a user to record why a physician or patient stopped a medication. Common reasons for stopping a medication include:

1.  The medication's high cost, which can take the form of coverage, co-pays, or cash out-of-pocket
2.  The medication's inefficacy
3.  The medication's side-effects
4.  The medication's side effects outweighing its benefits
5.  Patients don't understand the medication's possible benefits
6.  Patients or physicians don't trust whoever prescribed the medication

Medication timelines are richer and more informative when they capture why medications were stopped. Timelines that give users insight into patients' history with given medications can eliminate the need for time-consuming searching, paging through progress notes, or laboriously exploring historical medication list entries.

<div class="example" id="fig-5-3"><div class="ex-title"><span class="ex-type">Figure 5.3 **Medication Timeline Shows Details Like “Reason for Stopping” When User Selects a Timeline Bar![Show Details Like Reason for Stopping](./assets/images/examples/medication-list/UM_EHR_0013_tap1.png)](./assets/images/examples/medication-list/UM_EHR_0013_tap1.png "Figure 5.3 - Medication Timeline Shows Details Like “Reason for Stopping” When User Selects a Timeline Bar")</div>
#### 5.1.7 Renewing Medications

<div class="scenario">
#### Clinical Scenario — Renewing Medications Due before the Next Appointment

Mr. Martin has been seeing his family physician every three to six months, but his medications often come due for annual renewal before his upcoming appointments. Because of this disparity, Mr. Martin sometimes doesn't get his refills in time, and has to go without some of his medications for several days. Mr. Martin's refills also come in at different times throughout the month, and so he has to make several trips to the pharmacy to pick up his various prescriptions. Mr. Martin wishes his 'medication procurement' schedule could be simplified and consolidated, so that he only had to make one trip.

Mr. Martin's physician also finds the situation frustrating. If the patient came in before the renewals came due, the physician could determine whether the medication was effective, and whether the dose was right before signing off on the next round of pills. The physician feels the out-of-sync schedule they've established is a time-wasting hassle, inefficient, unsafe, inaccurate, inconvenient and pointless.

</div>

An EHR can allow a physician to renew multiple medications at the same time. This saves time and reduces the margin for error. Designing an EHR that can sort and filter the medication list by “renewal due date,” “pharmacy” and “prescribing physician” will minimize physicians' cognitive load and allow them to provide better patient-centered service.

Patients with multiple prescriptions and prescribers are often burdened with poor refill synchronization. Their refills come in on several different dates each month, and their annual renewal due dates are scattered throughout the calendar year. If physicians could easily discern which prescriptions require renewal before the next planned appointment, the physicians could consolidate their patients' prescriptions. This would reduce the physicians' workload and would be more convenient for the patients<sup>1</sup>.

Designers could allow users to easily modify existing prescriptions, preserving existing details and offering easy access to common alternative details where users might need to make changes (changing from 10 mg to 20 mg, from 1 tablet to 2 tablets, or from 30 days to 90 days, etc.).

<div class="example" id="gal-5-2"><div class="ex-title"><span class="ex-type">Gallery 5.2 **Allow Sorting and Filtering to Efficiently Facilitate Renewals</span></div><div id="cbp-fwslider-2" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">5.2 a</span> Sorting the List by Renewal Due Date**>— Makes it easier to group and manage the medications due for renewal.![Sort by Renewal Due Date](./assets/images/examples/eRx/UM_EHR_0012_sort-renew.png)](./assets/images/examples/eRx/UM_EHR_0012_sort-renew.png "Gallery 5.2 a - Sort the List by Renewal Due Date - Makes it easier to group and manage the medications due for renewal")</div>
*   <div><div class="caption"><span class="ex-type">5.2 b</span> Filtering the List by Prescriber**>— Makes it even easier to focus only on the selected medications, eliminating distracting items.![Filter by Prescriber](./assets/images/examples/eRx/UM_EHR_0013_filter-physician.png)](./assets/images/examples/eRx/UM_EHR_0013_filter-physician.png "Galery 5.2 b - Filtering the List by Prescriber - Makes it even easier to focus only on the selected medications, eliminating distracting items")</div>

</div></div>

A bar graph data visualization ([Figure 5.4](#fig-5-4) below) displaying “renewal due dates” reduces users' cognitive load.. It allows physicians to note which items need to be managed during the current visit by doing a quick visual scan. The physicians recognize what medications they need to focus on by picking out preattentive attributes, such as color and line length, rather than by having to do complex mental calculations involving reading dates, quantities, and number of refills.

<div class="example" id="fig-5-4"><div class="ex-title"><span class="ex-type">Figure 5.4 **Icons for “Refills Remaining”**>— Icons use preattentive attributes to reduce cognitive load during the medication renewal process</span>![Icons for Refills Remaining](./assets/images/examples/eRx/RenewalDue_Icons_PCTouchCerner.png)](./assets/images/examples/eRx/RenewalDue_Icons_PCTouchCerner.png "Figure 5.4 - Icons for Refills Remaining - Icons use preattentive attributes to reduce cognitive load during the medication renewal process")<div class="credit">

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

</div><div class="one-half column"><div class="example" id="fig-5-5"><div class="ex-title"><span class="ex-type">Figure 5.5 **Before: Interruptive Dialog Box**>— Doesn’t allow the physician to see existing prescription orders</span>![Dialog doesn’t allow the physician to see existing orders](./assets/images/examples/eRx/UM_EHR_0004_new-medication-bad.png)](./assets/images/examples/eRx/UM_EHR_0004_new-medication-bad.png "Figure 5.5 - Before: This interruptive dialog box doesn’t allow the physician to see existing prescription orders")</div></div><div class="one-half column"><div class="example" id="fig-5-6"><div class="ex-title"><span class="ex-type">Figure 5.6 **After: Non-interruptive Dialog Box**>— Allows users to see existing orders using a separate panel, or by making the dialog box non-interruptive.</span>![See Existing Orders in a separate panel, or a non-interruptive dialog box](./assets/images/examples/eRx/UM_EHR_0003_new-medication.png)](./assets/images/examples/eRx/UM_EHR_0003_new-medication.png "Figure 5.6 - After: Allow Users to See Existing Orders - This can be done in a separate panel, or by making the dialog box non-interruptive.")</div></div><div class="sixteen columns">
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

</div></div></div></div><div class="one-half column"><div class="example" id="fig-5-7"><div class="ex-title"><span class="ex-type">Figure 5.7 **Before:**>The physician needs to expend a lot of effort to fill in the many missing details. There are many opportunities for error.</span>![More effort is required to fill in missing details](./assets/images/examples/eRx/UM_EHR_0006_new-medication-unfilled.png)](./assets/images/examples/eRx/UM_EHR_0006_new-medication-unfilled.png "Figure 5.7 - Before: The physician needs to expend a lot of effort to fill in the many missing details. There are many opportunities for error.")</div></div><div class="one-half column"><div class="example" id="fig-5-8"><div class="ex-title"><span class="ex-type">Figure 5.8 **After:**> The EHR pre-completes key fields. Less frequently needed details are displayed less prominently.</span>![Pre-complete key fields and Display less frequently needed details less prominently](./assets/images/examples/eRx/UM_EHR_0005_annotated.png)](./assets/images/examples/eRx/UM_EHR_0005_annotated.png "Figure 5.8 - After: The EHR pre-completes key fields. Less frequently needed details are displayed less prominently.")</div></div><div class="sixteen columns">
#### 5.2.4 Assign the Correct Diagnosis for an Order or Prescription

The EHR can make the problem and diagnosis lists readily available to physicians entering orders. It could also allow users to add new diagnoses on the fly, without having to exit the ordering tool to add them.

The EHR can provide clinical decision support by suggesting probable diagnoses based on patients' list entries and lab results.Some orders are almost exclusively associated with a single diagnosis, and in these cases the system could assign this diagnosis to these orders by default. For instance an order for a A hemoglobin A1c lab test will almost always be associated with a diagnosis of diabetes or hyperglycemia.

#### 5.2.5 EHRs Can Adapt to Users, Not Users to EHRs

An adaptable EHR can let physicians “add to the shopping cart” ([Figure 5.9](#fig-5-9)), then “continue shopping” without checking out right away. This allows the physicians and patients to make preliminary decisions, and act on them immediately, but also allows them to make adjustments as the visit unfolds.

<div class="example" id="fig-5-9"><div class="ex-title"><span class="ex-type">Figure 5.9 **New Order Workflow**>— EHRs must offer users the option of building sets or collections of orders to facilitate their workflow.</span>![Build sets or collections of orders to facilitate workflow](./assets/images/examples/eRx/neworders.png)](./assets/images/examples/eRx/neworders.png "Figure 5.9 - EHRs must offer users the option of building sets or collections of orders to facilitate their workflow.")</div>
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

1、insurance formulary  处方集
2、pharmacy benefit plan 药房福利方案
3、 combination analgesics 复合镇痛药
