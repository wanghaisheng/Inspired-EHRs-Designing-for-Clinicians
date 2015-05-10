## 2

## 用药列表


有效的用药管理是患者医疗保健中很重要的部分。

* * *


用药列表记录了患者当下正在服用的所有药品和规定的剂量相关的信息。用药列表可以是多种形式，这章中只关注三类：**简单的列表形式**、**交互式列表形式**、**时间轴形式**。同时我们会给大家提出一些建议和存在的挑战。

Medication lists record information about all the drugs a patient is currently receiving and their prescribed dosages. Medication lists come in many forms, but this chapter will only focus on three:**simple lists**,**interactive lists**, and**medication timelines**. We’ll offer a few tips and challenges along the way.

Gallery 2.1

2.1 a **简单的列表形式**— 能够帮助医生完成多种工作，比如做出治疗决策，完成电子处方。
![A simple medication list](../images/SimpleList_ReduceNoise.png)

2.1 b **简单的列表形式**— 也很适合患者在移动端访问。
![Simple lists are also good for mobile](../images/SimpleListMobile.png)

2.1 c **交互式列表形式**— 包含了更多有关用药的详细信息，能够帮助医生完成多种工作，比如做出治疗决策，完成电子处方。
![An interactive table as a medication list](../images/UM_EHR_0000_table.png)

2.1 d **时间轴形式**— 充分利用了信息可视化的作用，能够让医生掌握随着时间推移用药情况的变化。
![A medication timeline](../images/UM_EHR_0000_Annotated-Timeline.png)


* * *

### 2.1[简单的列表形式](http://inspiredehrs.org/simple-list/)


简单的列表形式只是展示一些基本信息。这是为了快速阅读，一眼就能扫完。视觉上一眼就很容易了解药品名称、规格和剂量。列表是按照字母顺序排列的，这样检索和定位某个项目也很容易。这样，能够让用户，通常也就是医生能够对患者的病史和用药有个整体把握。医生在快速扫完列表之后能够做出一些最初的观察，比如总共有24种药物，但只有2种治疗高血压的处方药。良好的设计能够让这些工作变得很容易，糟糕的设计会变得很复杂。

The simple list displays bare-bones basic information. It’s made to be read quickly, scanned at a glance. It’s easy to scan visually to see the name, strength, and dosing of the medication. The list is alphabetical, which makes it easy to search for and locate particular items. It gives the user, usually a physician, a broad overview of the patient’s medical history and their related medications. A physician quickly scanning the simple list can make initial observations such as,_“There are twenty-four medications here, but only two prescription medications for high blood pressure.”_ Good design can make such tasks easy; bad design can make them much harder.

这里我们提到的“患者”不仅是病人自己，也包括能够代表患者的护理人员或家庭成员。类似的，我们提到的”医生”不仅仅是只医生，也包括其他具有处方权的医务人员。

We use the term “patient” to apply to either patients themselves, caregivers, or family members acting on their behalf. Similarly, we use the term “physician” to apply to physicians proper or other healthcare professionals with prescribing authority.

>#### 常见场景——门诊诊查

>内科医生Dr.Barnes正准备走进检查室查看她的病人Mr. Martin马丁先生，马丁先生60岁，6患有10种慢性病(糖尿病、高血压、高胆固醇、膝关节炎、抑郁症、失眠等等)，服用着17种药物。医生注意到患者的血压偏高十个点，打算询问患者是否在家里测量过自己的血以及测量的结果。

>Dr. Barnes, a general internist is about to go into the exam room to see her patient Mr. Martin, a 60-year-old man with ten chronic diseases (diabetes, high blood pressure, high cholesterol, knee arthritis, depression, insomnia, etc.) who is taking seventeen medications. The physician notes that the patient’s blood pressure is about ten points too high. She plans to ask the patient if he has been taking his blood pressure at home and what the results of any such tests have been.

在这个场景中，在面对面的诊查开始之前，医生需要对患者所有的用药情况、慢性病病情、最近的生命体征指标和相应的实验室检验结果等了然于胸，(病人有没有在服用胰岛素？有没有吃任何的高风险药物如华法林？)。有了这些基础信息之后，医生才能够把注意力都放在病人讲述自己的病情，不用在病人和电子病历系统屏幕间来回切换以提醒他患者的用药信息。把全部注意力都放在病人身上,向病人展示了医生是在用心倾听，而且是关心病人所说的话。建立语境能够让医生专心在这次就诊的实用性和情感基调上，将这次就诊与全局联系起来，其中包括了患者既往和当前数据以及患者对病情的讲述。

In this scenario, the physician needs to have an overall awareness of the patient’s medications, chronic problems, latest vital signs, and relevant lab test results fresh in her mind when the face-to-face visit begins. (“Is he taking insulin? Is he on any high-risk drugs like warfarin?”) Armed with this background, the physician is able to give her full attention to the patient telling his story, and she won’t have to keep glancing away from him and back at the EHR to be reminded of the medications. Giving full attention to his story shows the patient that she’s listening to and cares about what he has to say. Establishing context will allow our physician to attend to the practicalities and the emotional tone of this encounter, and to frame this visit in relation to a bigger picture that includes the patient's past and current data, his story.

>#### 情境意识、态势感知Situational Awareness

>态势感知也就是说拥有做出高效决策的所有背景知识的同时，了解当前你身边所发生的一切，预见未来会发生的。在门诊过程中管理慢病的医生而言，态势感知包括了
在患者走进诊室之前，获取全面的有关患者的关键信息。在患者进入诊室之后，医师就能够把注意力集中在患者身上，并根据眼前的患者进行调整，进行交谈。

>Situational awareness is having all the background information you need to make effective decisions while simultaneously being aware of what is currently happening around you and anticipating what will happen in the near future. For physicians managing chronic diseases during ambulatory visits, situational awareness consists of taking in a broad overview of key information about patients before walking into the exam room. Upon entering the exam room, the physician can then be mindful of and attuned to the patient sitting before them and the unfolding of their conversation.

