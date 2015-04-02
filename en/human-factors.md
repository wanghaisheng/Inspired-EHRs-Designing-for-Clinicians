## 7

## Human Factors Principles

<div class="subheader">

Systems that complement how we see, read, think and decide can improve our performance.

</div></div></div></div><section id="human-factors-engineering" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### What is Human Factors Engineering?

</div>

Human Factors Engineering seeks to improve human performance by designing systems that are compatible with our perceptual, cognitive, and physical abilities. Imagine an EHR that requires a physician to cancel a prescribing task, then navigate through several screens, remember a value, and navigate back to complete the prescription. This EHR taxes the well-known limits of human memory. Over-taxing users’ memory causes them to make errors, especially if they’re interrupted while using the system – a common occurrence in healthcare.

In contrast, an EHR that allows a physician to see at a glance how well a patient is controlling his diabetes and hypertension gives the physician the situational awareness (and time) he needs to begin to address his patient’s current concerns. The physician can focus attention on understanding the story of the human sitting across the room, instead of on remembering and finding the necessary information to make decisions.

The Fundamental Theorem of Biomedical Informatics states “that a person working in partnership with an information resource is ‘better’ than that same person unassisted.” Human Factors Engineering involves building this partnership, designing hardware and software that make it as easy as possible for users to do tasks safely and efficiently. An EHR based on sound human factors engineering principles can help clinicians focus on the difficult task of caring for patients, rather than on figuring out how to use or work around the EHR. We must understand the ways people see, read, think and decide so that we can use this information to build systems that enhance people's job performance.

</div></div></section><section id="how-people-perceive" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 7.1 How People Perceive

</div>
#### 7.1.1 Our Eyes Have Expectations

**Our eyes are drawn to familiar patterns. Sometimes we even see patterns we know and expect instead of what's actually there.**

Your eyes take in data, but your brain 'perceives' this data and parses it into meaningful visual information. Our brains create shortcuts to help us make sense of the estimated 40 million sensory inputs they receive per second. They use our expectations, past experiences, associations, and learned rules of thumb to make guesses about what it is we're looking at. Everyone has seen something at a glance and thought it was a certain object, and then focused on it and realized it was actually something else.

<div class="example" id="fig-7-1"><div class="ex-title"><span class="ex-type">Figure 7.1</span><span class="ex-caption">Read the Following Words:<span class="capt-desc">Tae Cat looks like The Cat when the tops of the A's are cut off</span></span></div>[![Tae Cat looks like The Cat when the tops are cut off](./assets/images/examples/human-factors/thecat.png)](./assets/images/examples/human-factors/thecat.png "Figure 7.1 - Read the Following Words - Tae Cat looks like The Cat when the tops of the A's are cut off")</div>

