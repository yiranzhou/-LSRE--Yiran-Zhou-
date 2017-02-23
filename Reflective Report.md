#Reflective Report

##Selected article: 
Requirements Abstraction Mode
A Method for Early Requirements Triage and selection Utilizing Product Strategies 

##Why: 
These two papers help define excutable requirements, which is useful and practical in software development process. And based on each saminer,  I think the techniques provided by these papers are easy to understand and implement, though there are some defects in them. 

##Implementation Plan:

-Use the method from Requirements Abstraction Model to break down requirements.

-Use the method from A Method for Early Requirements Triage and selection Utilizing Product Strategies to calculate the points of each requirement.

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

Requirement 1 Booking

Description:The system should be able to input and modify booking information.

Reason/Benefit/Rationale: WHY: The user want to input and modify booking information.BENEFIT: the user can use this system to book for guests.

Restrictions/Risks: The length and type of input text should be restricted.


Requirement 2 Check-in

Description: The system should be able to input and modify check-in information.

Reason/Benefit/Rationale: 
WHY: The user want to input and modify check-in information. 

BENEFIT: the user can use this system to check in for guests. 

Restrictions/Risks: The length and type of input text should be restricted. The system should be used to confirm the identity information of the user is legitimate.


Requirement 3 Payment

Description: The system should provide interfaces to kinds of external payment systems and record the payment information

Reason/Benefit/Rationale: 

WHY: The guests need to pay for their romms by using different credit card and cash and the hotel need payment information for management. 

BENIFIT: Make the usage of the system more attrctive 

Restrictions/Risks: The security of information is an issue.

Requirement 4 Reception management

Description: The system should be able to check, modify guest information, room information, and set room information

Reason/Benefit/Rationale: 

WHY: Guests sometimes may change their schedule and the rooms may need renovate. 

BENIFIT: Make the system more flexible.

Restrictions/Risks: This may conflict with booking and check in if not promptly update.


Requirement 5 Back Office management

Description: The system should be able to manage the privilege of the system and modify the state of rooms

Reason/Benefit/Rationale:

WHY: The system are only used by reception staff of a hotel. 

BENEFIT: Ensure the the security of the  guest information and hotel information.

Restrictions/Risks: The security of system is an issue.


Requirement 6 Record

Description: All the information and operation information should be record.

Reason/Benefit/Rationale: 

WHY: The managers of hotel or other people may need the information.

BENIFIT: If there is an accident, the system can provide some evidence.

Restrictions/Risks: Customer information and hotel information may be stolen.


Requirement 7 Check-out

Description: The system should be able  to check out for guests.

Reason/Benefit/Rationale: WHY: The user want to check out for guest. BENIFIT: the user can use this system to check out for guests. 

Restrictions/Risks: Only the user has privilege can check out for guests.

Step 2 Place

According to the first step specify, the following is the abstraction level of requirements.

Product level: Reception management;Back Office management

Feature level: Booking;Check-in;Payment

Function level: Record

Conmponent level:Check-out


Step 2 to 1 Breakdown Requirement

According to the RAM, the requirements belong product and feature levels need to be broken down. I broke down Reception Managment and Payment as instances below.

-Reception management breakdown into function level:Query room state; Set room state; Supplement guest information

Requirement 8 Query room state 

Description: The system should be able to query room state.

Reason/Benefit/Rationale: WHY: The user want to check the state of room when new guests come. BENIFIT: the user can check in for new guests according to the result of query. 

Restrictions/Risks: The state does not get update timely.

Requiremnet 9 Set room state

Description: The system should be able to set room state.

Reason/Benefit/Rationale: WHY: The user want to set the state of room when the room is taken or need renovate. BENIFIT: the user can set the state of room when necessary. 

Restrictions/Risks: Only user who has the privilege can set room state. 

Requirement 10 Supplement guest information

Description: The system should be able to supplement guest information.

Reason/Benefit/Rationale: WHY: In some situation, the user may need to supplement guest information. BENIFIT: the user can record complete and correct information of guests. 

Restrictions/Risks: Only user who has the privilege can set room state. Supplementary information should be identified.

-Payment breakdown into functional level: record payment information;Interface to external payment system 

Requirement 11 Record payment information

Description: The system should be able to record payment information.

Reason/Benefit/Rationale: WHY: the hotel need payment data to complete financial statements. BENIFIT: Make the management of financial more convenient. 

Restrictions/Risks: The security is an issue.

Requirement 12 Interface to external payment system 

Description: The system should provide different interfaces for different external payment systems.

Reason/Benefit/Rationale: WHY: The guests should pay for their rooms.BENIFIT: Make the payments more convenient for hotel and guest.

Restrictions/Risks: The security is an issue. 


Sept 3 Absratction(work up)

According to the paper, I need to abstract or create new requirements depending on the original requirements. For instance, I create a
new requirement named Log, depending on requirement 'record'.

According to the Requirement's states in RAM, if the requirements that has been specified are accepted and in scope, they can be 
planned requirements. The next step is to prioritize the requirements. 

####2. MERTS

Question (1) "where do we want to go"

Factors          Weightings of factors       Requirement(Interface to external payment system )   Normalized

Market growth:   50			     80							  40

Market share:    25			     80							  20

Profit:          25			     50							  12.5


Question (2)"how to get there"

Factors                  Weightings of factors  Requirement(Interface to external payment system ) Normalized 

Customer segments:       40			American Paypal(60);Sweden PayEX(20);China Ali(20)	40			

Competitors:             30			American Opera system(80);China Ctrip system(20)        30

Differential advantage:  30			Price (80); Non-functional requirements(20)             30


Question (3)"what to do"

Factors			   Weightings of factors  Requirement(Interface to external payment system ) Normalized

Architecture stabillity:   50	                   70  							35

Customization flexibility: 50                      80							40

The total normalized points are 247.5. We can calculate other requirements according to the three questions, and compare the points of each requirements to prioritize the requirements. Additionally, we can presents more factors in the 'table' to get a detailed rating for each requirements.

Then I can decide the roadmap of this system according to the priority of requirements and estimate resource.

The last step is to answer why this roadmap(strategy) would be successful.

I think the excution in this report has proved the two technique is useful. The RAM can breakdown abstract requirements and the MERTS
make senses in prioritizing requirements.

##Lessons Learned:

1.The experience in requirement engineering is VERY important. No matter breakdown or prioritize requirements.

2.Not only the requirement itself, we need consider target market, target customer, competitors,etc. 

3.Customized requirements for different target market is a good choice.

4.If I want breakdown and prioritize requirements, I need more practise.

##Reflections:
1.When I have an idea, I take too much time to make it excutable. I think it is because I still do not master these two techniques, I am not familiar with them and not fully grasp these technologies.

2.The reason why I only presents four attributes of requirements in this report is that the proportion of these four attributes is
 much higher than other attributes. But maybe I can search a method to points them and check whether the rest attributes make sense.

