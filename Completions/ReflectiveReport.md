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

It is critical for product management to select the requirements aligned with the overall business goals and discard others as early as possible. Due to the emergence of markets for off-the-shelf or packaged software, the result is a large amount and continuous flow of requirements that threaten to overload the development organization. MERT could combine the strategic and technical perspectives to formulate product strategies that are good-enough. MERTS takes strategic and technical views into account, so that it can acts as a stepwise guide to creating product strategies. The strategies resulting from MERTS can be used by managers to perform requirements triage for early requirements triage and selection. These two papers help define excutable requirements, which is useful and practical in software development process. And based on each saminer,  I think the techniques provided by these papers are easy to understand and implement, though there are some defects in them.


##Implementation Plan:

1. Based on the prerequisites of the proposed methods, and the limitation of my research, the implementation plan focus on the scoping of the tested project firstly. The project should be market-driven and available for one master student research.
2. Selecting a project as the experimental material to apply the methods which are proposed in selecting papers is the next step.
3. Using the method from ‘A Method for Early Requirements Triage and selection Utilizing Product Strategies’ to calculate the points of each requirement.
4. Using the method from ‘Requirements Abstraction Model’ to break down the requirements from the tested project.

##Excution:

1.	Scoping the tested project
As the description in‘Method for Early Requirements Triage and Selection Utilizing Product Strategies, ‘the market-driven product development has large numbers of requirements threaten to overload the development organization. ’And in the explanation in ‘Requirements Abstraction Model’，‘software requirements arrive in different shapes and forms to development organizations. This is particularly the case in market-driven requirements engineering, where the requirements are on products rather than directed towards projects.’The tested project should be a market-driven project. And the limitation of human resources and time lead to the project size should be suitable for a master student research.
2.	Selecting the tested project
A project has been chosen, which is a windows application, named Hotel Management System, the target customers are hotels. The system should include management sub-system and back office sub-system. 
3.	Break down the requirements 
I have presented some basic requirement of Hotel Management System. Parts of them have been break down, according to 'Requirement Absreaction Model'. Additionally, most requirements are from my own experience and some are from network.
4.	Calculating the points of each requirement
According to the case of first technique, there is one requirement named payment, it is a good instance for this technique. Based on the paper, 'A method ', I will resent a table to presents the excution of this technique. Due to this is a report on Github, the table is translated into plaintext.


##Proof of Concept:

In this section, I proposed a hotel management system, which include all most basic function for managing a hotel. Fisrtly, I use RAM model to break down these original requirements. Then I use MERTS to prioritize these requirements. It should be noted that due to the limitation of my ability, the original requirements are not so 'large scale', but the final requirements are 'large scale'. What's moere, I can use the existing process of breaking requirements to speculate the process of applying these methods in large scale requirement engineering. The fact is that the amount of requirements is almost geometrically growing when applying the RAM model to the original requirements. 

####1.Technique from Requirements Abstraction Model to break down requirements.

The RAM model allows for placement of requirements on different levels and supports abstraction or break down of requirements to make them comparable to each other. As the sources of the requirements vary and the equirements themselves are both direct and indirect in ature it is not surprising that they come in different hapes and forms, at multiple levels of abstraction, and escribed on varying levels of refinement. RAM is modeled towards a product perspective, supporting a continuous requirement engineering effort, aimed at taking requirements of multiple types (abstraction level) as input, and offers a structure for the work-up of these requirements. Through work with RAM, requirements on a high level of abstraction (comparable to product strategy) and a low level of abstraction (good enough as input to a project) are available. In addition, as several levels of abstraction are offered, a richer understanding can be obtained as to the purpose of a requirement, its origin and so on, by looking at requirements over the abstraction level boundaries.The work-up process involves creating new requirements (called work-up requirements hereafter) on adjacent abstraction levels or linking to already existing ones, depending on the situation. Besides, there are another 10 attributes, such as Requirement Source, Requirement Owner, Requirements Manager and so forth.

To apply the RAM method, firstly I proposed some basic requirements and specified them in Step 1. The original requirements are not so many, but as the process of applying the RAM, there will be large scale requirements. Secondly, I placed them in Product Level, Feature Level, Function Level and Component Level in Step 2. Then, the requirements will be broken down in Step 3. The Step 2 and 3 are 

Step 1 Specify

The first step (Specify) involves specifying the initial requirement and eliciting enough information about it to specify a number of attributes. At first step, I present three attributes: Description, Reason/Benefit/Rationale, and Restrictions/Risks to specify the original requirements.