Most people read the following as “The cat,” even though the middle letter in each word is exactly the same, and neither is a perfect H or A. Our perceptual system uses context (the letters around the middle letter) and expectations (predicated on our familiarity with common English words) to allow us to cope with and make sense of imperfect, noisy input. But the same properties that make our perceptual system robust can also lead us astray. For instance, can you name the first drug on this prescription ([Figure 7.2](#fig-7-2))?

<div class="example" id="fig-7-2"><div class="ex-title"><span class="ex-type">Figure 7.2</span><span class="ex-caption">Handwritten Prescription<span class="capt-desc">— Name the first drug on the list<span class="smaller">(from[Western Journal of Medicine](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1070756/)).</span></span></span></div>[![Handwritten Prescription](./assets/images/examples/human-factors/handwritten-prescription.png)](./assets/images/examples/human-factors/handwritten-prescription.png "Figure 7.2 - Handwritten Prescription - Name the first drug on the list")</div>

The cardiologist who prescribed the medication wrote 'Isordil,' but the pharmacist read it as 'Plendil.' After taking the prescribed medication for two days, the patient had a heart attack. Several days after that, he died<sup>1</sup>. In this case, the pharmacist was led astray by the very same perceptual system that enabled him to do his job correctly most of the time. Our perceptual system makes assumptions so automatically that we often don’t even realize that it is doing so.

Users come to computers with expectations (mental models) based on what they have seen before, and with a built-in tendency to make assumptions about what it is they're seeing. When we scan a screen, we look for digestible chunks: familiar things like navigation bars, buttons and logos. We also tend to look at the center of the screen rather than at the edges, because we expect the edges to display less important things, like logos and tools not relevant to the task at hand. We expect the core components of an interface to be front and center, easy to find.

<div class="example" id="fig-7-3"><div class="ex-title"><span class="ex-type">Figure 7.3</span><span class="ex-caption">An Unclear Layout<span class="capt-desc">— Adding allergies without good workflow guidance from the interface.</span></span></div>[![An Unclear Layout](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png)](./assets/images/examples/allergy-list/Um_Ehr_AllergyList_0004_cough-search.png "Figure 7.3 - An Unclear Layout - Adding allergies without good workflow guidance from the interface")</div><div class="example" id="fig-7-4"><div class="ex-title"><span class="ex-type">Figure 7.4</span><span class="ex-caption">Meeting Our Expectations<span class="capt-desc">— We're still adding an allergy, but now the format is more familiar, and lists the tasks users need to complete in a sequential order.</span></span></div>[![Meet Expectations with a more familiar format](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy_2.png)](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy_2.png "Figure 7.4 - Meeting Our Expectations - We're still adding an allergy, but now the format is more familiar, and lists the tasks users need to complete in a sequential order.")</div><div class="example" id="fig-7-5"><div class="ex-title"><span class="ex-type">Figure 7.5</span><span class="ex-caption">A Few Common Affordances<span class="capt-desc">— 1) These three words look like buttons, so users understand that if they click one, that will do something. 2) Users understand that the small icon of a calendar will expand into a full calendar menu if they click it.</span></span></div>[![Affordances including clear selections and icons](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy.png)](./assets/images/examples/allergy-list/Um_Ehr_0006_add-an-allergy.png "Figure 7.5 - A Few Common Affordances - 1) These three words look like buttons, so users understand that if they click one, that will do something. 2) Users understand that the small icon of a calendar will expand into a full calendar menu if they click it.")</div><div class="example" id="fig-7-6"><div class="ex-title"><span class="ex-type">Figure 7.6</span><span class="ex-caption">Disclosure Arrow Affordance<span class="capt-desc">— In this image, the arrow affordance lets users know that they can expand or collapse the entry to access more information.</span></span></div>[![Arrow affordance shows that entries can expand or collapse for more information](./assets/images/examples/human-factors/Um_Ehr_0010_collapse-affordance.png)](./assets/images/examples/human-factors/Um_Ehr_0010_collapse-affordance.png "Figure 7.6 - Disclosure Arrow Affordance - In this image, the arrow affordance lets users know that they can expand or collapse the entry to access more information")</div><div class="example" id="fig-7-7"><div class="ex-title"><span class="ex-type">Figure 7.7</span><span class="ex-caption">Sort Arrow Affordance<span class="capt-desc">— Here, the arrow indicates the ability to sort the list by different columns.</span></span></div>[![Arrow indicates the list can be sorted by different columns](./assets/images/examples/human-factors/Um_Ehr_0011_sort-affordance.png)](./assets/images/examples/human-factors/Um_Ehr_0011_sort-affordance.png "Figure 7.7 - Sort Arrow Affordance - Here, the arrow indicates the ability to sort the list by different columns.")</div>

Affordances tell users at a glance that particular elements of the graphical user interface are functional devices. Well-designed affordances also give users an idea of what will happen when they use them.

#### 7.1.2 We See in Gestalts

**People perceive whole shapes, or gestalts, rather than disconnected forms.**

Gestalt is a German word for form or shape. In English, it has come to have connotations of ‘wholeness.’ When you walk into a room, you immediately form an overall sense of what's going on therein and its corresponding emotional tone. Most people understand when they've come in and interrupted a fight, even if they heard none of the previous conversation. When you view a webpage for the first time, you get a similar overall impression of it. You can say pretty quickly whether you think the site looks cluttered or appealing, modern or out of date. Several design elements feed into our gestalt impressions of sites and applications.

#### Proximity

The distance between objects determines what we perceive the relationships between those objects to be. If things are close together, we assume that's significant and 'group' them in our minds. If elements in a designed object are grouped together, we assume this was intentional and is meaningful.

</div><div class="one-half column"><div class="example" id="fig-7-8"><div class="ex-title"><span class="ex-type">Figure 7.8</span><span class="ex-caption">Proximity<span class="capt-desc">— Our eyes notice the distribution of these dots...</span></span></div>[![Dots in a group with one separate](./assets/images/examples/human-factors/UM_EHR_0001_spatial-grouping.png)](./assets/images/examples/human-factors/UM_EHR_0001_spatial-grouping.png "Figure 7.8 - Our eyes notice the distribution of these dots...")</div></div><div class="one-half column"><div class="example" id="fig-7-9"><div class="ex-title"><span class="ex-type">Figure 7.9</span><span class="ex-caption"><span class="capt-desc">... and our brains group the closer objects automatically.</span></span></div>[![Clear isolation of separate dot](./assets/images/examples/human-factors/UM_EHR_0002_spatial-grouping-2.png)](./assets/images/examples/human-factors/UM_EHR_0002_spatial-grouping-2.png "Figure 7.9 - ... and our brains group the closer objects automatically")</div></div><div class="sixteen columns">

