Select /two/ articles that describe a method or technique for LSRE.
- Implement the two techniques.
- Keep a running log of your selection and implementation, with experiences therefrom.
- [-] Write a Report:
- [X] /Article Selection:/ Which articles have you chosen, and why?
- [ ] /Implementation Plan:/ How do you plan on implementing the proposed technique/method?
- [ ] /Execution:/ Describe what you have done.
- [ ] /Proof of Concept:/ Run through a worked example of using your implementation
- [ ] /Lessons Learned:/ What did you learn about LSRE/MDRE and the implementation?
- [ ] /Reflections:/ How does your implementation, and your experiences, relate to what other /research/ articles say?

Comments:
Article motivation: What defects are there, and /why/ do you think they are easy to use and implement? Empirical evidence?

RFC2119 tells you wether to use MUST, SHALL, SHOULD, or MAY to define how important a requirement are. Please adhere to this.
Seven Requirements? Anything is easy with so few requirements and you are not going to run into any relevant challenges at all.

There is no trail to properly see how you applied the two techniques -- I only see the results.

Where in your execution did you learn the lessons you state under "lessons learned". There is no connection to what you did and what you learned.
Please discuss your lessons learned.

Todo in order to Pass:
- Describe the two methods better.
- Describe in detail how you apply them.
- Apply them on a larger base of requirements.
- Discuss the lessons learned in connection to what you have done.
- Reflect and relate your lessons to literature.


##Selected article: 
Requirements Abstraction Mode

A Method for Early Requirements Triage and selection Utilizing Product Strategies 
 

##Why: 

There are eighteen articles as the alternative reference literatures. I have selected those two papers because they have logic which can use in different steps for requirement analysis of a project. The ‘A Method for Early Requirements Triage and selection Utilizing Product Strategies’ introduces a method to help analyze the requirement triage and product strategies. And the other article, ‘Requirements Abstraction Mode’, shows a model which can further analyze the requirement. In the mode, the requirements will be refined into smaller one for further design and development.

It is critical for product management to select the requirements aligned with the overall business goals and discard others as early as possible. Due to the emergence of markets for off-the-shelf or packaged software, the result is a large amount and continuous flow of requirements that threaten to overload the development organization. MERT could combine the strategic and technical perspectives to formulate product strategies that are good-enough. MERTS takes strategic and technical views into account, so that it can acts as a stepwise guide to creating product strategies. The strategies resulting from MERTS can be used by managers to perform requirements triage 

for early requirements triage and selection. These two papers help define excutable requirements, which is useful and practical in software development process. And based on each saminer,  I think the techniques provided by these papers are easy to understand and implement, though there are some defects in them.


##Implementation Plan:

- Use the method from Requirements Abstraction Model to break down requirements.

- Use the method from A Method for Early Requirements Triage and selection Utilizing Product Strategies to calculate the points of each requirement.

1. Based on the prerequisites of the proposed methods, and the limitation of my research, the implementation plan focus on the scoping of the tested project firstly. The project should be market-driven and available for one master student research.
2. Selecting a project as the experimental material to apply the methods which are proposed in selecting papers is the next step.
3. Using the method from ‘A Method for Early Requirements Triage and selection Utilizing Product Strategies’ to calculate the points of each requirement.
4. Using the method from ‘Requirements Abstraction Model’ to break down the requirements from the tested project.

##Excution:
####1.Technique from Requirements Abstraction Model to break down requirements.

I have chosen a case, which is a windows application, named Hotel Management System, the target customers are hotels. The system should include management sub-system and back office sub-system. And I presents some basic requirement of Hotel Management System, I will break down parts of them according to 'Requirement Absreaction Model'. Additionally, most requirements are from my own experience and some are from network. 


####2.MERTS

According to the case of first technique, there is one requirement named payment, it is a good instance for this technique. Based on 
the paper,'A method ', I will resent a table to presents the excution of this technique. Due to this is a report on Github, the table 
is translated into plaintext.


##Proof of Concept:
####1.Technique from Requirements Abstraction Model to break down requirements.

Step 1 Specify

| ----- | Description | Reason/Benefit/Rationale| Restrictions/Risks |
| :-------------: | :-------------: | :-------------: |:-------------: |
|Booking |The system should be able to input and modify booking information | WHY: The user want to input and modify booking information.BENEFIT: the user can use this system to book for guests. |The length and type of input text should be restricted.|
|Check-in | The system should be able to input and modify check-in information |WHY: The user want to input and modify check-in information.BENEFIT: the user can use this system to check in for guests|The length and type of input text should be restricted. The system should be used to confirm the identity information of the user is legitimate|
| Payment | The system should provide interfaces to kinds of external payment systems and record the payment information |WHY: The guests need to pay for their romms by using different credit card and cash and the hotel need payment information for management. BENIFIT: Make the usage of the system more attrctive |The security of information is an issue |
|Reception management|The system should be able to check, modify guest information, room information, and set room information|WHY: Guests sometimes may change their schedule and the rooms may need renovate. BENIFIT: Make the system more flexible.|This may conflict with booking and check in if not promptly update.|
|Back Office management|The system should be able to manage the privilege of the system and modify the state of rooms|WHY: The system are only used by reception staff of a hotel. BENEFIT: Ensure the the security of the guest information and hotel information.|The security of system is an issue.|
|Record|All the information and operation information should be record.|WHY: The managers of hotel or other people may need the information. BENIFIT: If there is an accident, the system can provide some evidence.|Customer information and hotel information may be stolen.|
|Check-out|The system should be able to check out for guests.|WHY: The user want to check out for guest. BENIFIT: the user can use this system to check out for guests.|Only the user has privilege can check out for guests.|