>如果由于时间上的压力或信息混乱，Dr. Barnes走进诊室时并没有做好100%的准备，她将争取听懂患者的疑虑/担心。[信息混乱](./human-factors.php#info_chaos)
包括信息过载、不足、分散、传统和错误信息。相反，在患者讲话的时候她将会在电子病历系统中进行检索，疯狂地企图填补知识的不足。患者会意识到医师注意力的分散，可能会认为医师没有好好听他讲话，
会感觉患者自己被排除在自身身体健康和问题决策之外了。由于医师的注意力被分散了，医师可能会遗漏一些患者讲述的重要细节。

>If Dr. Barnes enters the exam room half-prepared due to time pressure or information chaos, then she’ll struggle to listen to the patient’s concerns.[Information chaos](./human-factors.php#info_chaos)(See Information Chaos in the Human Factors chapter) comprises information overload, underload, scatter, conflict, and erroneous information. Instead, she’ll search through the EHR while the patient speaks, frantically trying to fill the gaps in her knowledge. The patient will sense the physician’s distraction, and may feel that he’s not being heard, that he is being left out of decisions that concern his body and wellbeing. The physician may miss something important, telling details about what the patient says because she is distracted.

从[Figure 2.1](#fig-2-1) 和[ Figure 2.2](#fig-2-2)你可以看出，一个列表看起来比另一个整齐。这样的一些简化能够让使用此类列表的用户一眼就看到患者正在服用的药物名称。考虑到其中使用的如“一日两次”
这样平常的语言而非拉丁的简写如"b.i.d"，如下所示的列表能够同时满足医师和患者的需求。

Look at[Figure 2.1](#fig-2-1) and[ Figure 2.2](#fig-2-2). As you can probably tell, one list looks cleaner than the other. Such simplicity makes it easy for people using this list to see the names of the drugs the patient is taking, which allows a quick overview. Given that it uses plain language like “twice daily,” instead of Latin abbreviations like “b.i.d.,” the list below would meet the needs of both physicians and patients.

Figure 2.1 **Before: An Awful Medication List**
![Figure 2.1 **Before: An Awful Medication List**](../images/EHR_SimpleList_Before.png)
Figure 2.2 **After: Simple Medication List Makeover**
![Figure 2.2 **After: Simple Medication List Makeover**](../images/EHR_SimpleList_After.png)


患者也可以使用这样的列表。患者能够轻易的讲这样的列表拿给其他医师、牙医、急诊室的工作人员或其他护理人员看。需要填写每周用药提醒表单的患者可能会需要一种更加详细的列表-
能够说明表单中不同部分的具体内容，更加明确的区分每天的什么时段应该服用那种剂量的药物。

Patients can also use this list. Patients can easily show this list to other physicians, dentists, emergency room staff, or their caregivers. Patients filling up weekly medication reminder boxes might, however, need a more detailed list —perhaps one that illustrates the contents of each compartment of their box, and more clearly differentiates the time of day at which they should take each dose of medication.

医师或护士希望能够拿到之前就诊过程中的形如这种简化格式的病程记录，病历概要，或者是其他电子病历系统产生的就诊总结。这只是一个快照，旨在扫一眼。医师在进行更加复杂的任务如电子处方时可能更倾向于一种交互式的展现方式，能够有更多的信息，比如交互式的表格或者是用药的时间轴。

A physician or nurse would expect a progress note from a previous visit, a dashboard overview, or a visit summary from an outside EHR to make use of this simple format. It’s a quick snapshot, intended to be taken in at a glance. A physician doing a more complex task, like e-prescribing, might prefer an interactive display with more information, such as the interactive table or the medication timeline.

在这样的语境下，医师只需要扫一眼药物的名称。避免在这里添加额外的细节信息。简洁的列表更易于医师阅读。医师无需知道药物的数量、起止日期时间或者在某次处方中重复拿药的数量。如果列表中使用的是商品名，一定也要包括药物的通用名。处理商品名、通用名和化学名是很具挑战性的。

In this context, the physician just needs to quickly see the medications’ names. Avoid the temptation to add extraneous detail here. Concise lists are easier to read. Physicians don’t need to see the medications’ quantities, start dates, or the number of refills in a given prescription to perform this task. If the list uses a brand name, be sure to include the product’s generic name as well. Dealing with brand, generic, and compound names can be a challenge (see the following note).
>#### 挑战：商品名和通用名的处理

>这是很棘手的，我们承认：是否在用药列表中展示药物的商品名或通用名，或者2种同时展示，可能并不存在一个正确的答案。具体取决于语境/具体情况和参与对话的人。
电子病历系统能够轻松地获取所有相关药物的通用名和商品名。但在获取时诸多因素会使整个问题变得复杂。

>This can get tricky. We’ll admit right now: there may not be one correct answer to the problem of whether to show the brand name, the generic name, or both names by default in medication lists. It depends on the context, and the people in the conversation. The EHR can offer easy access to both the generic and the brand names of all relevant drugs. But several factors complicate the question of the form this access could take.

>如下是一些考虑因素。

>Here are a few considerations.

>理想情况下，在正确的时间应该按需展示2种名称即可。有时候，同时展示商品名和通用名是比较好的——比如 “呋塞米片furosemide (Lasix) 20 mg.”。
为了保持一致性，根据通用名来进行字母排序。但如果你使用的是打印列表，你可能得选某一种展示方法。由于通用名可能难以记忆或发音，即使是医师，大家在对话中常常更倾向于使用
商品名。尝试下面快速读下面的名称3次：

>*   阿达木单抗adalimumab — Humira
>*   枢复宁ondansetron — Zofran
>*   furosemide — Lasix

>Ideally, both names would be available on demand at just the right time. Sometimes it may be appropriate to display both generic and brand name —for example “furosemide (Lasix) 20 mg.” For consistency, sort alphabetically by the generic name. But if you’re working with a printed list, then you might have to choose a single method of display. People often prefer to use brand names in conversation because the generic names may be difficult to remember or pronounce, even for for physicians. Say these three times fast:

>*   adalimumab — Humira
>*   ondansetron — Zofran
>*   furosemide — Lasix

>此类问题常常与一些药品有多种易弄混淆的商品名牵扯在一起。比如，Diltiazem地尔硫卓，可能是：
>*   Cardizem
>*   Cardizem LA
>*   Cardizem CD
>*   Cartia XT
>*   Dilacor XR
>*   etc., etc.

>The problems are compounded by the fact that some medications have many confusing non-interchangeable brand names. Diltiazem, for example, may be available as:

>*   Cardizem
>*   Cardizem LA
>*   Cardizem CD
>*   Cartia XT
>*   Dilacor XR
>*   etc., etc.

>在和患者讨论药品的时候，医师需要知道那些病人也知道的药物的名称。由于药物名称写在药房配药时的药瓶上，或者是某个名称更易于记忆或发音，患者可能对某个版本的药物名称比较熟悉，
。在和患者谈话的时候，医师会发现同时说出药物的两种名称会更有帮助一些(“Your furosemide, also called Lasix”)。同时展示2种名称，特别是那些罕见药，
可能会减少认知负荷。
When discussing medications with patients, physicians need to be aware of the name of the drug as the patients know it. Patients may be more familiar with a particular version of a drug’s name because it is what is written on the medication container dispensed by their pharmacy, or because that version of the name is easier to recall or pronounce. When speaking with patients, physicians might find it helpful to refer to drugs by both names (“Your furosemide, also called Lasix”). Having both names displayed, especially for less common drugs may decrease mental effort.


我们可以通过**强调**药物名称和de-emphasizing其他内容的方式让用药列表易于阅读。医师的眼睛需要更多的注意药物名称和规格而非整行内容。尽管在一些情况下诸如
"每日一片"这样的用法用量也很重要，但这都是次要的信息。其中一种用于表示次要信息的方法是使用灰色文本。这些灰色文本和其余内容的差别不会太极端，因此不会带来视觉上的困扰，反而会直接作用于人类大脑的
[视觉处理系统> (See How People Perceive in the Human Factors chapter)</span>](./human-factors.php#how-people-perceive).与这些稍微显暗的文本相比，加重的药物名称将会是“[preattentive attributes](./human-factors.php#preattentive-attributes)"<span class="print-only"> (See Preattentive Attributes in the Human Factors chapter)</span>，我们的大脑很容易的区分和将其标记为重要信息。

We can make medication lists easier to read by**emphasizing** the names of drugs and<span class="grey">de-emphasizing</span> everything else. Physician’s eyes need to notice the names and strengths more than they need to take in the whole line of text. Dosage instructions such as “take 1 tablet daily,” while important in some contexts, are secondary pieces of information. One method of denoting that these instructions are of secondary importance is to use gray text. The difference between this gray text and the rest won’t be extreme, and thus won’t be visually jarring, but it**will** be immediately apparent to the human brain’s[visual processing system<span class="print-only"> (See How People Perceive in the Human Factors chapter)</span>](./human-factors.php#how-people-perceive). Compared with this light gray text, the black medicine names will possess the “[preattentive attributes](./human-factors.php#preattentive-attributes)"<span class="print-only"> (See Preattentive Attributes in the Human Factors chapter)</span> our brains readily detect and flag as important.

Gallery 2.2 **Making Added Emphasis to Text Just Right **

2.2a  **Too jarring**

![](../images/too-jaring.png)

2.2b  **Too subtle**

![](../images/too-subtle.png)

2.2c  **Invisible to color-blind users**

![](../images/invisible-to-blind.png)

2.2d  **Just right**

![](../images/just-right.png)

另一方面，有时候，[deliberately jarring](./design-principles.php#dark-side-of-color)能够引起用户的注意。一些EHR使用**tall man lettering**
来区分那些会引起混淆的看起来像和或听起来像的药物名称。Tall man lettering通过大写单词的某部分将其与邻近的单词区分开： hydrALAzine vs. hydrOXYzine.
这种不同寻常的看起来“不正确的”大写方式在告诉用户，“这里要注意，这部分是很重要的”。HydrALAzine是一种控制血压的药物而hydrOXYzine是抗组织胺药，差之毫厘,谬以千里。

On the other hand, sometimes a[deliberately jarring](./design-principles.php#dark-side-of-color)<span class="print-only"> (See The Dark Side of Seeing Color in the Design Principles chapter)</span> type style alerts the user to pay attention. Some EHRs use**tall man lettering** to differentiate look-alike and/or sound-alike drug names that might otherwise be easily (and dangerously) confused. Tall man lettering capitalizes the parts of a word that separate it from its near-doppelgangers: hydrALAzine vs. hydrOXYzine. This unusual, seemingly “incorrect” capitalization says to the user, “Hey, pay attention here, the part I’ve emphasized is really important.” HydrALAzine is a blood pressure medication, hydrOXYzine is an antihistamine. Small differences matter.

>#### 前注意属性 Preattentive Attributes

>前注意属性是那些人们下意识的注意到并能够快速理解的细小的视觉物体，快到我们只能够注意到这是下意识的。尝试一下下面的测试，能够帮助你理解我们探讨的是什么


>Preattentive attributes are the little visual things people unconsciously notice and understand quickly, so quickly that we have only noticed it at an unconscious level. Try this little exercise, which can help you understand what sort of things we’re talking about.

>**下面的矩形中分别有多少个5？**

>**How many fives do you find in each rectangle below?**

![Find the fives in a grid of numbers](../images/findthe5s.png)

>在右图中更加容易找到5是由于我们的大脑无需意识控制就能接受加黑的字体。

>It’s much easier to spot the fives in the right-hand figure because our brain perceives the bold characters without our conscious volition.

>在处理视觉信息时，我们的大脑能够将最基本的属性(形状、大小、方向和动作)整合成对我们有意义的"对象"。这个过程十分快，在我们意识到之前。其中一些特性更加突出，
更加易于被注意到。这些特性被称之为[前注意属性preattentive attributes](./human-factors.php#preattentive-attributes)

>When processing visual information, our brains combine very basic attributes (shape, size, orientation, motion) into “objects” that have some meaning to us (face, pole, box). This happens very quickly, below the level of our conscious awareness. Some features stand out more readily and are noticed more quickly than others. Those features are called[preattentive attributes](./human-factors.php#preattentive-attributes)<span class="print-only"> (See Preattentive Attributes in the Human Factors chapter)</span>.


按字母顺序给列表排序。读者期望列表中的文本是按照字母顺序排列的。这样能够让他们在比较长的列表中快速找到某些名称。“你是否在服用 warfarin”。只需要跳到“w”
的部分去找就可以了。

Alphabetize the list. Readers expect a list of text items to be alphabetical. This helps them find particular names quickly in long lists. “Are they taking warfarin?” Just jump to the “w” section to check.

减少视觉噪声。如果某个视觉元素不能增加或提高信息处理或感知的能力，尝试移除这些元素。参考[ Figures 2.3](#fig-2-3) and[2.4](#fig-2-4)

Reduce visual noise. If a visual element doesn’t add data or improve the perception or processing of information, try leaving it out. See[ Figures 2.3](#fig-2-3) and[2.4](#fig-2-4).

Figure 2.3    **Before: The Frame Creates Visual Noise**
[![A simple list as a table with thick borders](../images/SimpleList_Noisy.png)

Figure 2.4    **After: Cleaner, Data Takes Center Stage**
[![A cleaner simple list with clear information hierarchy](../images/SimpleList_ReduceNoise.png)

边框并没有添加信息，移除边框能够让你的数据减少视觉噪声。

Borders don’t add information, and removing gridlines can make your data less visually noisy (and thus easier to read).

接下来，让我们来了解一下交互式表格
Now, let’s move on to the interactive table.

* * *

### 2.2 [The Interactive Table](http://inspiredehrs.org/medication-list/)

交互式表格允许用户进行排序、筛选，根据自己当前任务的需要调整展示界面。这个表格是电子病历系统的标配，有些时候可能是唯一可以看到的内容。
这个表格足够灵活和强大，能够适应多种任务的需要，和简单的列表比起来，它也可以很复杂，可能需要更多功夫来学习和使用。
交互式列表能够在多种任务中发挥作用，比如做出治疗决策和电子处方。这个列表中甚至可能会包含存储在电子病历系统中的其他数据，如诊断、实验室检验结果和生命体征。在我们的三个例子里，该列表中展示了大多数新兴，能够给紧张的认知任务提供最大程度的支持。

The interactive table allows users to sort, filter, and otherwise adjust their displays to meet the needs of the tasks at hand. This table is the standard workhorse of an EHR, and may sometimes be the only view available. The table is sufficiently flexible and powerful to adapt to fit a variety of tasks, but it can also be complex and may require more effort to learn and use than a simple list. Interactive lists help with a variety of tasks, such as making treatment decisions or e-prescribing. The list might even be able to draw on other data stored in the EHR, such as diagnoses, lab values or vital signs. Of our three examples, this list displays the most information and can provide the best support for cognitively intense tasks.

[Interactive 2.1](#int-2-1)给出了一个交互式表格的范例。默认情况下，这类表格是按照药物名称的字母顺序排列的。
医师可以对某列数据进行排序以获取对药品新的认识以及支持药物medication renewal的多种功能。但并非所有的列都需要排序
，比如，按照用法用量或规格排序对于医师来说就没有多大用处，但按照药物名称来排序(能够按照字母来浏览和查找药物名称)、按照起止日期时间、诊断名称、
下达处方的医师姓名就很有用。

[Interactive 2.1](#int-2-1) shows an example of an Interactive Table. By default, such tables are sorted alphabetically by medication name. Physicians can sort columns of data to gain new insight into the medications and have support for various functions of medication renewals. Not all columns need to be sorted, however. For example, a physician would not find it helpful to sort by the instructions or quantity prescribed, but would find it useful to sort the list by drug names (allowing the physician to scan alphabetically, looking for a specific name), by dates (starting, renewal due, etc), diagnoses, and prescriber names.

Interactive 2.1 Interactive Table Prototype —[Try it out!](http://inspiredehrs.org/medication-list/)

![Interactive table as a medication list](../images/UM_EHR_0000_table.png)


>#### 回到之前的临床场景——血压过高

>走进诊室之前，Dr. Barnes 了解到Mr. Martin先生一直以来按规律锻炼，饮食正常。Mr. Martin先生正在服用17种药物。
Mr. Martin先生能够忍受这些药物并按时服用。今天他的血压偏高10个点，这和他在家里时量的一样高。Dr. Barnes 想要对
抗血压药物进行一些调整来更好的控制血压。

>Upon entering the room, Dr. Barnes learns that Mr. Martin has been exercising regularly and eating a healthy diet. He is on seventeen medications. He is tolerating them well, and taking them consistently. His blood pressure is about 10 points too high today, however, and it has been similarly elevated when he measured it at home. Dr. Barnes wants to adjust his blood pressure medications to achieve better control.

>Dr. Barnes 查看了交互式的用药列表，根据诊断名称对药物进行排序。Dr. Barnes注意到患者已经在服用三种抗血压药物。
经过一些努力，Dr. Barnes 确定这三种药物已经是最大剂量。患者需要额外开始服用另一种抗血压药物。Dr. Barnes 觉得服用
lisinopril是最明显的选择，但由于这个决定太过于明显，她开始思索患者至今未服用lisinopril是不是有什么其他隐藏原因

>Dr. Barnes turns to the interactive medication list and sorts the medications by diagnosis. She can readily see that the patient is already on three medications for blood pressure. With some effort, she determines that all three medications are at their maximum dose. The patient will have to begin taking an additional blood pressure medication. She thinks prescribing lisinopril is the obvious next step, but given that this decision does seem so obvious, our physician wonders if there’s some hidden reason why the patient isn’t on lisinopril already.


如下是医生的认知活动：

*   复查/回顾用药列表.
*   确定患者正在服用的治疗高血压的药物
*   确定患者服用的每种药物是否已经是最大剂量
    *   如果一种或多种当前服用药物未达到最大剂量，考虑是否增大剂量(this may be preferable because it won’t cost the patient a new co-pay, increase their potential drug interactions, or increase the number of pills the patient has to take).
    *   如果所有药物都已达最大剂量，医生应选择另外一种药物并将其添加至治疗方案当中。

Here’s the mental task for our physician (see[Figure 2.5](#fig-2-5)):

*   Review the medication list.
*   Identify medications for treating high BP (antihypertensives) that the patient is taking.
*   Determine if the patient is already taking the maximum dose of each of these medications.
    *   If one or more of the current medications is not at the maximum dose, consider whether that medication’s dosage could be increased (this may be preferable because it won’t cost the patient a new co-pay, increase their potential drug interactions, or increase the number of pills the patient has to take).
    *   If all the BP meds are at their maximum dose, then the physician must select an additional medication and add it to the treatment plan.

要考虑这些因素是很费脑的，幸运的是，您可以使这项工作变得更简单。

Juggling these considerations can be a lot of mental work. Fortunately, you can make the job much easier.

Figure 2.5 **The [Cognitive Load](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#cognitive-load) on Physicians Adjusting Blood Pressure Medications**

![Physician has to look at each medication, dose, and condition](../images/UM_EHR_0006_mental-work.png)

通过使用一些精妙的设计，你可以减少医疗过失的风险(用药列表中缺失某种药物)，
降低必要的[认知负荷cognitive load](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#cognitive-load)。

You can reduce the risk of error (missing one medication in the list) and decrease required mental effort ([cognitive load](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#cognitive-load)) by using smart design features.

对于如何改进用药列表，我们有一些建议。遵循[《高效表格设计指南Effective Table Design guidelines》](https://sbmi.uth.edu/dotAsset/3fc9f186-7608-4b57-9ade-64a90e5916e0.pdf)。比如，确保表头总是可见的，不会随查看而滚动
。最重要的列放在左边(这里也就是药品名称)。确保比较长的名称不会被截断，不会留下发生了什么的视觉迹象
，确保整个名称能够很快查看得到。可以在[SHARP-C website](https://sbmi.uth.edu/nccd/index.htm)的网站上查看更多表格设计的知识。

We have several suggestions for improving medication lists. Follow[Effective Table Design guidelines](https://sbmi.uth.edu/dotAsset/3fc9f186-7608-4b57-9ade-64a90e5916e0.pdf). For example, make sure table headers remain visible all the time and don’t scroll out of view. The most important columns can be on the left (in this case, drug names). Make sure long names (like those of compound drugs) don’t get truncated without leaving some visual indication that this is what happened, and make sure the entire names are quickly accessible. You can read more about table design at the[SHARP-C website](https://sbmi.uth.edu/nccd/index.htm).

**允许用户依据相关的诊断来对用药进行排序**。人们有限的工作记忆只能保留3到4种
化合物和复杂条目，比如药物的规格，日常的用法用量。

**Allow users to sort the medication list by associated diagnosis.** Humans’ limited working memory can only hold three to four compound and complex items, like medications with associated strengths and daily dosing instructions, at a given time.

>#### 工作记忆 Working Memory

>工作记忆，或者说短期记忆，能够让我们在一分钟以内回忆起一些信息片段-说出我们正在写下
来或键入手机的电话号码。我们不得不关注一些内容，将其放在我们的短期记忆里。

>Working memory, or short term memory, enables us to recall manageable chunks of information —say phone numbers we’re in the process of writing down or punching into our phones —that we need for less than a minute. We have to focus on something to keep it in our short term memory.

>要求人们阅读一页纸上的内容并记住它，写在另外一张纸上，能够训练人们的短期记忆。
在设计交互界面时，要牢记的是，问自己是否能够以让用户关注那些自己工作内容的元素的方式来展现信息。
而不是关注你的系统。尽量避免用户只从一个页面上获取信息，需要记住这些信息才能在后续页面中使用

>Asking people to look at information on one page and then remember it and use it on another page strains their short term memory. When designing interfaces, keep this in mind. Ask yourself if you can present information in a way that will allow users to focus on remembering the elements of their own tasks, rather than on engaging with your system. Try to avoid having the user get information on one page and then needing to remember it in order to use it on another page.

>[Read more on Working Memory in the Human Factors chapter.](./human-factors.php#working-memory)


只有以前的医师或医疗机构输入了引发患者处方的诊断信息的情况下才能够通过诊断
来排序。目前并不要求医师总是输入这样的信息，由于看不到明显的好处大多数都不会这么做。
但有了EHR系统，能够高效的按照诊断来排序，一次性为每个药物输入此类信息会节约大量后续的认知工作。
当医师下达一种新的药物，系统会给出患者目前的诊断或慢病列表。医师可以从
列表中点选其中一个或多个可以使用的，或者添加一种新的诊断或慢病。这本质上和医师在下达检验检查医嘱时的工作是一模一样的。


Sorting by diagnosis is only possible when previous physicians or providers have entered the information about the diagnoses that prompted a patient’s prescriptions. Currently physicians aren’t required to always give this information, and many don't because they don't see an obvious benefit to doing so. However with an EHR that effectively sorts by diagnoses, entering this information once for each medication will prevent a lot of unnecessary mental work in the future. When a physician prescribes a new medication, the system will present a list of the patient's current diagnoses or chronic problems. The physician can merely pick one or more of these from this list as applicable, or add a new diagnosis or chronic problem. This is essentially the same work physicians already have to do when sending out lab and imaging orders.

然而，按照诊断来排序的确给设计人员和开发人员带来了额外的挑战。对与不止一个的诊断相关的用药进行排序
是设计上的挑战。如何来展示与多个诊断相关的用药呢?在医疗信息交换过程中，
EHR如何来处理不同厂商的诊断信息本体？一个家庭医生可能会把condition描述成
"慢性腰背痛"，而整形外科医生则可能把同样的疾病称之为“腰椎病lumbar spondylosis”

Sorting by diagnosis does, however, present designers and developers with additional challenges. Sorting medications that are associated with more than one diagnosis will be a design challenge. How might they represent medications associated with multiple diagnoses? How might an EHR deal with different providers' ontologies for diagnoses in the context of a health information exchange? A family physician might describe a condition as "chronic low back pain," while the orthopedic surgeon might call the same problem "lumbar spondylosis."

Gallery 2.3 **Easing Mental Work** — How many current medications for hypertension? Which medication was previously used for hypertension?

2.3 a **Sorted by Condition**

*  ![Interactive table sorted by Condition](../images/UM_EHR_0001_sort-condition.png)

2.3 b **Filtered by Condition**
*  ![Interactive table filtered by Condition](../images/Um_Ehr_0002_condition-focus.png)

通过将药品名称与药品的参考信息关联起来，实现通过点击获取**剂量范围信息**。
药品信息数据库包括了每种适应症或诊断建议的最佳剂量范围。心率衰竭的最大剂量可能比高血压要大一些。

Make**dose range information** available**with a click or a tap** by linking the medication name to reference information about that medication. Drug product information databases include information about the recommended dose range for each indication or diagnosis. The maximum dose might be higher for heart failure than it is for hypertension.

利用**图标或简单的配色方案**，一眼就能看到剂量范围的信息。简单的配色方案也就是说暗灰色表示小剂量，
深灰色表示更大的剂量，黑灰色表示最大剂量，红色表示超过了建议的最大剂量，这样能很好的满足医生的需要无需点击、无需阅读也无需计算。

Make that same dose range information available at a glance by using an**icon or simple color scheme**. A simple color scheme in which light gray represents a low dose, darker gray a higher dose, solid black a maximum dose, and red a dose over the recommended maximum would reveal relative dosages in a way that elegantly meets physicians’ needs. No clicks, no reading, and no math necessary.

Figure 2.6 **Shading Displays Information about the Maximum Dose**

![Shading Displays Information about the Maximum Dose](../images/UM_EHR_0009_lisinopril.png)

在任何电子病历的表格中，都可以给每种药品添加如这里所示的小图标来表示最大剂量。
这种展示方法也能够帮助患者更好的理解他们的用药。通过这样的一些适合于医生、护士和患者的视觉设计
我们能够让电子病历系统和相应的诊疗过程，对于患者来说更加透明、更加易于理解。

In any standard EHR table view, that maximum dose indicator could be added with a single small icon for each medication, shown here. This display would also help the patient better understand their medication. By creating visual designs like this that work equally well for physicians, nurses, and patients, we can make the EHR and associated care processes more understandable and transparent for patients.

>#### 挑战：辨别最大剂量
>#### Challenge: Identifying the "Maximum Dose"

>一些药品针对不同的诊断会有完全不同的最大和最小剂量范围。比如高血压可以每日服用
10 到 40 mg的 lisinopril，但心率衰竭的患者可以每日服用5到40mg。
带状疱疹后搔痒post-herpetic neuralgia的gabapentin的最大剂量为每日3600mg
。对于gabapentin而言，必须根据肾功能来调整，随着肾功能的下降，最大剂量从1400mg下降到700mg，再到300mg每日。对于dialysis透析的患者，每日的最大剂量就只能是300mg。
开发团队需要核实药房数据库中最大剂量的数据是结构化的还是文本文字。
能够标注最大剂量并提供患者特征来按需调整剂量的电子病历系统能够帮助医生做出更加安全的决策。

>Some medications have different minimum and maximum dose ranges depending on the diagnosis they’re prescribed for. For example, 10 to 40 mg of lisinopril can be taken daily for hypertension, but a patient can take 5 to 40 mg daily for heart failure. The maximum dose for gabapentin is 3600 mg daily for partial seizures or neuropathic pain, and 1800 mg daily for post-herpetic neuralgia. For gabapentin, the maximum dose must be adjusted downward for reduced renal function and, as renal function declines, the maximum allowable dose drops from 1400 mg to 700 mg, and then to 300 mg daily. For patients on dialysis, however, the maximum dose of gabapentin is just 300 mg daily. Development teams will need to check with their pharmaceutical database provider to learn if data about maximum doses is available as discrete data rather than textual data. An EHR that signals maximum doses and provides information about patient characteristics that supports dosage adjustments can help physicians make safe decisions.

>针对儿科的剂量，年龄、体重都是影响最大剂量的因素。一些药品的剂量应该依据儿童的体表面积来计算。
能够在需要的案例中提供此类信息的电子病历系统能够为医务人员提供高效的临床决策支持。


>For pediatric dosing, age and weight introduce further variables in maximum dose calculations. Some drug dosages should be based on the surface area of a patient’s body (a function of weight and height). An EHR that provides this information in applicable cases will provide effective clinical decision support to providers.


下图 ([Figure 2.7](#fig-2-7) and[ 2.8](#fig-2-8))的例子中，我们
提到了嵌套在表格视图中的用药的时间轴。其中使用了前面介绍过的同样的配色方案
(暗灰表示小剂量、深灰表示大剂量、红色表示超过了最大剂量)


In the examples below ([Figure 2.7](#fig-2-7) and[ 2.8](#fig-2-8)), we refer to the medication timeline (described in detail later in the chapter) embedded in the table view. It uses the same color scheme described earlier (light gray text represents a low dose, darker gray a higher dose, solid black a maximum dose, and red a dose over the recommended maximum).

Figure 2.7 **List with a Column for the "Maximum Dose" Icon**

![Medication table with a row of grey and dark squares to denote whether dose is max](../images/UM_EHR_0007_dose-max.png)


Figure 2.8 **Mini-Timeline** — Shows maximum dose information for each medication

![A mini timeline in the medication table can indicate dose information and start/end dates](../images/UM_EHR_0008_timeline.png)


#### 尝试一下Try It Out

我们已经制作了一个交互式的原型，你可以尝试一下。想象一些临床任务(下面我们给出了一些建议)
在使用的时候和你们现在使用的电子病历系统中的工具与这个原型进行一个比较，
体会一下我们所做的一些调整在用户体验上的差异。尝试对使用原型完成一项任务和朋友或同事使用现有的电子病历系统完成同样任务进行计时。我们的原型是不是对你来说更加精确？

We’ve made an interactive prototype you might like to try out. Imagine a few clinical tasks (we've listed some suggestions below) and, as you work through them, compare this prototype to the tools in your existing EHR and see the difference our changes make in your user experience. Try timing yourself doing a task on the prototype and a friend or colleague doing the same task in your current EHR. Is one tool more accurate for you?

对于我们的原型，假设今天是2013年9月18日

For this prototype, assume “today” is September 18, 2013.

Interactive 2.2 **Interactive Table Prototype**  —[Try it out!](http://inspiredehrs.org/medication-list/)


![Interactive Table Prototype](../images/UM_EHR_0000_table.png)


#### 尝试如下的任务Try these tasks:

1.  患者是否在服用胰岛素insulin?
2.  患者是否在服用糖尿病相关的药物？有哪些？
3.  患者是否在服用高血压相关的药物？有哪些？
4.  我们能否安全地增加任何一种抗血压药物的剂量？如果有的话，是哪个？
5.  其中Dr. Barnes要负责任的是哪个药物？


1.  Is the patient taking insulin?
2.  Is the patient taking any medication for diabetes? How many?
3.  Is the patient taking any medication for high blood pressure (hypertension)? How many?
4.  Could we safely increase the dose on any of those high blood pressure medications? If so, which ones?
5.  For which medications is Dr. Barnes responsible?


* * *

### 2.3 [The Medication Timeline](http://inspiredehrs.org/timeline/timeline.html)

在处理拥有多种复杂慢病的患者的时
候，在管理多个如用药、实验室检查、意外的手术等干预措
施的时候，在应对多个医疗机构的多次家庭、医院或诊所就诊的时候，
医生渴望能够有一个时间轴来帮助他们管理这些复杂的数据。要审视所有的数据需要耗费巨大
的经历。即使是要掌握只有一种用药的患者的病史，医生可能需要翻阅病程记录、
用药的表格、多年以来的处方续签记录。对于第二种、第三种用药，医生可能不得不重复这样的工作来掌握患者的病史。


Physicians working with people who have many complex, chronic conditions (diseases), and managing many interventions, such as medications, laboratory tests, occasional procedures, and many visits with multiple health care providers at home, offices, and hospitals, yearn for a timeline that can help them manage all this complex data. Juggling all that data takes a tremendous amount of mental effort (cognitive load). A physician seeking to understand a patient's history with even a single medication may have to dig through progress notes, medication list tables, and years' worth of prescription renewals. The physician might then have to do the whole thing over again to understand the patient's history with a second or third medication.

用药的时间轴利用信息可视化的技术：
1.  提供了按时间顺序排列的患者用药史的概述
2.  能够让医生按需缩放该列表并对列表中的项目进行过滤
3.  按需展示信息的详细程度

A medication timeline harnesses the power of information visualization to:

1.  Provide a chronological overview of the patient’s medication history.
2.  Enable physicians to zoom in on and filter the list.
3.  Reveal details on demand.

概述信息能够背景和观点，也可能让用户有重要发现。(噢，原来六个月前患者的所有药物都发生了变化)
时间轴可视化能够帮助医生快速理清思路，快速得到一个开始结束的映像，
而非依赖我们缓慢的思考过程来阅读日期并作出计算。缩放和过滤功能能够有一些
初步的答案。医生可以深度挖掘更多的详细信息，比如用药变化的精确日期，影响用药事件的相关原因等。


The overview provides context and perspective, and may enable the user to make salient discoveries. ("Wow, all this patient's meds were changed six months ago.") The timeline visualization helps harness our fast thinking mind, which can quickly make sense of the start and stop images, rather than relying on our slow thinking mind to read dates and make calculations. Zooming and filtering can provide answers to preliminary questions or hunches. Physicians can drill down to seek more specific details, such as the exact dates of medication changes, or related facts that could influence the medical chain of events.

>#### 回到临床场景——今天之前到底发生了什么？

>#### Returning to the Clinical Scenario — What Happened Before Today?

>Dr. Barnes认为Mr. Martin的血压过高，需要新增一种控制血压的药物。
由于lisinopril是她最常用的三种抗血压药物之一，她想知道为什么lisinopril没有出现在患者的用药列表中。于是，查看了用药的时间轴，从患者的"当前用药"切换到“当前和既往用药”视图，
她注意到 ([Figure 2.9](#fig-2-9) below)以前开过lisinopril，但患者只服用了几个月而已。她想知道原因。在查找了病历之后，她发现
一份电话记录中写到患者出现长期干咳，但在停用lisinopril之后就好了。在病历中并没有其他相关的不良反应的记录，
于是Dr. Barnes将lisinopril添加到患者的过敏列表中，注明了不良反应是“咳嗽”。
如果电子病历系统支持的话，她可以在lisinopril相应的批注栏中写下“咳嗽”是“停止用药的原因”

>Dr. Barnes had determined that Mr. Martin’s blood pressure was too high, and that it would be necessary to prescribe an additional drug. She wondered why lisinopril was not already on this patient’s medication list, since it would normally be among the first three drugs she used for hypertension. So, turning to the medication timeline, she explores the patient’s medication history by toggling from the “Active Medications” view to the “Active & Inactive Medications” view. She sees ([Figure 2.9](#fig-2-9) below) that lisinopril had once been prescribed, but that the patient had only taken it for a few months. She wonders why. Doing a search of the chart, she finds a phone note reporting that the patient developed a persistent dry cough, which had resolved when he stopped taking lisinopril. There was no other record of that adverse effect in the chart, so Dr. Barnes added lisinopril to the allergy list, with “cough” as an “adverse effect.” If her EHR supports the function, she might also write “cough” in the comment field associated with lisinopril under the “reason for stopping” column.

Figure 2.9 **Show All Medications (Active & Inactive)** — Lisinopril had been stopped
—[Try it out!](http://inspiredehrs.org/timeline/)

![Show All Medications and see what had been stopped](../images/UM_EHR_0007_lisinopril-stopped.png)


现在Dr. Barnes医生考虑使用amlodipine来控制患者的血压，但想了解一下患者对目前正在服用的药物的依从性
对用药时间轴进行缩放，Dr. Barnes医生发现重新拿Coreg药已经晚了3个礼拜，但耻于承认。患者昨晚上才要求重新配药，打算今天门诊完了之后去药房拿药。
Coreg相对较高的共同承担费用导致患者不能按时重新配药。考虑到这个原因，医生们讨论一下在in the beta-blocker class中价格相对便宜的替代品
最终选择了每日200mg的metoprolol XL 。通过阅读[Chapter 3, Medication Reconciliation](./medication-reconciliation.php)你可以了解患者不愿服用处方中的药品的原因。

Dr. Barnes now considers prescribing amlodipine to control the patient’s high blood pressure, but wonders about the patient’s adherence to the medications he’s already on. Zooming in on the medication timeline, she finds that the patient was three weeks late refilling his Coreg, but had been embarrassed to admit to it. The patient had just requested a refill last night and planned to pick it up from the pharmacy after the visit today. Coreg’s relatively high co-pay made the patient hesitant to refill his prescription in a timely manner. With this brought to her attention, the physician discussed less expensive alternatives in the beta-blocker class. Together they selected metoprolol XL 200 mg daily. You can read more about why patients might not be taking their medication as prescribed in[Chapter 3, Medication Reconciliation](./medication-reconciliation.php).

Figure 2.10 **Zoom in to See Granular Details like Gaps in Medication Adherence**

![Zoom in to See Granular Details like Gaps in Medication Adherence](../images/UM_EHR_0008_zoom-in.png)

时间轴给出的是一个完整的概述。在最顶层，时间轴能够传递患者何时开始、停止服用某种药物的详细信息，药物剂量何时变更的信息、
药物剂量的变更是增加还是减少以及服用的剂量是不是最大剂量。

A timeline offers a complete overview. At the top level, a timeline conveys details about when a patient starts and stops taking a medication, when that medication's dose changes, whether that change is an increase or decrease, and whether the dosage taken is the maximum one.

在[Gallery 2.4](#gal-2-4)中给出的时间轴中，每个条都表示一种药物的用药史（比如起初citalopram的
剂量是10mg，慢慢的增加到40mg每日）。医生可以调整时间宽度得到更加详细或宽泛的患者用药史的视图。深黑色表
示的是某种药物的最大剂量，暗灰色表示相对较小的剂量。这种设计能够让用户一眼就获取大量信息。


In the straightforward timeline presented in[Gallery 2.4](#gal-2-4), each bar represents the history of a single medication (e.g. citalopram started at 10 mg, and the dosage progressively increased to 40 mg daily). The physician can adjust the timescale to give a wider or narrower view of the patient’s medication history. Solid black represents the maximum dose of that particular medication, with shades of gray representing progressively lower doses (lighter means lower). This design presents the user with a wealth of information at a glance.

好的EHR电子病历系统的设计能够适应大量的用药列表。患有复杂疾病的患者的现用药列表中可能会有15到20种药物。。
理想情况下处理此类案例的医生无需滚动视图即可查看患者的所有用药信息。

Highly usable EHR designs can accommodate large medication lists. Patients with an array of complex problems can have 15 to 20 medications on their active list, and ideally physicians dealing with challenging cases such as these won't have to scroll to view all of a patient's medications at once.

某种药物(比如西酞普兰citalopram)的所有类型都应该放在同一个时间轴中，即使它们是不同的规格(10mg,20mg
    或40mg)或者是出现在不同的时间点(比方说，四年前的为期八个月的疗程，过去十二个月的另一个疗程)

All instances of a medication (e.g. citalopram) will occur in the same timeline, even if they involve different tablet strengths (10 mg, 20 mg, or 40 mg) or occur at distinct points in time (say, an eight month course four years ago, and another course for the past twelve months).

Gallery 2.4 **Medication Timeline**

*   2.4 a **Medication Timeline Showing Drug Dosages for "Today"**

![Medication Timeline Showing Drug Dosages for Today](../images/UM_EHR_0000_Annotated-Timeline.png)

*   2.4 b **How to Read the Timeline**

![How to Read the Timeline](../images/UM_EHR_0010_notated.png)

*  2.4 c **Special Cases<span class="capt-desc">— PRN (as needed) medications and medications with no fixed maximum dose**

![PRN medications have no fixed maximum dose](../images/UM_EHR_0011_notated-2.png)

我们所说明的用药时间轴其中包含了一些基于认知科学的创新的界面可用性的特征。高效的“高级概述”在单个视图中展示了
患者完整的用药列表的时间轴。这个工具避免了医生在工作记忆中尝试并记住所有碎片化信息，或者是在多个视图间切换时为了记住细节而做笔记。
医生在查看此类可视化视图时会注意到[preattentive attributes](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#preattentive-attributes)如颜色、长度和[proximity](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#proximity),能够比纯文本或数字形式的数据更加容易的识别出这些不同的模式。

The medication timeline we illustrate incorporates some innovative interface usability features predicated on cognitive science. The efficient “high-level overview” shows the timeline for a patient’s complete list of medications in a single view. This tool will eliminate the need for the user to try and hold all these disparate pieces of information in her working memory, or to make written notes just to keep track of the details scattered across several EHR views. A physician looking at this visualization will pick up on[preattentive attributes](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#preattentive-attributes)such as color, length, and[proximity](http://inspiredehrs.org/designing-for-clinicians/human-factors.php#proximity), and will be able to discern patterns in these far more easily than she might see them in text or numerical data.

我们的医生也可以对感兴趣的区域进行缩放来了解更多的细节。EHR电子病历系统能够提供解释、剂量信息、甚至于
能拿到药房的重复拿药数据或患者自发填写依从性数据情况下的依从性信息。这些将进一步帮助医生确认自己的预感，形成新的问题。

Our physician will also be able to zoom in on areas of interest and explore them in more detail. The EHR can provide her with explanations, dose details, and even adherence information if pharmacy refill data or patient-reported adherence data is available. This will further assist our physician to confirm hunches and develop new questions to pursue.

EHR电子病历系统也能够展示曾经下达给患者的任意的episodic medications药物，如疼痛、恶心和哮喘发作的PRN药物。
在[Gallery 2.5](#gal-2-5)中，这些是使用白色的条来表示的。EHR电子病历系统通过额外的视觉提示来表示患者曾经使用过此类药物
。EHR电子病历系统可能使用点或正方形来表示药房配药的事件，使用很小的垂直#(hash)标记来表示患者自发填报的用药。

The EHR can also display any episodic medications a patient has been prescribed, such as PRN medications for pain, nausea, asthma exacerbations, etc. In[Gallery 2.5](#gal-2-5), these are represented by a white bar. The EHR will display that a patient has used these medications by means of additional visual cues. An EHR might indicate pharmacy dispense events with a square or dot, and patient reports of medication use with a small vertical hash mark.

EHR电子病历系统能够按需只显示现用药或已停止用药，或者两者都显示。这能够帮助回答医生在调查之时发现的一些问题(为什么去年12月份停用这种药物
    转而使用另外一种药物)。

EHR filtering can be capable of showing only active medications, discontinued medications, or both, as needed. This will help physicians answer other questions that arise during their inquiries (“Why was this medication stopped last December, and what made the patient switch to this alternative medication?”).

在时间轴中，我们使用单色来传达大多数信息。拥有特殊配色方案的EHR电子病历系统可以调整我们的配色方案，使用深蓝色或深绿色来
来表示最大数量。我们很少使用颜色来提醒医生诸如超过推荐最大剂量等要点。一般而言，采用单色是一种比较好的设计。
你可以保守的使用颜色，以不会干扰用户的方式来传达信息。要记住的是一些用户无法识别颜色。在我们的例子中，
由于无法识别颜色是很常见的残疾，在需要表示最大剂量的时候，我们同时使用了颜色和交叉阴影，
正是为了确保大家都能注意到这些重要的信息。用单色来打印你的设计来确保你所设计的最大剂量的获取以及理应传达的所有信息仍然是可见的。


For the timeline, we used monochrome (grayscale) to convey most information. EHRs with specific color schemes could adapt our black scheme for conveying a maximum number to a “darkest blue” or “darkest green”. We used color sparingly, to alert physicians to issues such as dosages over the recommended maximum dose. In general, it’s a good idea to design in monochrome first. You can then add color sparingly to convey meaning in a way that won’t distract the user. Remember that some users will not perceive color. In our example, we combined color and cross hatching when we needed to indicate a maximum dose to make sure that no one missed crucial information due to this quite common disability. You can make sure you’ve designed for maximum accessibility by printing your design in grayscale and checking that all the information it is supposed to convey is still visible.

首先，文字必须清晰易辨认。在我们的时间轴中，药品名称是左对齐的，这样更容易阅读。剂量要么是黑色要么是白色，与背景色都形成了
鲜明的对比。有经验的用户能够手动缩放时间轴至合适的程度，但即使是新手也能够使用按钮来缩放至常用的、恰当的时间区间(比如过去的三个月或过去的一年)。

Above all, the text must be legible. On our timeline, the drug names are left-justified, which makes them easier to read. The dose, displayed in either black or white, contrasts with the background. Experienced, dexterous users can comfortably manually zoom in on our timeline, but even absolute beginners can use the buttons that allow them to quickly zoom in on commonly-used, useful time periods (such as “the last three months” or “the last year”).

我们的时间轴旨在适应每一个潜在的用户：医生、护士、患者、护理人员、药房人员、精神卫生从业人员、健康保健的教练以及所有其他医疗从业人员。时间轴也能够适应较长的用药列表。
十多种药品是很常见的情况。20种药品也不稀奇。30种药品可能就比较少见了。用药的时间轴能够减轻视觉负担，
它是一个数据可视化的工具，它的妙处在于首先是概述，然后是缩放和过滤，然后是按需查看详细信息。

Our medication timeline aims to accommodate every conceivable user: physicians, nurses, patients, caregivers, pharmacists, mental health professionals, health coaches, and all other medical specialists. It can accommodate long lists of medications. A dozen medications can be quite common. Twenty medications would not be surprising. Thirty medications, sadly, may not be rare. The medication timeline handles the visual burden with ease. It’s a tool for data visualization, whose mantra is “overview first, then zoom and filter, then details-on-demand.” Let’s look at[Gallery 2.5](#gal-2-5) to demonstrate how.

Gallery 2.5 **Medication Timeline**

*   2.5 a **Instructions on How to Read the Timeline**

![Instructions on how to read the timeline](../images/UM_EHR_0001_tutorial.png)

*   2.5 b **Active Medications in the Timeline**

![Active Medications in the Timeline](../images/UM_EHR_0000_Annotated-Timeline.png)

*   2.5 c **Grab the Scrubber**— Drag it across the timeline to look at more details about certain dates
![Drag scrubber to look at more details about certain dates](../images/UM_EHR_0002_drag.png)

*   2.5 d **Dragging the Scrubber Further Back in Time**— Medications not yet prescribed appear as grayed out names, and the labels disappear.

![Drag Scrubber Back in time. Medications not yet prescribed grayed out names and labels disappear](../images/UM_EHR_0003_drag2.png)

*   2.5 e **Show All Medications**— Active medications are at the top, inactive medications are at the bottom.

![Active medications are at the top, inactive medications are at the bottom](../images/UM_EHR_0004_show-all.png)

*   2.5 f **Tap on a Medication Line to See More Details**
![Tap on a Medication Line to See More Details](../images/UM_EHR_0005_hover.png)

*   2.5 g **Expanding a Bar Reveals Details that Influenced a Patient’s History with a Medication**— Such as their reason for discontinuing it. Access other details (pharmacy, prescriber, etc) by linking a drug timeline to that drug in the interactive table.

![Click to expand a bar](../images/UM_EHR_0013_tap1.png)

*   2.5 h **Back to Where We Started**
![Active medications in the timeline](../images/UM_EHR_0000_Annotated-Timeline.png)

浏览下面的演示视频来了解时间轴的操作。

See the Timeline in action in this short demo video.

[Watch the Demo Video of the Timeline Prototype](http://vimeo.com/99496442)

#### Try It Out

我们已经制作了一个交互式的原型，你可以尝试一下。想象一些临床任务(下面我们给出了一些建议)
在使用的时候和你们现在使用的电子病历系统中的工具与这个原型进行一个比较，
体会一下我们所做的一些调整在用户体验上的差异。尝试对使用原型完成一项任务和朋友或同事
使用现有的电子病历系统完成同样任务进行计时。我们的原型是不是对你来说更加精确？


We’ve made an interactive prototype timeline you might like to try out. Imagine a few clinical tasks (we've listed some suggestions below) and, as you work through them, compare this prototype to the tools in your existing EHR and see the difference our changes make in your user experience. Try timing yourself doing a task on the prototype and a friend or colleague doing the same task in your current EHR. Is one tool more accurate for you?

要注意的是目前还仅仅是个原型，有很多不足的地方，后续的版本希望能够改进它(比如改进缩放功能，时间轴的标签，自定义颜色，
    能够获取更改原因的记录或者详细信息，过滤器高等)

Note that this is an early prototype with known limitations we hope to address in future versions of the book (e.g. improved zooming, better labels for the time axis, customizable use of color, access to notes and details about reason for changes, filters, etc.)

对于我们的原型，假设今天是2013年9月18日

For this prototype, assume "today" is September 18, 2013.

Interactive 2.3 Medication Timeline Prototype[Try it out!](http://inspiredehrs.org/timeline/)

![Try our medication timeline prototype](../images/UM_EHR_0000_Annotated-Timeline.png)

#### 尝试如下任务Try These Tasks

1.  操作直到你可以在时间轴底部看到起止日期2013年9月18号(我们把当前日期设定为2013年9月18号，这样就有一年的操作空间).
2.  患者最近开始服用的是什么药物？何时开始服用该种药物？
3.  患者最近停用的是哪种药物？
4.  拖动底部的scrubber直到看到5年期的时间轴
5.  患者原来停止服用，现在又开始服用的是哪种药物?
6.  试着朝左边拖动最右边的药物名称的列表。你会发现其中一些药品名称不见了。只有患者当下在服用的
药物和剂量才会出现在这个列表之中。

1.  Navigate so that you can see the starting date, September 18, 2013, by dragging the gray shaded area (the scrubber) in the bottom timeline. (We set a current date of September 18th so our prototype will work both now and for years to come).
2.  What medication did the patient start taking most recently? About when did he start taking it?
3.  Which medication did the patient stop taking most recently?
4.  Drag the scrubber at the bottom of the frame until you can see a 5-year timeline.
5.  Which drugs did the patient stop taking, and then start taking again?
6.  Try dragging the list of medication names on the right side of the frame towards the left. Notice that some names disappear. Only the drugs and the dosages the patient was taking at the point in time you’ve moved the scrubber to will show up on the list.

#### 用药时间轴未来的发展方向 Future Directions for Medication Timeline

我们的时间轴目前还不能解决所有的问题。我们还没有试着去解决复杂人物如化疗、儿科剂量中涉及到的数据需求。其他临床任务
实际上需要一个整合了其他临床数据的历史视图。比如，华法林抗凝管理(warfarin anticoagulation management)需要
之前华法林剂量变更、其他药物变更和凝血酶原时间(又称protime, or PT or INR) 实验室检查结果等的详细信息。
胰岛素管理要求医生能够同时查看最近的血糖结果、 血红蛋白A1c的结果、饮食和活动的信息，有时候还要有患者正常病情或活动的异常信息。。

Our timeline doesn’t yet provide all the answers. We haven’t attempted to address the data needs of complex regimens like chemotherapy, or the variables involved in pediatric dosing. Other clinical tasks really demand a historical view that integrates other clinical data. For example, warfarin anticoagulation management requires details about prior warfarin dose changes, other medication changes, and prothrombin time (also known as protime, or PT or INR) lab results. Insulin management requires physicians to be able to simultaneously view recent blood glucose results, hemoglobin A1c results, diet and activity details, and sometimes other details about exceptions to the patient’s usual condition or activities.

实验室检查结果的图表展示和时间轴一起可能能更多的帮助医生。诸如此类情况的理想时间轴能够让医生了解哪些药物发生变化，如果有的话
，发现肝损伤的实验室标记出现上升，或者抗血压药物如何影响电解质和肾功能。这种类型的展示方式能够通过一种使目前的模式和现象对用户更加透明的
方式来提升患者的安全和医疗质量


A graphical display of laboratory values to accompany the timeline may help physicians
 even more. An ideal timeline for cases such as these would allow physicians to see what medication changes, if any, preceded a rise in laboratory markers of liver injury, or how a blood pressure medication affected electrolytes and kidney function. This type of display could enhance patients’ safety and quality of care by presenting information in a way that makes currently obscure patterns and phenomena crystal clear for the user.

 >#### 不同用药列表的设计能够完成不同用户的任务

>#### Different Medication List Designs Address Different Users’ Tasks

>**针对开处方的医生**

>**For Prescribers**

><table class="sidebar-table" id="prescribers"><thead><tr><th>用户任务</th><th colspan="3">功能</th></tr><tr><th></th><th>简单列表</th><th>交互式表格</th><th> 用药时间轴</th></tr></thead><tbody><tr><td>**快速浏览列表**</td><td>●</td><td></td><td></td></tr><tr><td>**管理治疗决策**  
<span>(整体概述来辅助决策)</span></td><td>●</td><td>●</td><td></td></tr><tr><td>**重新拿药**  
<span>(何时拿药以及做出调整)</span></td><td></td><td>●</td><td></td></tr><tr><td>**完成用药核对**  
<span>(转诊转科时比较2个或多个列表)</span></td><td>●  
<span>参考后续章节</span></td><td></td><td></td></tr><tr><td>**回顾时间进程**</td><td></td><td></td><td>●</td></tr><tr><td>**管理临时性变化**     简要的进程(类固醇破裂或如化疗等间歇性治疗)<span> **手术相关的调整**
 (在手术期间需要的临时用药或用药调整)</span></td><td></td><td>●  
<span>"期望的停药日期"来排序</span></td><td></td></tr><tr><td>**回忆尝试过的&失败了的用药过程**  
<span>(哪些药有效、哪些没用，原因是什么?)</span></td><td></td><td></td><td>●  
<span>但前提是信息是由用户所记录的</span></td></tr><tr><td>**依从性评估**  <span>
(是否及时再次拿药? 服用的剂量是否和计划的一样?)</span></td><td></td><td></td><td>●  
<span>取决于诸如配药数据或患者上报等其他数据</span></td></tr></tbody></table>
>#### For Patients

><table class="sidebar-table" id="patients"><thead><tr><th>用户的任务</th><th colspan="2">功能</th></tr><tr><th></th><th>简单列表</th><th>交互式表格</th></tr></thead><tbody><tr><td>**浏览或记住列表**</td><td>●</td><td></td></tr><tr><td>**与他人分享列表**</td><td>●</td><td></td></tr><tr><td>**Restock the [pill organizer](http://en.wikipedia.org/wiki/Pill_organizer)**  
<span>(展示pill应该放在小小的每周的药盒的哪些地方)</span></td><td></td><td>●  
<span>几乎没有</span></td></tr><tr><td>**记住日常的剂量**  
<span>(提醒用户日常用药和不常用药的剂量。让用户在服药时核对那些不在列表中的药品)</span></td><td>●</td><td>●</td></tr><tr><td>**记住药房的重新配药**  
<span>(帮助用户协调去药房拿药以及请医生重新续药)</span></td><td></td><td>●  
<span>可能需要来自药房的数据或来自药瓶的数据</span></td></tr><tr><td>**在门诊之后更新列表**  
<span>(考虑在某次就诊之后对用药列表所做的所有变化生成一个最终版的列表)</span></td><td></td><td>●</td></tr></tbody></table>


* * *

### 2.4 总结Summary

1.  在设计EHR电子病历系统时，要考虑用户和他们要完成的一些任务。这些内容能够帮助
你决定在使用某种特殊的用药列表视图时，医生需要哪些功能和详细信息.
2.  使用[preattentive attributes](./human-factors.php#preattentive-attributes)<span class="print-only"> (参考 Preattentive Attribute in the Human Factors chapter)</span> (诸如颜色、大小、形状和对齐)来吸引用户的注意力到
突出的细节。
3.  首先使用单色来设计，然后谨慎地和有意义地添加颜色，也就是那些能够添加信息而不分散用户注意力的地方。
4.  要牢记人们的[工作记忆](./human-factors.php#working-memory)<span class="print-only"> (See Working Memory in the Human Factors chapter)</span>, 特别是像用药和剂量等复杂项或混合物。尽可能将信息直接置于视图之中。
杜绝医生需要在一系列的工作流程中记住某个步骤中的详细信息.
5.  通过给用户所有关键信息的概述来提升用户的态势感知
6.  减少用户的[认知负载](./human-factors.php#cognitive-load)<span class="print-only"> (See Cognitive Load in the Human Factors chapter)</span>. 替用户做脏活累活。设计时要力求最小化重复阅读。直接地展示信息而不是要求用户记忆信息
7.  牢记数据可视化的奇妙之处：首先是概览，然后是缩放和过滤，最后是按需展示详细信息
8.  设计要能够适应超大用药列表.要牢记在现用药列表中存在15-20种药品是很常见的。
尝试设计无需滚动视图即可查看患者的所有用药信息的列表.


译者注：
1、Exam Room  诊疗室 检查室 根据语境来看            这里就是医生自己的办公室  诊疗室。
2、situational awareness  态势感知              参考http://news.xinhuanet.com/mil/2011-12/09/c_122402518.htm
3、medication reminder boxes
4、dashboard overview 病历概要
5、mental effort 认知负荷
6、de-emphasizing
7、Dosage instructions 用法用量
8、preattentive attributes 前注意属性
9、workhorse 标配
10、medication renewal
11、co-pay——
比如保险中规定医疗费用达到1000以上，多出的部分保险公司才报销，1000以下自理，这个1000就是deductible
比如总共花了3000，那多出的2000，根据不同的医疗服务项目，有的是受保人要固定支出的共同费用（比如10元，100元），这种固定的共同费用就是Copay/Copayment
有的是受保人按照一定比率自己支付的费用（比如10%，20%），这种按照比率收取的费用就是Coinsurance。是不是这样？
12、prescription renewal
13、in the beta-blocker class
14、cross hatching 交叉阴影
15、Renew medications 重新拿药
16、 data visualization mantra
有的是受保人按照一定比率自己支付的费用（比如10%，20%），这种按照比率收取的费用就是Coinsurance。是不是这样？
12、prescription renewal
13、in the beta-blocker class
14、cross hatching 交叉阴影
15、Renew medications 重新拿药
16、 data visualization mantra
