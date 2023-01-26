
>   **SENG 438 - Software Testing, Reliability, and Quality**


**Lab. Report \#1 – Introduction to Testing and Defect Tracking**


| Group: Group Number 4 |
|---------------------|
| Student 1 Andrew Howe
| Student 2 Alexander Sembrat
| Student 3 Hajin Kim
| Student 4 Jenna Vlaar


**Table of Contents**


[1 Introduction ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#introduction)

[2 High-level description of the exploratory testing plan   ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#high-level-description-of-the-exploratory-testing-plan)

[3 Comparison of exploratory and manual functional testing  ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#comparison-of-exploratory-and-manual-functional-testing)

[4 Notes and discussion of the peer reviews of defect reports   ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#notes-and-discussion-of-the-peer-reviews-of-defect-reports)

[5 How the pair testing was managed and team work/effort was
divided ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#how-the-pair-testing-was-managed-and-team-workeffort-was-divided)

[6 Difficulties encountered, challenges overcome, and lessons
learned ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#difficulties-encountered-challenges-overcome-and-lessons-learned)

[7 Comments/feedback on the lab and lab document itself ](https://github.com/AlexSembrat/Seng438-a1/blob/main/seng438-a1-group4.md#commentsfeedback-on-the-lab-and-lab-document-itself)




# Introduction

Exploratory testing involves using intuition on how a user is meant to interact with the program to guide testing. Manual functional testing involves the use of automation tools or a specific guideline to follow when testing. These tools are created based on the goals of the program and the severity of each use case. Exploratory testing is very effective at ensuring that realistic use cases of the system are entirely bug-free while manual functional testing is effective at ensuring each feature meets the requirements of the system. We will be exploring both methods of software testing and determining the advantages and disadvantages of each method by recording our defect reports in Azure. 


# High-level description of the exploratory testing plan

High-level testing plan rough draft based on the requirements of the ATM:

1. Test functionality of ON/OFF (machine should not work when off etc.) Machines should not be allowed to turn off while servicing a customer.
2. Test validation of card and pin, assert proper functionality
3. Test withdrawal function, assert correct amount withdrawn, test unnatural values(negatives, alphabetical, symbols, etc)
4. Test deposit function, assert all accounts can be accessed, assert correct values and error checking
5. Test transfer function, test multiple accounts(any two accounts linked should be able to be used)
6. Test balance inquiries
7. Test abort function, assert the process was actually aborted(values should be unchanged)
8. Test transaction verification. If the customer fails to deposit the envelope within the timeout period or cancels, a message should not be sent to the bank and the deposit shouldn’t be credited to the customer.
9. Test PIN security measures (too many failures)
10. Analyze given receipts for successful transactions. (date, time, location, type of transaction, accounts, amount, available balance of affected account).
11. Perform other random actions during processes (click buttons that are not supposed to be clicked to see if they do anything)


# Comparison of exploratory and manual functional testing


Exploratory testing was deemed to be about as effective at finding defects in the system as manual functional testing. This may have been because the system was not being tested against specific requirements for every single aspect of the system, rather was tested based on expected use. Exploratory testing led us to find more severe defects as we prioritized finding defects in the most critical parts of the system. Alternatively, manual functional testing was efficient at finding a wide variety of defects within the system. Some of these, however, were not as critical as those discovered with exploratory testing. The majority of defects we found in manual functional testing had already been discovered by exploratory testing.

Exploratory testing relies much more on the testers creativity and feel than the highly structured manual testing. This provides an advantage over manual testing as the random element of exploratory testing is far closer to the ATM’s real use case. Exploratory testing can also take longer than manual testing as the tester needs to think of what to test and in what way, while in manual testing the tester just follows the test instructions.

Manual testing provides an efficient and wide reaching scope of test cases that can test software functionality. Manual testing could be used to test every little potential problem with the system in an organized and systematic way, when compared to exploratory testing manual testing is much more organized which can be beneficial. One downside of manual testing is the preparation of the test cases. We did not have to prepare the 40 test cases provided to us; however, preparing a large number of manual test cases would take a tester a great amount of time and effort, especially compared to the more “go with the flow” exploratory testing.

Testing is a very important part of the software development life-cycle and both exploratory and manual testing have their places to ensure high quality, and reliable software is produced.

# Notes and discussion of the peer reviews of defect reports

Peer reviews gave the bug reports an opportunity to be double-checked. This allowed us to discover bug reports of issues that could not be recreated. In this case, these reports were discarded. Defect reports also opened an opportunity for discussion on how the bugs may be related or how they may be fixed. Reviewing each other’s defect reports also ensured there were no duplicate reports.

# How the pair testing was managed and team work/effort was divided

In pairs, we divided the system into logical parts. One team focused on withdrawals, and balance inquiries, while the other focused on deposits, entering bank info and transfers. In this way, the major functionality of the system is covered and finding bugs across the general use of the ATM is effective. 
We split our group into two halves with an approximately equal amount of work. From there, the groups delegated tasks between the two of them. One group member would test the system while the other reported those bugs to Azure. 
For manual testing we split the test up equally and any defects found were reported to Azure along with the version of the software that the bug exists in.

# Difficulties encountered, challenges overcome, and lessons learned


One of the challenges we found was that because we were totally unfamiliar with the system it caused the testing to be very slow at first, this became less of a problem as we got more familiar with the system and what was working on it. Another of the main challenges faced was prioritizing certain aspects of the design. We decided that we would put the majority of our work into finding bugs within deposits and withdrawals as they may result in the bank and/or the customer losing money. We learned that it is impossible to stress every single aspect of the design with exploratory testing, so it is important to focus on which features are most vital to the software.

# Comments/feedback on the lab and lab document itself


The lab document was not introduced in the lab session. It would have been easier to begin completing the lab if the guidelines were laid out for us in the beginning. The lab outline, specifically appendix C is poorly formatted and hard to decipher. Several of the test cases seem to merge with each other and are not clearly defined. However, the lab itself allowed us to gain experience using actual software that test engineers use in their daily life, so it was interesting to learn about these tools. 
