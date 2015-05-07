## 1

##  本书简介

* * *

###  目标

我们编写此书的目的在于通过介绍一些临床场景和观点来**启发**兼具实用性和可用性的电子病历系统的设计，其中伴有基本设计原则指导下形成的交互式设计的范例。

Our goal in writing this book is to**inspire** useful and usable Electronic Health Record (EHR) interface design by providing clinical scenarios and insights with examples of interactive designs, guided by basic design principles.

### 说明性的并非规定

尽管有意义的使用的标准影响了该书主题的选择，我们和我们的支持者们(California HealthCare Foundation and SHARP-C Project)希望这本书能够与临床有关，具有说明性，有启发性，但**并不是什么规定**，希望我们的设计范例能够在读者改进各自的系统设计时有所启发。   

While meaningful use criteria influenced the choice of the book topics, we and our supporters (California HealthCare Foundation and SHARP-C Project) want this book to be clinically relevant, illustrative, and inspirational —but**not prescriptive**. We hope our design examples will inspire our readers to improve their own EHR designs.

### 受众

该书适合**任何开发和实现医疗IT系统的人员**，但特别适合那些想学习更多人为因素和设计相关知识的电子病历供应商的团队人员。那些想了解电子病历用户需求的设计人员、医学信息学的学生、想要学习更多设计原则的电子病历系统用户也能从该书中受益

This book is written for**anyone who develops and implements health IT applications**, but particularly for electronic health record (EHR) vendor teams who want to learn more about human factors and design. Designers who want to learn about the needs of EHR users, medical informatics students, and EHR users who want to learn more about design principles might also benefit from reading this book.

### 关注点


1.  **聚焦在临床**: 该书关注的是**成人的门诊护理**。我们的范例特别强调了**全科医生**的需求。
2.  **聚焦在电子病历的功能上**: 我们的范例试图解决5个领域：用药列表、用药核对、过敏列表、电子处方和药品警告

我们希望后续的书中可以解决其他临床上的需求和其他能够让电子病历兼具可用性和有用性的设计中的很多其他部分，这样它们才能够被谨慎的实现，无缝地与医疗机构衔接起来。

1.  **Clinical focus**: This book focuses on**ambulatory adult care**. Our examples especially emphasize the needs of**primary care** practitioners.
2.  **EHR functionality focus**: Our design examples seek to address five specific areas: medication list, medication reconciliation, allergy list, e-prescribing and drug alerts.

We hope that future books will address other clinical needs and the many other elements that EHR designs require to be useful and usable, so they can be carefully implemented and seamlessly integrated into healthcare organizations.

### 章节概述

后续的5章每章聚焦一个特殊的电子病历的功能(用药列表、用药核对、过敏列表、电子处方和药品警告)。讨论了基本的临床需求和可用性的问题，简单的描述了人们在使用电子病历的用户界面时，一般是如何查看、阅读、关注、思考、记忆和作出决定的。


The next five chapters each focus on a specific EHR functionality (medication list, medication reconciliation, allergy list, e-prescribing and drug alerts). Basic clinical needs and usability issues are discussed, with simple descriptions of how humans typically see, read, pay attention, think, remember, and decide when using EHR user interfaces.

每章开篇是一到多个**临床场景**。从人的角度来描述，能够帮助读者体会电子病历系统的用户和他们的难处。每章都会有很多**设计范例**。其中有一些是简单的带标记的图片(要么是单张，要么是多张一个系列),更为详细的设计范例使用了交互式原型，能够让用户亲自体验，还附带了演示视频。每章的末尾都是对每章提到的要点的总结。


Each chapter starts with one or more**clinical scenarios**. This brings a human perspective and will help readers empathize with EHR users and their struggles. Each chapter includes many**design examples**. We present simple examples with annotated figures (either single images or galleries showing a series of images). The more elaborate design examples use interactive prototypes that give readers a hands-on experience and video demonstrations. Finally, each chapter ends with a summary of the important points covered therein.

这5章采用的是平常的语言，任何读者都可以查看。除了在最后三章为有兴趣学习更多的读者给出了**相关设计原则的链接**。

Those five chapters use plain language and are accessible for all readers. In addition they provide**links to related principles** found in the last three chapters for the benefit of those who wish to learn more.

本书后三章涉及了**设计的原则**、**人文因素**、**医疗IT可用性**三方面。它们为读者提供人类大脑如何工作以及视觉设计的基本原则的基本理解，为开发人员设计具有可用性的用户界面建议了一些步骤。这里的内容只是对某个主题的简单介绍，但我们对那些想要深入学习的读者给出了参考文献。

The book’s last three chapters cover**principles of design**,**human factors**, and**health IT usability**. They aim to provide readers with a basic understanding of relevant information about how the human brain works and fundamental principles of visual design to suggest steps developers can take to create usable user interfaces. The content herein provides an introduction to the subject, but we also offer recommendations for those interested in reading further.

该书中提到的所以医生和患者都是虚构的。该书中的设计范例是由我们的团队所设计的，接受了国际级的临床和人文学家的评审，但并没有对现有的设计在实际中做任何检验。

All patients and physicians mentioned in the book are fictitious. The designs in this book were created by our team and reviewed by a national panel of clinical and human factors experts, but have not been empirically tested against existing designs.

### 如何使用本书

读者可以以任何顺序来阅读本书。不过，我们鼓励读者按照我们的章节顺序。比如在第2章(用药列表)中引入了后续章节用到的诸多基本概念。

This book’s chapters can be read in any order. Nevertheless, we encourage you to read them in the order our layout proposes. Chapter 2 (Medication List), for example, introduces basic concepts that are reused in subsequent chapters.

### 意见反馈

 欢迎发送邮件至[feedback@inspiredEHRs.org](mailto:feedback@inspiredEHRs.org?Subject=EHR%20feedback).欢迎大家的评论。务必告诉我们在后续的版本中你们还想看到哪些额外的主题。 我们会在[TooManyClicks.com](http://toomanyclicks.com/)发布来信当中的一些有价值的范例或者观点。
 
 We welcome your comments. Please let us know what subjects you would like us to cover next. We will post the helpful examples or insights you send our way to Jeff Belden’s blog at[TooManyClicks.com](http://toomanyclicks.com/).


译者注：      
1、user interfaces 用户界面        
2、human factor 人因         参考http://baike.baidu.com/link?url=VjqsyS0uD2WtPw9DZ9nDtpPPSsT0cCgf67eF2NTjCETMWuOlPYS6zeCxpc9SWLvyNG2eHWj6pSQvG0jRjfsf9K        

http://baike.baidu.com/link?url=VjqsyS0uD2WtPw9DZ9nDtpPPSsT0cCgf67eF2NTjCETMWuOlPYS6zeCxpc9SWLvyNG2eHWj6pSQvG0jRjfsf9K        
3、 medication reconciliation 用药核对  赵新远老师译作用药比对 药物比对  这里现没有约定俗成的译法。