**Example:** The medication reconciliation view below ([Figure 7.10](#fig-7-10)) breaks medications into groups. It then places these groups in the same columns. Users can tell there are different groups (columns) at a glance, without having to focus on, read, and understand all the information on the chart.

<div class="example" id="fig-7-10"><div class="ex-title"><span class="ex-type">Figure 7.10</span><span class="ex-caption">Ambulatory Medication Reconciliation Workflow<span class="capt-desc">— Items in the center are most alike, and those at the sides are most different. Items in between need clarification.</span></span></div>[![Figure 7.10 - Ambulatory Medication Reconciliation Workflow - Items in the center are most alike, and those at the sides are most different. Items in between need clarification.](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png)](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png "Figure 7.10 - Ambulatory Medication Reconciliation Workflow - Items in the center are most alike, and those at the sides are most different. Items in between need clarification.")</div>
#### Closure

Our brains fill in visual blanks for us and draw conclusions with less than complete information. This helps us make sense of the world quickly. Sometimes we can draw the wrong conclusions, misleading our users. We need to keep the advantages and shortcomings of this perceptual habit in mind when we design systems. Designers can make use of our brains' tendency to fill in the blanks to help users to quickly understand a whole idea based on a partial picture, but design can also accidentally lead users to unintended and unhelpful 'false' gestalt impressions.

**Example:** Our minds take lines or curves and build objects out of them. This is how we can know we're looking at something that's supposed to represent a person when it's a stick figure. Even though the lines below don't add up into a circle and a rectangle, people can still see and identify both shapes.

<div class="example" id="fig-7-11"><div class="ex-title"><span class="ex-type">Figure 7.11</span><span class="ex-caption">Closure</span></div>[![Partially drawn shapes](./assets/images/examples/human-factors/UM_EHR_0003_closure.png)](./assets/images/examples/human-factors/UM_EHR_0003_closure.png "Figure 7.11 - Closure")</div>
#### Similarity

We perceive visual elements that look**similar** as parts of a group. Designers can indicate that two objects are similar, and thus related, by giving the objects the same sizes, shapes or colors. Interfaces that visually group related items are easier to use than those that don't. As a general rule, items that users must process together could be grouped together, while items that need to be processed separately are not.

<div class="example" id="fig-7-12"><div class="ex-title"><span class="ex-type">Figure 7.12</span><span class="ex-caption">Users Perceive That the Blue Dots Are Associated</span></div>[![Blue dots with several dark red dots interspersed](./assets/images/examples/human-factors/UM_EHR_0004_similarity.png)](./assets/images/examples/human-factors/UM_EHR_0004_similarity.png "Figure 7.12 - Users Perceive That the Blue Dots Are Associated")</div>

**Example**: In the medication reconciliation interface we looked at earlier,**proximity** marked certain groups of items as categories (columns). Now, when we add color, we create new groups ([Figure 7.13](#fig-7-13)). Medications the user approves turn green, and medications the user deselects fade to light gray.

<div class="example" id="fig-7-13"><div class="ex-title"><span class="ex-type">Figure 7.13</span><span class="ex-caption">Color Creates New Groups</span></div>[![Color creates new groups](./assets/images/examples/human-factors/UM_EHR_0009_the-final-selection-clean.png)](./assets/images/examples/human-factors/UM_EHR_0009_the-final-selection-clean.png "Figure 7.13 - Color Creates New Groups")</div>
#### Symmetry

Our minds like to make sense of complex visual fields by assigning them a perceived center and attendant**symmetry**.

**Example**:[Figure 7.14](#fig-7-14) shows us how our minds like to see two symmetrical diamonds rather than other, equally possible (but less pleasingly symmetrical) shapes.

<div class="example" id="fig-7-14"><div class="ex-title"><span class="ex-type">Figure 7.14</span><span class="ex-caption">Symmetry<span class="capt-desc">— Our brains try to resolve complex visual fields into combinations of simple, symmetrical shapes.</span></span></div>[![Symmetrical shapes colored in different ways](./assets/images/examples/human-factors/UM_EHR_0005_symmetry.png)](./assets/images/examples/human-factors/UM_EHR_0005_symmetry.png "Figure 7.14 - Symmetry - Our brains try to resolve complex visual fields into combinations of simple, symmetrical shapes.")</div>

**Example**: When we first glance at[Figure 7.15](#fig-7-15), below, we see two columns. In fact, a series of individual entries creates the illusion of columns.

<div class="example" id="fig-7-15"><div class="ex-title"><span class="ex-type">Figure 7.15</span><span class="ex-caption">Symmetry in Medication Reconciliation</span></div>[![Two lists side by side for medication reconciliation](./assets/images/examples/human-factors/UM_EHR_0005_two-lists-side-by-side-before-matching-clean.png)](./assets/images/examples/human-factors/UM_EHR_0005_two-lists-side-by-side-before-matching-clean.png "Figure 7.15 - Symmetry in Medication Reconciliation")</div>
#### Figure / Ground

Our brains perceive objects either as figures in the foreground or as part of the background. Whatever we're focusing on becomes the figure, and everything else shifts into the background accordingly.

**Example**: In[Figure 7.16](#fig-7-16) below, the ampersand is the figure, distinct from the blue rectangle that serves as its ground or background. As the designer intended, users understand the figure to be more important than the ground.

<div class="example" id="fig-7-16"><div class="ex-title"><span class="ex-type">Figure 7.16</span><span class="ex-caption">Figure / Ground</span></div>[![two faces or a vase](./assets/images/examples/human-factors/UM_EHR_0006_figure-ground.png)](./assets/images/examples/human-factors/UM_EHR_0006_figure-ground.png "Figure 7.16 - Figure / Ground")</div>

**Example**:[Figure 7.17](#fig-7-17) below is the classic Edgar Rubin image in which viewers see either two faces or a vase, depending on where they focus their attention. Rubin was a practitioner of gestalt psychology.

<div class="example" id="fig-7-17"><div class="ex-title"><span class="ex-type">Figure 7.17</span><span class="ex-caption">Ambiguous Figure/Ground Relationship</span></div>[![Ambiguous Figure/Ground Relationship](./assets/images/examples/human-factors/UM_EHR_0007_figure-ground-2.png)](./assets/images/examples/human-factors/UM_EHR_0007_figure-ground-2.png "Figure 7.17 - Ambiguous Figure/Ground Relationship")</div>
#### Continuity

In day to day life, our perception combines and relies on all of these components. Alignment creates groupings of items, and these groupings are said to have**continuity**. Our brains expect and try to reconcile contours into continuous objects.

<div class="example" id="gal-7-1"><div class="ex-title"><span class="ex-type">Gallery 7.1</span><span class="ex-caption">The Continuity Principle</span></div><div id="cbp-fwslider" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">7.1 a</span><span class="capt-desc">Though a rectangle 'blocks' parts of this curve...</span></div>[![A curve with portions cut off](./assets/images/examples/human-factors/UM_EHR_0008_continuity-1.png)](./assets/images/examples/human-factors/UM_EHR_0008_continuity-1.png "Gallery 7.1 a - Though a rectangle 'blocks' parts of this curve...")</div>
*   <div><div class="caption"><span class="ex-type">7.1 b</span><span class="capt-desc">...humans perceive both the curve and the box as whole, uninterrupted entities...</span></div>[![The cut off portions are actually the outline of a rectangle](./assets/images/examples/human-factors/UM_EHR_0008_continuity-2.png)](./assets/images/examples/human-factors/UM_EHR_0008_continuity-2.png "Gallery 7.1 b - ...humans perceive both the curve and the box as whole, uninterrupted entities...")</div>
*   <div><div class="caption"><span class="ex-type">7.1 c</span><span class="capt-desc">...rather than as a box and some line segments.</span></div>[![Rectangle and line separate and whole](./assets/images/examples/human-factors/UM_EHR_0008_continuity-3.png)](./assets/images/examples/human-factors/UM_EHR_0008_continuity-3.png "Gallery 7.1 c - ...rather than as a box and some line segments.")</div>

</div></div>

**Example**:[Figure 7.18](#fig-7-18) demonstrates several of the things we've been talking about. When we look at it, our brains detect the proximity of different medication lists and categories and the similarity of 'selected' and 'deselected' groups of medications. The list also takes advantage of the contrast we perceive between figure and ground. The dark text seems closer to us, and the faded text seems further away.

<div class="example" id="fig-7-18"><div class="ex-title"><span class="ex-type">Figure 7.18</span><span class="ex-caption">Continuity in Medication Reconciliation</span></div>[![Continuity in Medication Reconciliation](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png)](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png "Figure 7.18 - Continuity in Medication Reconciliation")</div>
#### 7.1.3 I Can't See It but I Use It

**We use our peripheral vision to get a big picture of what we're seeing, and we use that big picture to help us decide what to focus on.**

Our visual system consists of our eyes and the brain processes that work with them. This system does an amazing job of seeking out and providing us with visual information. It does so mostly without our being consciously aware of it. We are barely aware that only the very central part of our vision provides us with a sharp-focused image, detail rich, with color information. The periphery of our vision (outside of the central “peephole”) is fuzzy, and drained of color. That peripheral part of the vision is, however, able to detect features such as motion, edge, and contrast. These features guide our brains in making their "visual query" of the views before us.

Rapid eye movement enables our brains to sample the environment. The task we're trying to accomplish determines the details we unconsciously seek out. If we're looking for a friend, we notice faces in the crowd. If we're trying to find our way through the crowd, we notice the gaps between people.

Animated ads are effective (and annoying) because our peripheral vision detects motion. We want to ignore the ads, but their design takes advantage of the way vision works. Our eyes are drawn to anything that stands out. Our brains are trying to recognize threats in our environment, and our peripheral vision is always alert to differences and changes.

**Example**: When we look at[Figure 7.19](#fig-7-19), below, our eyes first do a quick visual query. They seek out major landscape elements and the details that will help us accomplish whatever we're using this display to do. What we notice in the scene below will vary depending on whether we're driving, deciding if we need to mow the lawn, or assessing if the weather will be suitable for a picnic this afternoon.

<div class="example" id="fig-7-19"><div class="ex-title"><span class="ex-type">Figure 7.19</span><span class="ex-caption">Visual Queries in the Real World</span></div>[![Visual Queries in the Real World](./assets/images/examples/human-factors/visualqueries3.png)](./assets/images/examples/human-factors/visualqueries3.png "Figure 7.19 - Visual Queries in the Real World")</div>

**Example**: When we look at a display like Gallery 7.2 below, we think we see something like the first image. Actually, what we really see at any given instant is something more like the second image. We only focus on a small area at any given moment. Our visual brain first latches onto a preattentive attribute like the red text, and is disproportionately drawn to that element. Then our eyes automatically scan to find the next point of visual interest.

<div class="example" id="gal-7-2"><div class="ex-title"><span class="ex-type">Gallery 7.2</span><span class="ex-caption">Visual Queries in EHRs</span></div><div id="cbp-fwslider-2" class="scale-with-grid cbp-fwslider">
*   <div><div class="caption"><span class="ex-type">7.2 a</span> We Think We See This</div>[![A visually busy interface](./assets/images/examples/human-factors/UM_EHR_0000_we-think-we-see-this.png)](./assets/images/examples/human-factors/UM_EHR_0000_we-think-we-see-this.png "Gallery 7.2 a - We Think We See This")</div>
*   <div><div class="caption"><span class="ex-type">7.2 b</span> ...But We Actually See This</div>[![Blurry interface with a red text clear](./assets/images/examples/human-factors/UM_EHR_0001_but-we-dont-we-see-this.png)](./assets/images/examples/human-factors/UM_EHR_0001_but-we-dont-we-see-this.png "Gallery 7.2 b - ...But We Actually See This")</div>

</div></div>

A peripheral glance tells people where they are and what to expect, helping us decide what to focus on. We can only truly see what we focus on. The display can only effectively convey that information at any given time.

**Design tip:** Feedback and error messages can pop up near an area people will already be focusing on. While we do use our peripheral vision to orient ourselves and scan for things, we also tend to ignore our peripheral vision when we're trying to focus on the task at hand.

#### 7.1.4 Preattentive Attributes

**Little, visual things people notice and understand quickly**

We notice some visual features, such as color, size, shape, orientation, and motion, more quickly than others. We call the things that especially stand out to us**preattentive attributes**. Before we fully process visual information, our minds prompt us to focus on these attributes. Things that stand out from the rest of their environment, as in[Figure 7.20](#fig-7-20) below, do so because of their attention-catching preattentive attributes.

<div class="example" id="fig-7-20"><div class="ex-title"><span class="ex-type">Figure 7.20</span><span class="ex-caption"><span class="capt-desc">How can we use preattentive attributes to facilitate data presentation?</span></span></div>[![preattentive attributes](./assets/images/examples/human-factors/UM_EHR_0009_attributes.png)](./assets/images/examples/human-factors/UM_EHR_0009_attributes.png "How can we use preattentive attributes to facilitate data presentation?")</div></div></div></section><section id="how-people-think" class="section"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 7.2 How People Think

</div>
#### 7.2.1 The Two Ways People Think

**Everyone has two modes of thinking. There's a rapid mode that requires little conscious effort and a slower mode that requires focus.**

If a system is easy to understand and work with, users don't have to engage with it via their 'slow, focused' mode of thinking. They can just use their rapid mode and save their mental energy for more important matters. Daniel Kahneman wrote a great book about these modes, and our thinking builds on his work.

The rapid mode of thinking is automatic and almost effortless. People often don't experience a sense of voluntary control over it. This mode allows us to:

*   See that something is larger than something else
*   Answer simple computations, like 2+2 = 4
*   Read words on a billboard
*   Understand simple sentences
*   Make rapid and simple associations, such as stereotypes (positive or negative)
*   Notice preattentive attributes

Our focused mode of thinking is effortful and allows us to perform more complex mental activities. We associate this mode of thinking with our experiences of agency, choice, and concentration: in short, with our 'consciousness.' This mode allows us to:

*   Focus on listening to one voice in a noisy room
*   Recall information, like addresses and phone numbers
*   Evaluate the validity of a complex argument
*   Scan for a particular piece of information in a long article

When creating an application, ask yourself whether you have any opportunities to convert tasks that require focused thinking into tasks that only require rapid thinking. Making the application perform complex calculations, sort information, and concisely present key details can free people up to do the focused thinking that only humans can.

The Twinlist medication reconciliation prototype,[Figure 7.21](#fig-7-21), makes the focused task of scanning two lists and finding similar drugs into a rapid one. The prototype identifies similar drugs and sorts them onto the same row. Twinlist also makes it easy for users to see the differences between similar drugs by highlighting these differences in yellow. A slow, visually and cognitively demanding search task involving two separate lists becomes a matter of brisk perception with Twinlist.

<div class="example" id="fig-7-21"><div class="ex-title"><span class="ex-type">Figure 7.21</span><span class="ex-caption">The Twinlist Prototype Facilitates Fast Thinking</span></div>[![The Twinlist Prototype Facilitates Fast Thinking](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png)](./assets/images/examples/human-factors/UM_EHR_0008_the-drug-becomes-bright-green-when-selected-clean.png "Figure 7.21 - The Twinlist Prototype Facilitates Fast Thinking")</div>
#### 7.2.2 Working Memory

**Working memory demands effort and is limited. Try to design systems that place limited demands on users' working memory.**

Working memory, or short-term memory, holds items like phone numbers until we can write them down or punch them into our phones. This type of memory stores information for less than a minute and demands focused thinking.

**Design tip**: Try not to ask people to look at information on one screen, remember it, and then enter it into another field on another screen.

If you ask people to use their working memories, make sure that what you're asking them to remember is uncomplicated. Don't distract them with additional demands, information and options while they're focusing on remembering a given bit of information. A system that interrupts people while they're trying to use their working memories causes them to forget what they're doing and wastes time.

People only keep three to four compound or complex items in their working memories at a time. The way interfaces display bits of information can influence users' working memory, however. If a design groups items together or breaks information down into manageable chunks, people can remember that information better. A phone number, for example, is easier to remember if it's been broken into chunks. Compare these numeric strings:

<div id="numeric-strings">

<span class="grey">Difficult:</span><span class="phoneno">9121889874</span>

<span class="grey">Easier:</span><span class="phoneno">912-188-9874</span>

<span class="grey">Easiest:</span><span class="phoneno">(912) 188-9874</span>

</div>

The first phone number is difficult to even just dial. If the interface asks users to enter phone numbers, it can allow them to enter these with or without the intervening hyphens or parentheses. It could display them, however, in the easy-to-read format. When the interface needs to display an unmanageable amount of information, and the design has done all it can to alleviate this, the interface can then 'chunk' its information in the manner of the phone number example.

#### 7.2.3 Cognitive Load

**Loads are heavy, even mental ones. Help lighten the user’s load.**

Our brains manage motor, visual and cognitive loads. The strain of managing and manipulating items within our working memory generates cognitive load. Motor load is the easiest for the brain to manage, while cognitive load is the most difficult.

Designers seeking to lighten users' cognitive loads need to bear these details in mind:

*   Focused thinking causes greater cognitive strain than rapid thinking. People can give a task about ten minutes of focused attention, but then they'll need a short break, unless they're particularly interested in the task or are in a flow state.
*   People can’t truly multi-task. We can only attend to one task at a time. When we think we’re multitasking, we’re actually rapidly switching tasks, start-stop-start-stop-start-stop. This can tire us out and cause us to make mistakes.
*   Recognizing is easy, remembering is difficult. We can recognize complex things like a map of Europe instantly, but most of us would likely have a hard time drawing such a map ourselves. Likewise, we find it easier to recognize patients' names than to recall them.
*   Problem-solving and calculating are hard, while learning from experience and performing learned actions is easy.

**Example**:[Figure 7.22](#fig-7-22) below demonstrates the mental work a doctor does when she reviews a medication list to try to understand what medications a patient is taking to control his blood pressure. She must read the list, recognize drugs' names, remember whether given drugs are prescribed for hypertension, recall from memory what the maximum doses for these medications are, and then check whether the patient has reached the maximum dosages for these medications. That's a lot of mental effort!

<div class="example" id="fig-7-22"><div class="ex-title"><span class="ex-type">Figure 7.22</span><span class="ex-caption">Scanning for Hypertension Medications</span></div>[![Scanning for Hypertension Medications](./assets/images/examples/medication-list/UM_EHR_0006_mental-work.png)](./assets/images/examples/medication-list/UM_EHR_0006_mental-work.png "Figure 7.22 - Scanning for Hypertension Medications")</div>

[Figure 7.23](#fig-7-23), below, sorts the list of drugs alphabetically by diagnosis. This allows our physician to access the same information, but costs her far less mental effort. Lightening the effort she has to expend on this task increases the amount of effort she can spend on other more important tasks.

<div class="example" id="fig-7-23"><div class="ex-title"><span class="ex-type">Figure 7.23</span><span class="ex-caption">Sort by Diagnosis<span class="capt-desc">— Makes it easier to search for hypertension medications</span></span></div>[![Sort by Diagnosis](./assets/images/examples/human-factors/UM_EHR_0010_sort-condition-mental-effort.png)](./assets/images/examples/human-factors/UM_EHR_0010_sort-condition-mental-effort.png "Figure 7.23 - Sort by Diagnosis - Makes it easier to search for hypertension medications")</div>

If the interface can indicate whether a medication has reached the maximum dose, this will save the doctor the effort of making a series of annoying calculations.

**Example**: Auto-complete functions can also lighten users' cognitive loads. Users typing in the name of a drug in a window with a predictive text function can employ low-impact recognition mental processes rather than more difficult recollection processes. If users employ rapid thinking at this stage of the proceedings, however, there's a danger that they might mistake similarly-named drugs. Employ tallman lettering to alert users to be aware that a similar-looking drug exists.

<div class="example" id="fig-7-24"><div class="ex-title"><span class="ex-type">Figure 7.24</span><span class="ex-caption">Recognizing Rather than Recalling<span class="capt-desc">— Drug searches that utilize auto-complete functions</span></span></div>[![Drug searches that utilize auto-complete functions](./assets/images/examples/medication-list/UM_EHR_0010_autocomplete.png)](./assets/images/examples/medication-list/UM_EHR_0010_autocomplete.png "Figure 7.24 - Recognizing Rather than Recalling - Drug searches that utilize auto-complete functions")</div>
#### 7.2.4 Everybody Likes a Chunk

**Breaking information down into small, digestible chunks helps people make sense of it.**

Human brains can only apply focused thought to a relatively small amount of information at a time. Interfaces must break information into chunks. They can give users information in manageable, controlled courses, like a formal dinner.

**Progressive disclosure** gives people the information they need when they need it. The interface gradually provides users with more and more detail. Designers need to develop a good knowledge of how their users will be working to understand what information they could begin with, and then what details can be introduced at successive stages. Keep in mind that people can only hold three to four things in their mind at once.

**Example:** The list in Figure 7.25 shows essential allergy information in four columns. The user has all the information she needs about the patient's medication allergies to make prescription decisions. If she needs additional information about the patient's allergies, she can select an entry to see more details.

<div class="example" id="fig-7-25"><div class="ex-title"><span class="ex-type">Figure 7.25</span><span class="ex-caption">Progressive Disclosure in an Allergy List</span></div>[![Progressive Disclosure in an Allergy List](./assets/images/examples/allergy-list/Um_Ehr_0005_allergies-details.png)](./assets/images/examples/allergy-list/Um_Ehr_0005_allergies-details.png "Figure 7.25 - Progressive Disclosure in an Allergy List")</div>
#### 7.2.5 Goal, Execute, and Evaluate!

**Humans have a thought cycle that guides decision making and it is 'Goal, Execute and Evaluate.'**

How do we get anything done? No, really. We start by forming a goal: get some food, edit a word document, impress our boss with our design skills, etc. Next we choose and execute actions that we think will help us accomplish that goal. Finally, we evaluate how well our actions worked. Were we able to accomplish our goal, or to at least make progress towards accomplishing it?

Interfaces can support clinical decision making if their designers establish a shared understanding of goals with physicians. The interfaces must then provide users with clear paths by which to accomplish these goals, useful 'action' choices, and the feedback they need to quickly and accurately make choices and evaluate their progress. If interfaces don't provide appropriate or sufficient feedback, users make errors and find the interface unsatisfying to use. This is a common problem with interfaces.

#### 7.2.6 Go with the Flow

**People like to get into flow states; if we're engrossed in what we're doing, everything else falls away**

We've all had moments where we get so involved in what we're doing that we lose track of time and get a lot done. This situation is called a 'flow state,' and you can enter it doing professional or (more likely) recreational tasks. No one likes having their flow state interrupted.

Interfaces can help users get into and stay in flow states. Some facts to remember:

*   People like being in control of themselves. Giving them control over their activities will help them get into the flow.
*   Distractions, in the form of noisy interfaces or interruptions from co-workers, interrupt peoples' flow.
*   People like goals that are challenging but achievable.
*   Break difficult tasks down like you would unmanageable amounts of information. Allow users to complete long or difficult tasks in clearly-defined stages.
*   Give users feedback on their progress. Seeing how far they've come and how far they still have to go can motivate people.

**Example**:[Figure 7.26](#fig-7-26) shows a medication list that a patient is in the process of updating. The page indicator on the bottom shows the patient that he's on step 2 of 22\. This information about his progress may help the user get into a flow.

<div class="example" id="fig-7-26"><div class="ex-title"><span class="ex-type">Figure 7.26</span><span class="ex-caption">Tracking Progress via Page Indicators<span class="capt-desc">— The dots along the bottom of the screen show the user where he is in the process.</span></span></div>[![dots along the bottom track progress](./assets/images/examples/medication-reconciliation/UmEhr_MedRec_0012_patient_stepmed_nottaking.png)](./assets/images/examples/medication-reconciliation/UmEhr_MedRec_0012_patient_stepmed_nottaking.png "Figure 7.26 - Tracking Progress via Page Indicators - The dots along the bottom of the screen show the user where he is in the process.")</div></div></div></section><section id="manage-information"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 7.3 How People Manage Information

</div>
#### 7.3.1 Information Chaos

> Too much information going through my brain, too much information driving me insane.  
> <span class="quote-author">- The Police</span>

Five things lead to a state John Beasley and his colleagues have called information chaos: information overload, information underload, information conflict, erroneous information, and information scatter.

**Information overload** happens when we're being asked to make sense of information quickly, but there's too much information for us to do so. This makes us tired and even anxious. It also reduces our situational awareness. Without good situational awareness, we can miss important information because we're 'unable to hear the signal for the noise.'

**Information underload** happens when we lack sufficient information to make decisions.

**Information conflict** happens when an interface gives us contradictory information or information contradicting what we already know.

**Erroneous information** is information that, for whatever reason, isn't correct.

**Information scatter** happens when someone has access to all the information they need, but it's in several locations or formats and can't easily be reconciled into a complete picture.

If an interface allows for any of the above issues, a doctor could miss noticing important information, like a dangerously high blood pressure reading, and put her patient at risk.

**Example**: This walkthrough demonstrates the factors involved in information chaos.

<div class="example" id="fig-7-27"><div class="ex-title"><span class="ex-type">Figure 7.27</span><span class="ex-caption">Information Chaos</span></div>[![Information Chaos](./assets/images/examples/human-factors/UM_EHR_0011_info-chaos.png)](./assets/images/examples/human-factors/UM_EHR_0011_info-chaos.png "Figure 7.27 - Information Chaos")<div class="credit">

Reproduced by permission of the American Board of Family Medicine

</div></div>
#### 7.3.2 Situational Awareness

**Interfaces must help users put all the elements of complex situations into perspective so they can make good choices**

Situational awareness is an important component of everything from ordinary tasks like driving a car to emergency services. Effective EHR displays can improve users' situational awareness by presenting them with key information without disrupting their work.

It's difficult to design EHRs that can improve users' situational awareness, however, because the information users need varies depending on both the user and the task at hand. What's important for the user to know about one patient may not be important for them to know about another. Yet despite the situation's complexity, designers can meet this challenge. If a patient has a chronic disease such as diabetes or hypertension, an interface can help users quickly assess and manage these conditions. The interface need never force users to stop, for example, writing up an e-prescription to go look for the lab result they need in order to calculate a proper dose. Designers need to strike a balance between giving users lots of information to boost their situational awareness, and overwhelming them (see information overload).

Users' situational awareness suffers when they're distracted. If two children are arguing in the back seat, the car's driver won't be able to give her full attention to the road. Similarly, alerts about laboratory values may be important, but they may also distract a physician who's trying to order a medication and cause her to make a mistake.

</div></div></section><section id="summary"><div class="container"><div class="sixteen columns"><div class="sectionStart">
* * *

### 7.4 Summary

1.  Human Factors Engineering seeks to improve human performance by designing systems that are compatible with our physical, cognitive, and perceptual abilities.
2.  We subconsciously use expectations, past experience, associations, and rules of thumb to make guesses about what we are seeing. This lets us cope with noisy, incomplete data, but can also lead us astray.
3.  We have two modes of thinking, fast thinking that happens with little conscious effort and slow thinking that takes focus. Good design lets us use our fast system to do as much as possible.
4.  Working memory is limited to four things. Good design minimizes the need to use working memory.
5.  The more we have to remember and calculate in our heads, the higher the cognitive load. Good design reduces cognitive load by reducing the need to remember information and displaying information that can be used in decision making without additional calculations or navigation.
6.  Good information system design allows a user to quickly gain or maintain the situational awareness needed to make safe and effective decisions.

</div></div></div></section></section>