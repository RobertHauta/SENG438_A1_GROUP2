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

[1 Introduction	1](#Introduction)

[2 High-level description of the exploratory testing plan	1](#_Toc439194678)

[3 Comparison of exploratory and manual functional testing	1](#_Toc439194679)

[4 Notes and discussion of the peer reviews of defect reports	1](#_Toc439194680)

[5 How the pair testing was managed and team work/effort was
divided	1](#_Toc439194681)

[6 Difficulties encountered, challenges overcome, and lessons
learned	1](#_Toc439194682)

[7 Comments/feedback on the lab and lab document itself	1](#_Toc439194683)

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

Text…

# How the pair testing was managed and team work/effort was divided 

Text…

# Difficulties encountered, challenges overcome, and lessons learned

Text…

# Comments/feedback on the lab and lab document itself

We found this lab generally valuable. We feel this lab offers a digestible introduction to formalized software testing. This lab also provides a helpful
introduction to defect tracking systems and the process of reporting bugs.

We found the submission format (.md file on GitHub with an additional bug report in a .md/Excel/PDF file) to be a little bit confusing.
We are not incredible familiar with GitHub, so we are experiencing a steep learning curve. In the future, more specific submission instructions may be helpful.
