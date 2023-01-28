>   **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group: 2      |
|-----------------|
| Oliver Molina                |   
| Daniel Picazo              |   
| Quentin Jennings              |   
| Nouruddine Jaffan              |   


**Table of Contents**



[1 Introduction	1](#introduction)

[2 High-level description of the exploratory testing plan	1](#high-level-description-of-the-exploratory-testing-plan)

[3 Comparison of exploratory and manual functional testing	1](#comparison-of-exploratory-and-manual-functional-testing)

[4 Notes and discussion of the peer reviews of defect reports	1](#notes-and-discussion-of-the-peer-reviews-of-defect-reports)

[5 How the pair testing was managed and team work/effort was
divided	1](#how-the-pair-testing-was-managed-and-team-workeffort-was-divided)

[6 Difficulties encountered, challenges overcome, and lessons
learned	1](#difficulties-encountered-challenges-overcome-and-lessons-learned)

[7 Comments/feedback on the lab and lab document itself	1](#commentsfeedback-on-the-lab-and-lab-document-itself)

# Introduction

Functional testing is an important and essential part of the software development lifecycle. To ensure the program works correctly in all cases many tests should be performed to detect any defects and resolve them before damage can be caused. Our group was tasked with performing testing on an ATM simulator and reporting any bugs found. In order to do this we needed to apply our knowledge on exploratory and manual functional testing on both the system’s initial version, 1.0, and the following version, 1.1. Our functional testing started with exploratory testing, or human-based testing, in which we used our knowledge of the domain provided in the assignment description to selectively test values. Afterwards we performed manual scripted testing using the pair testing method on each case in a given test suite in which we must follow a provided script to check for defects.

Once we have finished performing the two types of functional testing on version 1.0 we had to check what defects the following version 1.1 actually patched. To do this we performed regression testing and re-tested the defects previously found to see if functions work properly or if the failures were addressed. We followed it up by performing manual scripted testing once more in an attempt to find new defects caused by the patch.

Following will be a more in-depth description of our process and results.


# High-level description of the exploratory testing plan

Our team separated into groups of two for our exploratory testing since the different approach of each group would likely lead to the most bugs being caught. Both of our groups had similar approaches in exploratory testing in which edge cases would be rigorously tested followed by targeting the most complex functions with interactions between multiple systems. Typical cases such as invalid or incorrect inputs often output errors as expected as well as the receipt printing and transferring functions.

The reason we chose a similar approach is because it was the most optimal use of our limited half-hour time - it was common that we would run into standard usage bugs along the way, covering more ground at once without repeating ourselves many times inefficiently. There were a few minor differences between group approaches however, most notably that one group focused mostly on menu errors and errors involving account type and the other group focused on edge cases such as invalid inputs.


# Comparison of exploratory and manual functional testing

Each group member spent approximately 30 minutes conducting exploratory tests and through those tests we discovered the majority of our problems here compared to the manual testing. Of the reported bugs only three were discovered in manual testing that we did not come across in our experimental tests. We believe this is because our exploratory testing did a better job targeting potential areas of defect compared to the given test suite, which mostly covered normal user usage and not edge cases. For instance, the test suite did not test invalid account types or invalid inputs which meant that it would not catch quite a few major defects. It was able to catch errors that would occur with normal customer usage, such as deposits not depositing the correct amount, but these errors were caught within our previous exploratory testing.

In this assignment our exploratory testing was much more efficient and found many more bugs than the manual testing because of the previously-discussed flaws with the test suite.

# Notes and discussion of the peer reviews of defect reports

There were several errors with our defect reports caught through our peer reviewing session, most often with simply forgetting a detail such as the affected version. In one occasion a bug that was initially noted as patched was retested and found to still be an issue highlighting the importance of the peer reviewing step. All such disputes were immediately handled and the bug reports were updated to reflect the new findings.

# How the pair testing was managed and team work/effort was divided 

The group of four members was split into two smaller groups of two. The first small group did exploratory testing for approximately 30 minutes before conducting half of the manual scripted testing. After the fact, the second group did their own same-length exploratory testing followed by continuation of the manual scripted testing, as well as reviewing the reported bugs by pair 1. This team then did half of the manual scripted testing for the 1.1 fix release, which then the first group returned to review what had been done and finish the manual scripted testing. Both groups came together at the end to discuss the found bugs and fixes, as well as what we learned throughout the testing process. Work was split evenly and all members contributed an equal amount to the assignment.

# Difficulties encountered, challenges overcome, and lessons learned

The first major difficulty was adapting to and learning a new environment; in our case, this was Jira. A decent while was spent learning our way around the Jira environment and getting used to its tools. As well, learning how the program worked was a must before we could begin to effectively test it. We overcame these difficulties by working together to learn Jira and the program as a group rather than individually, to ensure we all understood what was needed. We learnt that programs often require a lot more testing than expected, especially for small interactions one would normally assume works, there could always be some minor to major defect hidden in an obscure interaction in the program.

# Comments/feedback on the lab and lab document itself

The suite of test cases provided in the lab document was effective at testing the most basic functionalities of the system but failed to assess the majority of bugs we encountered in the system. This is likely intentional and we believe the effects of a bad test suite should be emphasized in the report of the lab. 