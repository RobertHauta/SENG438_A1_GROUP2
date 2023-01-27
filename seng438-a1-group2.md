>   **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group: 2      |
|-----------------|
| Jana                |   
| Robert              |   
| Ernest               |   
| Joshua                |   


**Table of Contents**

(When you finish writing, update the following list using right click, then
“Update Field”)

[1 Introduction	](#introduction)

[2 High-level description of the exploratory testing plan	](#high-level-description-of-the-exploratory-testing-plan)

[3 Comparison of exploratory and manual functional testing	](#comparison-of-exploratory-and-manual-functional-testing)

[4 Notes and discussion of the peer reviews of defect reports	](#notes-and-discussion-of-the-peer-reviews-of-defect-reports)

[5 How the pair testing was managed and team work/effort was
divided	](#how-the-pair-testing-was-managed-and-team-workeffort-was-divided)

[6 Difficulties encountered, challenges overcome, and lessons
learned	](#difficulties-encountered-challenges-overcome-and-lessons-learned)

[7 Comments/feedback on the lab and lab document itself ](#commentsfeedback-on-the-lab-and-lab-document-itself)

# Introduction

As a group in SENG 438 Lab 1, we will familiarize ourselves with three simple testing strategies, 
as well as concepts such as the system under test (SUT) and defect tracking systems.
Firstly, general exploration of the SUT and defect tracking will be performed. Each member will
understand the high level requirements of the software (Appendix B) so that meaningful testing can be done.
Secondly, members will learn how to right detailed and effective bug reports.

The testing methods to be used are:
    1. Exploratory (Manual Non-Scripted) Testing
    2. Manual Scripted Testing
    3. Regression Testing (verification of Defect Fixes)

The exploratory testing will be performed in pairs within the group. In each pair, one student will
perform tests while the other analyzes and records the results. Manual scripted testing will be 
performed as a group, following the test suite provided in Appendix C of the lab document. Finally,
all recorded defects will be re-tested to verify they have been fixed. If bugs persist, they will
be reported and attributed to the new version using the defect tracking system.

Exploratory testing is testing that attempts to create realistic scenarios the system may encouter. Rather than
developing a comprehensive and explicit testing suite, testers will probe the system and execute steps in an iterative manner.
The goal is to create human-realistic scenarios to uncover bugs and defects.

Manual scripted testing follows a strict set of instructions developed by the tester. This allows a detailed 
and thorough evaluation of all system functionalities. The developed test suite will act as an explicit guideline to 
indivdiually test all features and isolate any detected bugs.

# High-level description of the exploratory testing plan

Ernest and Jana decided to user a general approach to the exploratory testing. Over the testing period,
we tested each function broadly so we could test as many functionalities as possible.
We tested each funcionality in the way a user would typically interact with the system, such as
withdrawing or depositing a normal amount of cash, transfering funds between valid accounts, and checking the balance
of existing accounts tied to the card. We also tested how the system would behave if the user incorrectly entered
their pin by accident.

Robert and Joshua's goal was to test the basic functionalities in a broad perspective as well. We separated the functionalites 
and approached each step-by-step. We tried to imagine how a typical user would expect the system to function, and we created scenarios 
that would test these features. When a bug was encoutered, we stopped testing, recorded the bug, then proceeded on to higher functionalites.
In addition to expected functioality, we also tested how the ATM system handles invalid inputs. We explored invalid account information and
illegal withdrawal, deposit, and transfer operations. Forcing the system to respond to incorrect input accounted for most of the reported bugs,
as these behvaiours were often not handled properly by the system.

# Comparison of exploratory and manual functional testing

Exploratory testing uncovered a lot of bugs, however it was difficult to isoloate their causes. Although exploratory testing
was informative, tracking the causes-and-effects was a little ambiguous. This testing seemed to be effective in identifying the presence
of bugs, but not necessarily the specific locations or causes. Additionally, our exploratory testing yield a number of "compound bugs" or
scenarios where multiple faults were identified. For example, by exploring the deposit feature, we found issues in the actual deposit logic, the
receipt display, and the log functionality. These tangled issues made evaluting the system over-whelming and tedious.

Contrastingly, manual functional testing was very thorough and simple. The break-down of use cases allows for comprehensive, iterative testing
of all possible input and output combinations. Each ATM functionality has multiple components in its expected outcomes (transaction, display, receipt, 
and log), so separating each of these features was very helpful in isolating the bugs' locations. Furthermore, having a defined test suite allowed us 
to tangibly evaluate the performance of newer versions. Conceptualizing the test suite as functionality checklist makes comparing Version 1.0 and Version 1.1
of the ATM an intuitive and standardized process.

# Notes and discussion of the peer reviews of defect reports

Overall, our testing experiance in pairs was efficient. We could quickly and effectively  work together with one person testing for bugs while 
another reported them in the DevOps defect tracking system. Azure was a very good bug defect reporting program because it allowed us to easily 
report the bugs we foundas well as collaborate together in finding the bugs. It was as very easy to see everything other people reported, and track
the progress and state of each bug. We noted that is it very important to make detailed and informative bug report so there is no ambiguity as to where
the bug was found. Additionally, working together in two seperate pairs helped us find more bugs as the different pairs had different testing methods, which 
resulted in wide variety of bugs found.

# How the pair testing was managed and team work/effort was divided 

During the exploratory testing phase, we split into pairs. One group had Ernest and Jana, and the other had Robert and Joshua. 
A 30 minute timer was set for exploratory testing. During this period, each pair independently went through Version 1.0 and reported 
any bugs discovered during that time. At the end of the 30 minutes, each pair compared the bugs they reported in the defect tracking system. 
While testing, each pair used a strategy of one member serving as the system tester and the other reporting bugs as they were found.

After exploratory testing, the group moved into manual testing, Robert shared his screen and went through the 40 use cases in the test suite (Appendix B of the lab documents) while Jana, Ernest, and Joshua documented any bugs discovered. This strategy was helpful as all group members had a clear idea of the tests being performed.

We then performed regression testing on the next version of the program (Version 1.1.). A similar approach to the manual testing was done; Robert shared his screen and 
tested the system, while Jana, Ernest, Joshua reported all the bugs that were found. We tested all the bugs that were reported in the prior two phases. If a bug persisted, its recorded was updated to note its persistence. If a bug was resolved, its record was also updated accordingly.

Finally, we performed scripted testing by assessing Version 1.1 using the test suite, similar to how we assessed Version 1.0 above. We reported any new bugs we found.

# Difficulties encountered, challenges overcome, and lessons learned

There have been a few issues that we encountered. One of the difficulties was that it was hard to combine the reports of the two pairs of groups in the exploratory phase as there was overlap and redundancy in the found bugs. It was also hard to find the bugs that were repeated twice in the defect tracking system. We also had difficulty as a group getting started with Azure DevOps, as we did not initially know how to report bugs. We also had difficulty sharing one board with the rest of the team members. Another challenge is that some of us had difficulty getting started with GitHub and simultaneously working on one file. Some of the lessons learned are that we now know how to effectively use GitHub and Azure DevOps for future labs. Also, we learned how to report bugs. Another lesson learned is that we know how to find a bug in a system, and test its persistence using the testing techniques described above.

# Comments/feedback on the lab and lab document itself

We found this lab generally valuable. We feel this lab offers a digestible introduction to formalized software testing. This lab also provides a helpful
introduction to defect tracking systems and the process of reporting bugs.

We found the submission format (.md file on GitHub with an additional bug report in a .md/Excel/PDF file) to be a little bit confusing.
We are not incredible familiar with GitHub, so we are experiencing a steep learning curve. In the future, more specific submission instructions may be helpful.
