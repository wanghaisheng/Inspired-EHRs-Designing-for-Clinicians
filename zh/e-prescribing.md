5
-

电子处方和计算机辅助医嘱录入 E-Prescribing and Computerized Physician Order Entry (CPOE)
----------------------------------------------------------------------------------------

电子处方能够改善用户的准确率、效率和用户体验

E-Prescribing offers an opportunity to improve user accuracy and efficiency, a satisfying experience.

---

由于能够减少手写处方、更新用药列表以及变更诊疗记录的工作量，电子处方eRx成为了医生最满意的工具之一。但如果电子病历系统辅助数据录入的功能不够强大的话， 电子处方也会令人失望。电子处方能够减少由于药剂师误解处方、配出错误的剂量、或是与医生想要开的药品名十分相似的错误药品等引起的用药过失。

E-Prescribing (eRx) can be one of the most satisfying tasks of the physician because it saves the duplication of effort involved in hand-writing prescriptions, updating the list of medications, and including the changes in the office notes. E-Prescribing can also be frustrating when the EHR does not provide adequate data entry support. E-Prescribing offers the opportunity to reduce the medication errors that can result from pharmacists misreading prescriptions, dispensing an incorrect dose, or even prescribing the wrong drug because its name was similar to the name of the drug the physician actually intended.

电子处方的后台程序会发送片段的电子化数据到中心节点，由中心节点把处方信息以电子化的方式发送给待接收的药房(如果药房不支持电子处方的话可通过传真)。 药房也可以发送续药请求到下达医嘱的医生。还未广泛应用的新功能能够让下达处方的医生发送电子化的消息给药房来取消之前下达的处方。

The back-end process of e-prescribing sends discrete electronic data to a central hub, which then distributes the prescription message to the target pharmacy electronically (or via fax, if the target pharmacy lacks e-prescribing capabilities). The pharmacy can also send messages for renewal request to the prescribing physician. A new feature, not yet widely adopted, allows prescribers to send a message electronically to a pharmacy to cancel a previously prescribed medication or prescription.

> ### 临床场景—针对新诊断出的糖尿病的新处方
>
> 马丁先生是一名60岁的施工主管。三个月前，他被他的家庭医生Dr Barnes 诊断出患有糖尿病。尽管生活方式变得健康了一些，但体重仍未变化。他的手指针刺的血糖有所改善，但始 终过高，在200左右。他期望能达到80-140.
>
> Mr. Martin is a 60-year-old construction supervisor. Three months ago, he was diagnosed with diabetes by Dr. Barnes, his family physician. Despite some healthy lifestyle changes, his weight is unchanged. His fingerstick blood sugars are improving, but are still too high at around 200. His goal is 80-140.
>
> Dr. Barnes 医生想让马丁先生服用一种名为盐酸二甲双胍的药物来控制血压。他们一起查看了电子病历系统，发现盐酸二甲双胍在马丁先生的保险范围之内，而且 自付率很低。双方对此都恨满意。为了避免出现副作用，马丁先生想一开始先从本地的药店拿30天的用量。下达的新处方以电子化的方式发送给当地的药店。
>
> Dr. Barnes wants Mr. Martin to take a new medication named metformin to control his blood sugar. Together they look at the EHR screen and see that metformin is on Mr. Martin’s insurance formulary, and has the lowest-tier co-pay. Both are pleased. Mr. Martin wants to start with just a 30 day prescription from his local pharmacy in case he has any side-effects. The new prescription is sent electronically to the local pharmacy.

---

### 5.1 查找新处方