| ----- | Description | Reason/Benefit/Rationale| Restrictions/Risks |
| :-------------: | :-------------: | :-------------: |:-------------: |
|Booking |The system should be able to input and modify booking information | WHY: The user want to input and modify booking information.BENEFIT: the user can use this system to book for guests. |The length and type of input text should be restricted.|
|Check-in | The system should be able to input and modify check-in information |WHY: The user want to input and modify check-in information.BENEFIT: the user can use this system to check in for guests|The length and type of input text should be restricted. The system should be used to confirm the identity information of the user is legitimate|
|Payment | The system should provide interfaces to kinds of external payment systems and record the payment information |WHY: The guests need to pay for their rooms by using different credit cards and cash, and the hotel need payment information for daily management. BENIFIT: Make the usage of the system more attrctive |The security of information is an issue |
|Reception management |The system should be able to check, modify guest information, room information, and set room information|WHY: Guests sometimes may change their schedule and the rooms may need renovate. BENIFIT: Make the system more flexible.|This may conflict with booking and check in if not promptly update.|
|Back Office management |The system should be able to manage the privilege of the system and modify the state of rooms|WHY: The system are only used by reception staff of a hotel. BENEFIT: Ensure the the security of the guest information and hotel information.|The security of system is an issue.|
|Record |All the information and operation information should be record.|WHY: The managers of hotel or other people may need the information. BENIFIT: If there is an accident, the system can provide some evidence.|Customer information and hotel information may be stolen.|
|Log in|Only the relevant staff can log in to operate the system.|WHY: The system should be relatively closed, so that other unrelated personnel can not use the system. BENEFIT: others can not use this system to modify any information.| The security of information is an issue|
|System management|The system managment should include user management and login system.|WHY: The system should be able to let user change password and manage the users of the system. BENEFIT: the system could manage the privilege of the system.| The security of information is an issue.|
|Check-out |The system should be able to check out for guests.|WHY: The user want to check out for guest. BENIFIT: the user can use this system to check out for guests.|Only the user has privilege can check out for guests.|

Step 2 Place

