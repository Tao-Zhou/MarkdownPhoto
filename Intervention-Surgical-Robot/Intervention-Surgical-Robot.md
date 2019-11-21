# Intervention-Surgical-Robot

#### 1.《[Analysis of Interventionalists’ Natural Behaviors for Recognizing Motion Patterns of Endovascular Tools during Percutaneous Coronary Interventions](https://www.researchgate.net/publication/330326952_Analysis_of_Interventionalists'_Natural_Behaviors_for_Recognizing_Motion_Patterns_of_Endovascular_Tools_during_Percutaneous_Coronary_Interventions)》

#### Journal: [IEEE Transactions on Biomedical Circuits and Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=4156126)-----2019

**Abstract**—Many robotic platforms can indeed reduce radiation exposure to clinicians during percutaneous coronary intervention (PCI), however, interventionalists’ natural manipulations are rarely involved in robot-assisted PCI. This requires more attention to analyze interventionalists’ natural behaviors during conventional PCI. In this study, four types of natural behavior(i.e., muscle activity, hand motion, proximal force and finger motion) were synchronously acquired from ten subjects while performing six typical types of guidewire manipulation. These behaviors are evaluated by a hidden Markov model (HMM) based analysis framework for relevant behavior selection. Relevant behaviors are further used as the input of two HMM-based classification frameworks to recognize guidewire motion patterns. Experimental results show that under the basic classification framework (BCF), 91.01% and 93.32% recognition accuracies can be achieved by using all behaviors and relevant behaviors, respectively. Furthermore, the hierarchical classification framework (HCF) can significantly enhance the recognition ability of relevant behaviors with an accuracy of 96.39%. These promising results demonstrate great potential of proposed methods for promoting the future design of human-robot interfaces in robot-assisted PCI.

![]( https://raw.github.com/Tao-Zhou/MarkdownPhoto/master/Intervention-Surgical-Robot/images/1.png )

**Motivation:** 

1. The natural behaviors captured during surgical procedures are mainly used for the purpose of skills assessment. It is envisaged that such behaviors can also be applied to the motion pattern recognition of endovascular tools for facilitating the development of novel human-robot interfaces (HRI). Unfortunately, there are few studies looking at this issue.
2. Redundancy analysis of natural behaviors is seldom discussed in the researches mentioned above.
3. The relevance of behaviors also has rarely been discussed in existing studies.

![](https://raw.github.com/Tao-Zhou/MarkdownPhoto/master/Intervention-Surgical-Robot/images/3.png)

**Contribution:**

1. EMG, EM, accelerometer and fiber-optic bend sensors are integrated to simultaneously record interventionalists' natural behaviors during manual PCI.
2. An HMM-based analysis framework is developed to evaluate multimodal behaviors for selecting relevant behaviors, which are further used to recognize guidewire motion patterns by two HMM-based classification frameworks.
3. Experimental results show that 93.32% recognition accuracy can be obtained using relevant behaviors under the basic classification framework, much higher than 91.01% using all behaviors, and it can be further improved to 96.39% under the hierarchical classification framework.

![](https://raw.github.com/Tao-Zhou/MarkdownPhoto/master/Intervention-Surgical-Robot/images/4.png)

​                                                           the basic classification framework (BCF)



![](https://raw.github.com/Tao-Zhou/MarkdownPhoto/master/Intervention-Surgical-Robot/images/6.png)

​                                                  the hierarchical classification framework (HCF)

**Comment:**

This paper provides HMM-based frameworks for the analysis of interventionalists’ natural behaviors and the recognition of endovascular tool motion patterns during conventional PCI.