一般而言，医生在写处方时脑子里会有某种特定的药物。这种情况下，从最惯用的列表中选择或查询该药物是添加新处方的最佳路径。电子病历系统可以帮助医生做出正确的选择，帮助录入正确的信息。 在大多数情况下，电子病历系统预先填好处方单能够省下医生的时间和脑力劳动 ([cognitive load](./human-factors.php#cognitive-load)),而且能够降低过失的风险。 如果在医生输入的时候，电子病历系统能够从药品知识库中预先拿到检索结果，能够提高医生的速度和准确率。使用源自问题列表或诊断列表中数据的预测性算法能够进一步提高查询结果列表中的匹配项。

Typically, physicians will have a particular medication in mind when they write prescriptions. In that case, choosing from a “favorites” list or searching for the drug are the quickest routes to new prescription. An EHR can help physicians make the right choices and enter the correct details. In most cases, having the EHR pre-populate the prescription forms will save physicians time and mental effort ([cognitive load](./human-factors.php#cognitive-load)), and will reduce the risk of errors. It will help the physicians’ search speed and accuracy if the EHR pre-populates the search results from the drug database as the physician types. A predictive algorithm that uses data from the Problem List or Diagnosis List is able to promote likely matches farther up the search result list.

Gallery 5.1 **Making Prescription Search Results Robust**

-	5.1 a **Typing Causes the List to Pre-Populate**— User favorites can jump to the top of the list.

![Type-ahead for results, favorites moving to the top of the list](./assets/images/examples/eRx/search_results_1.png)

-	5.1 b **Typing More Characters Produces a Closer Match**— Additional details (tablet strength “500”) may be added to the search string.

![Additional details can narrow the search](./assets/images/examples/eRx/search_results_2.png)

-	5.1 c **Allow Users to Type a Portion of the Drug Name, and Then Skip to Additional Details**— Here the physician added the dosing frequency “bid.”

![Type Partial drug queries](./assets/images/examples/eRx/search_results_3.png)

-	5.1 d **Adding the Number of Tablets Makes the Top Choice Exactly What the Doctor Ordered**

![Search the Number of Tablets](./assets/images/examples/eRx/search_results_4.png)

From Cerner PowerChart. © 2014 Cerner Corporation. Reproduced by permission of Cerner Corporation.

---

#### 5.1.1 下新处方

一旦医生找到他想找的药品，就需要添加相应的详细信息，回顾药品的规格、使用说明、配药的数量、授权续药的次数等。考虑周全的设计会预先根据药品给这些字段赋值， 可能是最常见的开始剂量。电子病历系统会为医生推荐一些经常使用的选项或已收藏。对于复诊病人，会推荐他们已经选过的药房。

Once a physician finds the medication she's looking for, she needs to manage additional details like adding or reviewing the dosage strength, instructions, quantity to dispense, and number of refills to authorize. A thoughtful design will pre-populate fields associated with the medication with, possibly, the instructions for the usual starting dose. The EHR system could recommend a physician’s frequently-used choices or favorites. For a returning patient, it could recommend their chosen pharmacy.

在美国，医疗保险计划常常包括了处方集(drug formularies),也就是医保所覆盖的处方药的集合。在处方集范围内，药品根据患者自付的比例被分为不同的等级。 一般的医保包含4个等级：

-	第一级通常包括了最便宜的常用药物
-	第二级通常包括了优先选择的品牌药物
-	第三级通常包括了非优先选择的品牌药物
-	第四级通常包括了最昂贵的专科用药

In the United States, health insurance plans often include drug formularies, which are a list of prescription drugs that will be covered by the insurance plan. Within the formulary, the drugs are grouped into a tier assignment that determines the patient’s portion of the drug cost. A typical plan includes 3 or 4 tiers:

-	Tier 1 usually includes generic medications (the least expensive)
-	Tier 2 usually includes “preferred” brand name medications
-	Tier 3 usually includes “non-preferred” brand name medications
-	Tier 4 usually includes specialty medications (the most expensive)

如果系统了解患者的药房福利方案，就能够显示相应的处方集信息，并在浏览过程中提示属于哪一级。同时，系统可以按用户所需显示更多详细信息。

If the system knows the patient’s pharmacy benefit plan, it can display the associated formulary information, indicating the tier information at a glance. Also, the system can allow the prescriber to view more detail on demand.

电子病历系统所提供的这些信息能够减少医生完成此项工作所需的脑力劳动，从而降低了认知负载。这样的电子病历系统也能够通过杜绝医生分析和减少医疗过失来提高患者安全。

An EHR that provides these details reduces the mental effort a physician needs to expend to accomplish this task, and thus reduces their cognitive load. This EHR can also enhance patients' safety by eliminating physicians' distractions and reducing the margin for error.

> #### 处方详情 Prescription Details
>
> 处方详情中的一部分内容取决于患者的喜好
>
> Some of the details of the prescription will depend on a patient’s preferences:
>
> <table class="sidebar-table" id="challenges"><thead><tr><th>医生的考虑因素</th><th>开发人员面临的挑战</th></tr></thead><tbody><tr><td>\*\* 30天还是90天的用量?**</td><td>根据药品的费用，重新拿药的便利程度，是否是新接触的药品，想要先试试效果和适应程度，这些都会影响患者选择更多或者更少的用量.</td><td> 一般而言，保险公司提供30天或90天的药品用量。电子病历系统根据药品的剂量要求和医生指定的用药天数计算出要下达的药品数量。尤其是在进行更加复杂的计算时， 此类计算型的决策支持特别有用：比如基于体重的儿科用药剂量，计算要配发的液体药物的数量，要配发的吸入器的数量(通常只是单一的吸入器，30天的用量，但也不一定，).</td></tr><tr><td>**患者想要选择哪家药房?**</td><td>患者可能会有1到多个喜欢的药房，一些人选择多家供应商来满足他们的需要：订单邮寄类的药房常常某种药比较便宜，最喜欢的本地药房和其他有物流优势的本地药房(一个离家、工作地点或者离诊所近，另一家则营业时间更方便)</td><td>由于保险基本上每年都会变化，电子病历系统可能至少要能够选择三家患者常用的药房，允许移除患者不再常用的药房，药房也要能够随着保险的变化而调整</td></tr><tr><td>**是否要考虑一些剂量的限制?**</td><td>患者正在服用的其他药物可能会包含将要下达的新药品。尤其在止疼药中颇为常见。人们可能单独服用 Tylenol (acetaminophen) ， 也可能在处方中就使用如Vicodin or Percocet的复合镇痛药。</td><td>计算时考虑剂量限制能帮助医生避免患者服药过量，比如给患者增加acetaminophen每天最大剂量(4克/天)的 提醒。如果电子病历系统能够标记处此类问题，医生也就能够令患者注意这些内容。</td></tr><tr><td>**要不要考虑处方表?\*\*</td><td> 美国患者自付的处方药成本在急剧升高。处方表能够提醒医生药房划价时会遇到的问题。这些信息最大程度上使得医生和患者能够在诊疗结束之前找到昂贵药品的能够负担的起的替代物。 如果患者是在药房发现某种药物费用很高，这会导致他们延迟拿药，给患者、医生、药房带来额外的工作.</td><td>至少要显示该药物是否属于处方表。显示层次，自付的比例，是否存在处方数量的限制 (对于proton-pump inhibitors like Prilosec or Nexium的药物，每月只能配30片而不是60是很常见的)。显示是否在配药之前需要授权，以及何种情况下需要预授权，以及要得到预授权的联系方式.</td></tr></tbody></table></div></div></div>

#### 5.1.2 处方评审/处方核实 Review the New Prescription Order before Sending It Out

医师需要对要下达的新的处方进行最终的审核。电子病历系统可以对缺失的内容做出标记。在与患者进行口头核对之后，医师也可能会对处方进行一些最终的调整。

The physician will need to review the final configuration of the new prescriptions. The EHR can flag missing elements. The physician may still need to make last minute modifications after verbally reviewing the prescriptions with the patient.

需要逐渐减少剂量的服药说明用词要明确，要能够设置成预置的文本。如下是毒葛/橡木/漆树中毒之后服用10mg每片的强的松的剂量逐渐减少的服药说明的一个例子："先连续三天每天服用一次， 每次四片，然后连续服用3天每天服用一次，每次三片，然后连续服用3天每天服用一次，每次两片，最后连续三天每天服用一次，每次一片"。如果有转换(可能在某种药物服用之前或之后的若干天 另一种药物)的说明，医生可以添加上此类内容。

Instructions for tapering doses need to be clearly worded and can be available as preconfigured text. Here is an example of instructions for tapering doses of prednisone 10 mg tablets for poison ivy/oak/sumac: “4 tablets once daily for 3 days, then 3 tablets once daily for 3 days, then 2 tablets daily for 3 days, then 1 tablet daily for 3 days, then stop.” If there are transition instructions (stopping another medication a few days before or after starting the new one), the physician can add these.

电子病历可以在医生下达医嘱之前主动地显示药物提醒。在最终的医嘱提交之前显示打断性的提醒。

The EHR can display drug alerts passively before the physician gives the final order. Interruptive alerts appear before the final order is submitted.

#### 5.1.3 剂量的变更 Changing the dose

大部分药物剂量都存在一个范围，因此修改剂量是个很常见的动作。可以只是简单的将当前剂量变成新的剂量，也可以复杂如在一段时间内逐步加量至使用不同大小的片剂。有时候会涉及到片剂的分割(如果是 安全的话)，通过多种，或者在一天内使用不同的剂量(早上2片，中午一片，晚上两片)来达到一个更加理想的治疗效果或减少不良反应。使用电子病历系统医生可以将处方的规格互相转换。系统能够保留医嘱的详细信息，如数量、续药次数、药房信息和相关诊断信息。

Most medications have a range of possible doses, so modifying a dose is a very common prescriber activity. It can be as simple as switching from the current dose to a new dose, or as complicated as titrating upward using different tablet sizes over an extended period of time. Sometimes the change will involve splitting tablets (if it’s safe to do), using multiple tablets of the prior dose, or spreading the dose out through the day (2 in the morning, 1 at lunch, 2 at bedtime) to achieve a more even therapeutic effect or to reduce an adverse effect. The physician can convert from one prescription strength to another using the EHR. The system can preserve the order details, such as quantity, number of refills, pharmacy, and associated diagnoses.

#### 临床场景——增加剂量 Clinical Scenario — Increasing the Dose

若干年后，马丁先生的糖尿病得到了很好的控制，但他又患上了高血压。三个月前，他开始每天服用10mg的lisinopril来治疗高血压(该药也能保护糖尿病患者的肾脏)。 今天他的血压是153/96，有点偏高(他在家测量的血压值也是一样高)。马丁先生觉得能够适应目前药物的剂量，于是医生决定增加剂量到每天20mg。由于上个礼拜马丁先生刚刚收到够吃90天的药物，于是他就问是否可以每天吃2片10mg的片剂直到把这 些药先用完。

A few years later, Mr. Martin’s diabetes is well controlled, but he has developed high blood pressure (BP). Three months ago, he started on lisinopril 10 mg daily for his high blood pressure (it also protects the kidneys in people with diabetes). Today his BP is at 153/96, which is still just a little high (the readings of his BP he's taken at home are likewise high). Mr. Martin is tolerating the medication well, so his physician wants to increase the dose to 20 mg daily. Mr. Martin has just received a 90 day supply in the mail last week, so he asks if he may use up his current supply of 10 mg tablets by taking 2 tablets daily for a while.

马丁先生担心自己会拿到一瓶能够吃六个礼拜的20mg药，他询问医生如何能够避免这种情况的发生。他可以拿着打印好的处方以后再拿药么？电子病历系统能否发送一条消息告诉药师不要配药，直到患 者主动联系药师配药？还是说马丁先生以后再来拿这个新的处方？(要注意的是：由于会浪费医生的时间，医生倾向于避免以后再来)

Mr. Martin is afraid that he’ll get a new bottle of 20 mg pills six weeks before he really needs them. He asks his doctor how he can avoid that. Can he take a printed prescription to submit later? Can the EHR send a message to the pharmacist instructing her not to fill the prescription until the patient makes contact to request that it be filled? Can Mr. Martin just call later for the new prescription? (Note: His physician’s office prefers to avoid the later calls, because it would be an inefficient use of office staff and physician time.)

#### 5.1.4 当前处方变更为新处方 Changing the Current Order to a New Order

停用旧的处方，启用新的处方需要大量的时间和精力，也会引入医疗过失的风险。通常，医师只需要改变药片的规格。电子病历系统能够让用户从某种药物的不同规格中进行选择来节省时间。 医生也可能需要调整已下达处方中药物的数量。患者偶尔会选择另一个药房，或者要求在等待邮寄的90天的药物拿到之前在本地先配2-4个礼拜的药物。

Discarding an old prescription and starting over can require a lot of time and mental effort, and can introduce the risk of error. Often, the physician only needs to change the strength of the tablet. An EHR that allows users to pick from a list of the strengths for a medication can save time. A physician may also need to adjust the number of tablets she has prescribed. Occasionally, the patient may choose to use a different pharmacy, or may request a two to four week prescription that they can fill locally while awaiting a mail-order 90 day supply.

Figure 5.1 **Allow Physicians to Modify the Display Quickly by Offering the Most Common Detail Choices for a Particular Medication**>— These include strength, instructions, quantity, and number of refills.</span>![Bring up the Most Common Medication Details](./assets/images/examples/eRx/UM_EHR_0001_med-list-expand.png)

#### 5.1.5 与诊断或慢病关联 Allow Association of a Diagnosis or Chronic Problem

用户常常想要根据诊断对用药列表进行过滤和排序。某些药物能够缓解多种病症，电子病历系统要能够把处方关联到多个诊断上。多个诊断的功能也能够帮助患者理解治疗方案中多种药物的用途。 同时也能够告诉其他医务人员给该患者使用这种药物的原因。如果后来的医生需要更改药物的剂量或者停用这种药物，就需要了解此类信息。

Users often want to filter and sort medication list displays by diagnosis. Some medications are prescribed to alleviate multiple problems, and an EHR thus may need to be able to associate medications with multiple diagnoses. The 'multiple diagnosis' function also helps patients understand the roles of multi-purpose medications in their care plan. It also informs a variety of caregivers of all the reasons someone prescribed this medication. If a subsequent physician is considering changing a medication's dose or stopping it entirely, they'll need to know this information.

#### 自动分配治疗类型不可行的原因 Why Automatically Assigning a Therapeutic Class Won’t Work

一些电子病历系统软件厂商可能会使用药物治疗类型而非依赖医生所给的诊断。他们可能担心医生不愿意给药物指定诊断，如果对于医生而言没有回报可能是这样的。但是，如果医生能够得到好处 (用药列表的过滤和排序功能更强大，数据所带来的更好的决策支持，患者能够更好的理解用药的原因)，那么医生就有了分配诊断的动力。

Some EHR vendors may tempted to use a drug’s therapeutic class instead of relying on physician-assigned diagnoses. They may be concerned that physicians won’t be willing to assign diagnoses to medications, which may be true if there is no return on the time investment for the physician. However, if the physicians receive a benefit (better sorting and filtering of medication lists, better clinical decision support fueled by that data, and better patient awareness of the reason for the medication) then physicians have an incentive to make the diagnosis assignment.

使用治疗类型(而非针对某个患者实际的诊断)是不能够达到想要的目的的。医生和患者需要了解为**这个患者** **开** 这种药物的原因.只是了解药物是beta-blocker 是不够的， beta-blocker 可以用在任意的诊断中：高血压、心绞痛、冠心病、房颤、心律失常、震颤、偏头痛和门静脉高压。对于患者而言，治疗类型是没有意义的。

Using a therapeutic class (instead of the actual diagnosis selected for the individual patient) does not achieve the desired result. The physician and patient need to know why**this medication** has been prescribed for**this particular patient**. Knowing that a drug is a beta-blocker (the therapeutic class) is not sufficient, because a beta-blocker might be used for any of these diagnoses: hypertension, angina, coronary artery disease, atrial fibrillation, supraventricular arrhythmias, tremor, migraine, and portal hypertension. The therapeutic class will often be meaningless to the patient.

Figure 5.2 **Allow Association of One or More Diagnoses per Medication** ![Associate One or More Diagnoses per Medication](./assets/images/examples/eRx/UM_EHR_0002_change-priority.png)

#### 5.1.6 停用某种药物 Stopping a Medication

从用药列表中移除/拿掉某种药物是很简单的。同样的，让用户记录医生或患者停用某种药物的原因也是很简单的。常见的原因有：

1.	药物成本太高,可能是医保目录不包括，自付比例高，完全自费
2.	药物没有效果
3.	药物的副作用
4.	药物的副作用超过了好处
5.	患者无法了解药物可能的好处
6.	患者或医生不相信这种药物

Removing a medication from the list can be easy. It could also be easy (though optional) for a user to record why a physician or patient stopped a medication. Common reasons for stopping a medication include:

1.	The medication's high cost, which can take the form of coverage, co-pays, or cash out-of-pocket
2.	The medication's inefficacy
3.	The medication's side-effects
4.	The medication's side effects outweighing its benefits
5.	Patients don't understand the medication's possible benefits
6.	Patients or physicians don't trust whoever prescribed the medication

如果能够采集停药原因的话，用药的时间轴会更加丰富。时间轴能够让用户洞察患者的某种药物的用药历史情况，避免在病程记录中耗费时间搜索、查找，或者费力地整理既往的用药列表记录。

Medication timelines are richer and more informative when they capture why medications were stopped. Timelines that give users insight into patients' history with given medications can eliminate the need for time-consuming searching, paging through progress notes, or laboriously exploring historical medication list entries.

Figure 5.3 **Medication Timeline Shows Details Like “Reason for Stopping” When User Selects a Timeline Barg** ![Show Details Like Reason for Stopping](./assets/images/examples/medication-list/UM_EHR_0013_tap1.png)

#### 5.1.7 续药 Renewing Medications

> #### 临床场景——在下次预约之前续药 Clinical Scenario — Renewing Medications Due before the Next Appointment
>
> 马丁先生每三到六个月会来看自己的家庭医生，但每年度的续药总会在下次预约之前到期。由于这个原因，马丁先生有时候不能及时拿到自己续的药，这样子很多天就吃不了这种药。一个月内他续药续的药也有多种，这样子他不得不来回往返药房多次才能够拿到多种药物。 马丁先生希望“medication procurement药品采购”的安排能够简化，这样子他只需要去一次就行。

> Mr. Martin has been seeing his family physician every three to six months, but his medications often come due for annual renewal before his upcoming appointments. Because of this disparity, Mr. Martin sometimes doesn't get his refills in time, and has to go without some of his medications for several days. Mr. Martin's refills also come in at different times throughout the month, and so he has to make several trips to the pharmacy to pick up his various prescriptions. Mr. Martin wishes his 'medication procurement' schedule could be simplified and consolidated, so that he only had to make one trip.

> 马丁先生的家庭医生也觉得这种情况很令人失望。如果患者在续药到期日之前来访，医生能够确认该药是否有效，在签发下一个疗程的用药之前确认剂量是否合适。医生觉得目前他们所采用的
这种不同步的安排是很浪费时间，低效，不安全，不准确，不方便也是无意义的。

> Mr. Martin's physician also finds the situation frustrating. If the patient came in before the renewals came due, the physician could determine whether the medication was effective, and whether the dose was right before signing off on the next round of pills. The physician feels the out-of-sync schedule they've established is a time-wasting hassle, inefficient, unsafe, inaccurate, inconvenient and pointless.

电子病历系统能够让医生同时续多种药品。既能节省时间又能降低差错。设计一款能够按照"续药到期日"、“药房”、"处方医生"来排序和过滤用药列表的电子病历系统能够最小化医生
的认知负载，让他们能够提供更好的以患者为中心的服务。

An EHR can allow a physician to renew multiple medications at the same time. This saves time and reduces the margin for error. Designing an EHR that can sort and filter the medication list by “renewal due date,” “pharmacy” and “prescribing physician” will minimize physicians' cognitive load and allow them to provide better patient-centered service.

医生和服用多种药物的患者常常为不良的同步续药所累。这些续药总是安排在每个月不同的日期内，年度续药到期日分散在一年之内。如果医生能够轻松地理清楚那种药需要在下次预约之前续药的话，医生就可以整合病人的处方。
这样就能够减少医生的工作量，对于患者而言也更加方便。

Patients with multiple prescriptions and prescribers are often burdened with poor refill synchronization. Their refills come in on several different dates each month, and their annual renewal due dates are scattered throughout the calendar year. If physicians could easily discern which prescriptions require renewal before the next planned appointment, the physicians could consolidate their patients' prescriptions. This would reduce the physicians' workload and would be more convenient for the patients<sup>1</sup>\.

设计人员要让用户能够很容易地修改已有的处方，保存已有的详细信息，在用户需要改动时能够轻松访问常见替代品的信息(比如从10mg变到20mg，从1片到2片，从30天到90天等)。

Designers could allow users to easily modify existing prescriptions, preserving existing details and offering easy access to common alternative details where users might need to make changes (changing from 10 mg to 20 mg, from 1 tablet to 2 tablets, or from 30 days to 90 days, etc.).

Gallery 5.2 **Allow Sorting and Filtering to Efficiently Facilitate Renewals**

*   5.2 a Sorting the List by Renewal Due Date**>— Makes it easier to group and manage the medications due for renewal.

![Sort by Renewal Due Date](./assets/images/examples/eRx/UM_EHR_0012_sort-renew.png)

*  5.2 b  Filtering the List by Prescriber**>— Makes it even easier to focus only on the selected medications, eliminating distracting items.

![Filter by Prescriber](./assets/images/examples/eRx/UM_EHR_0013_filter-physician.png)

图5.4([Figure 5.4](#fig-5-4) below)中以条形图展示"续药到期日"来减少用户的认知负载。这样，医生快速浏览之后，就可以知道在本次诊疗过程中需要管理哪些条目，
通过挑选 preattentive attributes，诸如颜色，线的长度而不是通过阅读日期、数量和续药数量来进行计算，医生就可以知道需要关注的是哪些药品。

A bar graph data visualization ([Figure 5.4](#fig-5-4) below) displaying “renewal due dates” reduces users' cognitive load.. It allows physicians to note which items need to be managed during the current visit by doing a quick visual scan. The physicians recognize what medications they need to focus on by picking out preattentive attributes, such as color and line length, rather than by having to do complex mental calculations involving reading dates, quantities, and number of refills.

Figure 5.4 **Icons for “Refills Remaining”**>— Icons use preattentive attributes to reduce cognitive load during the medication renewal process

![Icons for Refills Remaining](./assets/images/examples/eRx/RenewalDue_Icons_PCTouchCerner.png)

From Cerner PowerChart Touch. © 2014 Cerner Corporation. Reproduced by permission of Cerner Corporation.

---

### 5.2 计算机辅助医嘱录入 Computerized Physician Order Entry (CPOE)

CPOE就是能够电子化录入患者医嘱的系统，医嘱能够以电子化方式发送给其他科室(影像科、检验科等)或者其他机构来执行。CPOE的医嘱能够比之前的系统更加快地传递。能够杜绝手写产
生的错误，根据核对已有医嘱避免重复医嘱的情况。

A CPOE (also sometimes referred to as*Computerized**Provider** Order Entry*) is an electronic entry of patient care orders that electronically transmits itself to the departments (lab, radiology, etc.) or outside organizations that will fulfill it. CPOE orders can be distributed more quickly than their predecessors. They eliminate errors based on hand-writing, and can prevent duplicate orders by checking new orders against existing orders.


>#### 临床场景——下达实验室医嘱 Clinical Scenario — Placing Future Lab Orders


>马丁先生已经把自己的糖尿病、血压、血脂控制的很好。在过去的一年内，服用固定剂量的药物，实验室检验结果也很稳定。现在他可以进入一个更可控的疗程，无需频繁的看医生和做检验。
在六个月之内，马丁先生需要进行一次hemoglobin A1c lab 血红蛋白的实验室检查，然后来看一次一生。在这之后的六个月，他需要完成后续的检查(另外一次血红蛋白和空腹血脂的检查)
，然后再看一次医生。

>Mr. Martin has achieved good control of his diabetes, blood pressure, and lipids. For the past year, he's been on stable doses of his medications, and his lab results have been stable as well. He can now settle into a more predictable routine, and won't need to visit the office or undergo lab tests as frequently. In about six months, Mr. Martin will need to come in for a hemoglobin A1c lab test, and then a visit. Another six months after that, he'll need to come in for further tests (another hemoglobin A1c a fasting lipid profile and a urine microalbumin test, both for his diabetes), and then another office visit.


#### 5.2.1 展示已有的医嘱以避免重复 Display Pre-Existing Orders to Prevent Duplication

患者的电子病历常常包含一些没有执行的医嘱。患者会忘记去做检验，或者没有时间去做。如果医生看不到患者已经下达的或最近的检验结果，他们可能会不小心下已经已经下过的或已经执行的医嘱，
或者类似的检查检验。这样子就增加了同事的工作量，浪费了资源。

A patient's EHR often contains unfulfilled orders. Patients forget tests, or can't find the time to get them done. If physicians can't see patients' existing future orders or recent lab results, they may accidentally order tests that have already been done or ordered, or very similar tests. This would duplicate their colleagues' work and spend resources wastefully.

当用户下达医嘱时，他们能够同时看到已经完成的医嘱，无需从当前未完成的医嘱中切换出去，就不会丢失自己的工作。

When users place new orders, they can simultaneously be able to see the work that's already been done, without navigating away from their own unfinished orders and losing their work.

Figure 5.5 **Before: Interruptive Dialog Box**>— Doesn’t allow the physician to see existing prescription orders

![Dialog doesn’t allow the physician to see existing orders](./assets/images/examples/eRx/UM_EHR_0004_new-medication-bad.png)


Figure 5.6 **After: Non-interruptive Dialog Box**>— Allows users to see existing orders using a separate panel, or by making the dialog box non-interruptive. 

![See Existing Orders in a separate panel, or a non-interruptive dialog box](./assets/images/examples/eRx/UM_EHR_0003_new-medication.png)

#### 5.2.2 简化查找恰当的医嘱 Make It Easy to Find the Right Orders

由于检查检验和手术操作常常优多个常用的名称，医嘱的命名是很有挑战的。同样的检验，不同的机构可能使用不同的名称。医生下医嘱的时候可能会
不熟悉电子病历系统医嘱目录中的名称，电子病历系统中可能会把X光称为"XR chest"，医生可能会在以下条目中查找：

-	chest x-ray (or variant spellings like “xray”)
-	chest XR
-	XR chest
-	X-ray chest
-	Chest x-ray 2 views
-	Chest x-ray PA and Lateral
-	CXR (fastest way to hand-write the order)

Naming orders can be a challenge, because tests and procedures can have several commonly-used names. Different organizations may use different names for the same test. The physician ordering procedures might not be familiar with precise names listed in the EHR order catalog. The EHR might formally call a chest x-ray "XR chest". A physician, however, might look for it under:

-	chest x-ray (or variant spellings like “xray”)
-	chest XR
-	XR chest
-	X-ray chest
-	Chest x-ray 2 views
-	Chest x-ray PA and Lateral
-	CXR (fastest way to hand-write the order)

这些都是正确的命名x光的方式。因此，界面中要能够让医生根据常见名称来查找检查检验和手术操作。

These are all correct ways to name a chest x-ray. Thus, the interface could allow physicians to find tests and procedures listed under their various commonly-used designations.

#### 5.2.3 预先配置好详细信息尽可能丰富的医嘱 Preconfigure Orders with as Much Detail as Possible

医生在急诊室或紧急诊疗情况下所下达的检验医嘱通常优先级很高，需要STAT执行。在全科诊室中医生所下达的常规检验医嘱优先级总是较低。可能是要今天完成，将来完成或以后某个
规定的时间内完成。要能够很容易的根据特定的care setting配置电子病历系统，能够为它所要处理的医嘱准备好默认的优先级设置会成为很强力的工具。

Tests physicians order in ER or urgent care scenarios are often high priority and need done STAT. Routine tests physicians order in primary care settings will almost always be lower-priority. They'll need completed today, in the near future, or at some specified future time. An EHR that could be easily configured to a specific care setting, one that established default "priority" settings for the orders it processed, would be a powerful support tool.

>#### 利用模糊日期来设置医嘱日期 Setting the Date for Orders: Using Fuzzy Dates

>有时候医嘱要求是精确的日期和时间。持续三天重复血浆凝血酶原时间能够保证warfarin(一款抗凝血药物)剂量正确。


>Sometimes orders demand a precise date and time. Repeating a Prothrombin Time (PT) lab test in exactly 3 days helps assure safe dosing of warfarin, a clot-preventer.

>有时候，日期不是那么精确可能更有用。如果医生下达了一个"一年以后"的实验室检验，但患者11个月后就来就诊，告诉患者来得太早让患者回去显然是欠妥的。电子病历系统要让用户能够
灵活的模糊日期。这样医疗机构就能够让患者选择自己合适的日期和时间来就诊。

>Other times, less precise dates would be more helpful. If a physician orders a lab for "one year from now," but the patient shows up eleven months later, telling the patient she's too early and sending her home would be counterproductive. The EHR needs to allow its users to set somewhat flexible "fuzzy dates." This will allow healthcare organizations to be adaptable, and to work with patients to find times and dates convenient for them.

Figure 5.7 **Before:**>The physician needs to expend a lot of effort to fill in the many missing details. There are many opportunities for error.

![More effort is required to fill in missing details](./assets/images/examples/eRx/UM_EHR_0006_new-medication-unfilled.png)

Figure 5.8 **After:**> The EHR pre-completes key fields. Less frequently needed details are displayed less prominently.

![Pre-complete key fields and Display less frequently needed details less prominently](./assets/images/examples/eRx/UM_EHR_0005_annotated.png)

#### 5.2.4 为医嘱或处方分配正确的诊断信息 Assign the Correct Diagnosis for an Order or Prescription

在医生键入医嘱时，电子病历系统能够让疾病和诊断信息显示给医生。也能够让医生无需退出当前的医嘱工具来添加新的诊断。

The EHR can make the problem and diagnosis lists readily available to physicians entering orders. It could also allow users to add new diagnoses on the fly, without having to exit the ordering tool to add them.

(这段 patients' list entries  list前面好像是缺了个词 )根据患者的xx列表条目和实验室检验结构，电子病历系统能够通过给出疑似诊断来提供决策支持。有时候，医嘱几乎只与一种诊断相关，这种情况下，系统要能够默认地分配诊断给这些医嘱。
比如，血红蛋白的检验项目总是和糖尿病或高血糖有关。

The EHR can provide clinical decision support by suggesting probable diagnoses based on patients' list entries and lab results.Some orders are almost exclusively associated with a single diagnosis, and in these cases the system could assign this diagnosis to these orders by default. For instance an order for a A hemoglobin A1c lab test will almost always be associated with a diagnosis of diabetes or hyperglycemia.

#### 5.2.5 EHR系统要能够配合用户，而不是用户配合系统 EHRs Can Adapt to Users, Not Users to EHRs

一个适应性强的EHR电子病历系统能够让医生“添加到购物车” ([Figure 5.9](#fig-5-9))，继续“购物”，不用马上付款。这样子医生和患者能够做出初步的决策，立刻响应，同时又能够在就诊过程中进行调整。

An adaptable EHR can let physicians “add to the shopping cart” ([Figure 5.9](#fig-5-9)), then “continue shopping” without checking out right away. This allows the physicians and patients to make preliminary decisions, and act on them immediately, but also allows them to make adjustments as the visit unfolds.

Figure 5.9 **New Order Workflow**>— EHRs must offer users the option of building sets or collections of orders to facilitate their workflow.

![Build sets or collections of orders to facilitate workflow](./assets/images/examples/eRx/neworders.png)

#### 5.2.6 形成类似清单的成组医嘱 Building Groups of Related Orders Function like Checklists

电子病历系统必须能够为用户提供成组医嘱的选项来优化工作流程。这样子让用户提供个性化的临床决策支持，免于让医生依赖记忆或外部材料来完成工作。
比如健康儿童的问诊就遵循可预测的模式。通常包括常规的免疫接种，预定的时间间隔，特殊的咨询(预期指导)，和一系列随访。

EHRs must offer users the option of building sets or collections of orders to facilitate their workflow. This offers users personalized clinical decision support and frees them from having to depend on their memories or external reference materials to complete involved tasks. Well Child Visits, for example, follow predictable patterns. They involve immunizations at regular, predetermined intervals, specific counseling (anticipatory guidance), and set follow-up visits.

4个月大的健康婴儿的问诊包括：

-	预约六个月后的下次问诊
-	注射多种疫苗
	-	hemophilus B
	-	rotavirus
	-	pneumococcal 13-valent
	-	combination of diphtheria / hepatitis B / pertussis - acellular / polio / tetanus.
	
A four-month-old's Well Child Visit would include:

-	scheduling the next visit, at six months
-	administering several specific vaccines
	-	hemophilus B
	-	rotavirus
	-	pneumococcal 13-valent
	-	combination of diphtheria / hepatitis B / pertussis - acellular / polio / tetanus.
---

### 5.3 总结

电子病历能够:

1.	提供能够推荐合适结果的搜索功能，简化用户选择新医嘱。
2.	尽可能地填充默认值(30或90天的处方补给)
3.	记住患者的药房选项，能够移除患者不再需要的药房
4.	使用 preattentive attributes,诸如颜色、字体来强调，让医生更加快速地找到可能的结果。使用颜色图标来图形化展示药物续药到期日期。
5.	在发送电子处方之前能够让医生进行审核以校正错误
6.	能够对用药列表排序和过滤来加速续药的流程
7.	能够根据已有医嘱进行修改而不是从头开始录入
8.	能够个性化设置界面，内置诸如清单的足够详细的成组医嘱套餐
9.	能够为新医嘱选择特定或灵活的日期

1、insurance formulary 处方集          
2、pharmacy benefit plan 药房福利方案       
3、 combination analgesics 复合镇痛药        
4、 Review the New Prescription Order 可作处方核实、处方审核解        
5、drug’s therapeutic class      
6、续药 Renewing Medications      
7、计算机辅助医嘱录入 Computerized Physician Order Entry (CPOE)       
8、Checklists      