The second step (Place) is centered around what abstraction level the now specified requirements resides on and last (Abstraction) each requirement goes through a work-up.  At second step, RAM consists of a number of abstraction levels (the driving motor of the model). This step involves analyzing what level a requirement is on and placing it on this level. The four abstraction levels are Product level(goal),Feature level(features), Function level(functions/actions) and Component level(details- consists of)
According to Step 1, these requirements are placed in following abstract level.
![step 2](https://docs.google.com/drawings/d/1fUCLekKpVTpLxKQ8X0vBc1RUP3fhyzhqUZEqgkAqAL8/pub?w=454&h=351)

Step 3 Break Down Requirements

The third step of RAM involves abstracting and/or breakdown of a requirement, depending on the initial placement of the original requirement. The work-up process involves creating new requirements (called work-up requirements hereafter) on adjacent abstraction levels or linking to already existing ones, depending on the situation. Besides, there are another 10 attributes, such as Requirement Source, Requirement Owner, Requirements Manager and so forth. The requirements on Feature Level and Product Level should be broken down. The requirements belong to Function Level can be broken down. 

![step 3-1](https://lh3.googleusercontent.com/-Lhz8c25RqoA/WK9BrVnp7VI/AAAAAAAAAMY/SCwtsIBOIfI54xsGWGk9qwz6jukHtCnTgCJoC/w530-h501-p-rw/Step%2B3-1.png)

| ----- | Description | Reason/Benefit/Rationale| Restrictions/Risks |
| :-------------: | :-------------: | :-------------: |:-------------: |
|Query room state|The system should be able to query room state.| WHY: The user want to check the state of room when new guests come. BENIFIT: the user can check in for new guests according to the result of query.|The state does not get update timely.|
|Set room state|The system should be able to set room state.|WHY: The user want to set the state of room when the room is taken or need renovate. BENIFIT: the user can set the state of room when necessary.|Only user who has the privilege can set room state.|
|Supplement guest information|The system should be able to supplement guest information.| WHY: In some situation, the user may need to supplement guest information. BENIFIT: the user can record complete and correct information of guests.|Only user who has the privilege can set room state. Supplementary information should be identified.|
|Record payment information|The system should be able to record payment information.|WHY: the hotel need payment data to complete financial statements. BENIFIT: Make the management of financial more convenient.|The security is an issue.|
|Interface to external payment system|The system should provide different interfaces for different external payment systems.|WHY: The guests should pay for their rooms.BENIFIT: Make the payments more convenient for hotel and guest.|The security is an issue.|
|Booking for members|The system should be able to have a booking for the member customer.|WHY: The user want to deal with the reservation case of customer member. BENEFIT: The user can process the customer member booking.| The booking is only for members|
|Booking for guests|The system should be able to have a booking for guests.|WHY: The user want to deal with the reservation case of guests. BENEFIT: The user can process the booking from the guest customers. |The booking is normal guests, but not for members|
|Booking for individual|The system should be able to have a reservation for the individual customer.|WHY: The user want to deal with the individual reservation case. BENEFIT: The user can process the booking of individual reservation case.|The booking is for individual who could be members or normal guests.|
|Booking for group|The system should be able to have a reservation for the group booking.|WHY: The user want to deal with the group reservation case. BENEFIT: The user can process the booking of group reservation case.|The booking is for group.|
|Record payment information|The system should be able to check the payment record|WHY: The user want to  check the record of payment information for financial management. BENEFIT:The user can check the payment record.|The Payment-related functions should have a very high security.|
|Interface to external payment system|The system should be able to allow using the external payment system.|WHY:The user want to allow the customers to pay by external payment system. BENEFIT:The customers can use external payment system.|The Payment-related functions should have a very high security.|
|System user management|The system should be able to manage the users.|WHY: The user want to manage the users who have restriction to use this system. BENEFIT:The user can manage the users who use the system.|Only privilege user could use user managemnet.|
|Hotel room management|The system should be able to manage the information of the rooms.|WHY:The user want to manage the state of rooms. BENEFIT:The user can manage the hotel room by the system.|The system is related to Booking, Check-out, Check-in.|
|Check-in online|The system should be able to deal with the check-in online.|WHY:The user want to the customers can check-in online by the system.  BENEFIT:The customers can use the system check-in online.| This function do not need authority of the main system. It connect to a external machine that customer could use to check in |
|Check-in hotel|The system should be able to deal with the check-in in reception.|WHY:The user want to the customers can check-in in the hotel reception by the system. BENEFIT: The customers can check-in in the hotel reception by the system.|Only reception staff could use this function|
|Check-out in hotel|The system should be able to deal with the check-out in reception.|WHY:The user want to the customers can check-out in the hotel reception by the system. BENEFIT:The customers can check-out in the hotel reception by the system.|Only reception staff could use this function|
|Self-check-out|The system should be able to deal with the self-check-out.|WHY:The user want to the customers can self-check-out by the system. BENEFIT:The customers can check-out by themselves by the system.|This function do not need authority of the main system. It connect to a external machine that customer could use to check out.|

##Merts
According to the literature study an initial draft of MERTS was created and elicited information from industry The input 
from the previous literature study and industry interviews was subsequently used for the creation of a final version of MERTS. Initial 
industry validation is presented and a discussion of lessons learned highlighting initial feedback is presented. 

- Step 1.Specify. Answer the three strategic questions ((1)Where we want to go?, (2) How to get there?, (3) What will be done?) for each product.
- Step 2.Assign Weights. The answers from Step 1 are assigned weights. The answers of each question have a total weight of 100 (Table 1) and the total weight of the three questions is 300.
- Step 3.Compare Requirements. There is an instance that shows the weights of same requirement are different in different market.

The explanation of the three questions in Step 1 as follows:

1. “where do we want to go”-finding out the right balance between the long term opportunities or goals and short term objectives. Goals are profit, growth, and market share.

2. “how will we get there”-The choice of customer targets depends on the nature of the goals and objectives selected when answering “where an organization wants to go”.

3. “what to do”-For determining a product’s position in the market it has to be differentiated based on either cost price or value of product offering. This means that the product has to be either low priced backed by low costs or better than competitors’products as seen by customer.

The first three steps of MERTS should be performed at product management level supporting the triage of requirements (aiding in the selection). According to the applying process of RAM, there are three requirements belong to Product Level, which are reception management, Back office management, Systmen management. 

The answers from Step 1 are assigned weights. The answers of each question have a total weight of 100.and the total weight of the three questions is 300. The rule is to assign weights to each of the factors based on their relative importance in a way that total weight remains 100. This way has been reported to be one of easiest and quickest prioritization methods.

Step 1 Specify

| Questions | Factors | Weight of factors|Sub classification|Sub classifications Weightings| Normalized Weightings| 
| :--------: | :--------: | :--------: | :--------: | :---------: |:---------: |:---------: |:---------: |
|Where|Market growth|50|||50|
||Market share|25|||25|
||Profit|25|||25|
|How|Customer segments|50|USA market|30|15|
||||EU market|30|15|
||||Asia market|40|20|
||Competitors|30|Company A|50|15|
||||Company B|30|9|
||||Others|20|6|
||Differential advantage|20|New Functions|60|12|
||||Princing|20|4|
||||Non functional requirements|20|4|


##Lessons Learned:

1. When the original requirements are proposed, they are usually belong to Product Level or Feature Level, which means that almost of them could be brokendown. Although some requirements are belong to Function Level, they can still be broken down. What's more, the proposed original requirements could be the sub-requirements of other original requirements. 

2. The break down process of RAM model is complicated so that the workload is huge, especially for large scale requirement engineering. I think that it is better to develop a system or a software step by step, not in large scale for individual. For big company, it is also better to split a large-scale project into small-scale project.

3. When I applying the MERTS, I also realized that the 'large scale' means huge workload. The MERTS require to identify kinds of weights for each requirement, 

##Reflections:
1.When I have an idea, I take too much time to make it excutable. I think it is because I still do not master these two techniques, I am not familiar with them and not fully grasp these technologies.

2.The reason why I only presents four attributes of requirements in this report is that the proportion of these four attributes is
 much higher than other attributes. But maybe I can search a method to points them and check whether the rest attributes make sense.
