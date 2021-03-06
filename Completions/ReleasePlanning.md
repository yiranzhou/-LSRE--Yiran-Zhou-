To conduct release planning for the system in this course, I chose a method from the recommended paper of Seminars, whose name is “The Art and Science of Software Release Plan”. The art of RP approach relies on human intuition, communication, and capabilities to negotiate between conflicting objectives and constraints. The science of RP approach formalizes the problem and applies computational algorithms to generate best solutions. The art of release planning addresses RP’s implicit and tacit aspects. The science of RP is primarily based on the belief that we can (at least approximately) formalize the problem, and that solving this formalized problem will produce meaningful results. I will conduct the releasing planning by this approach.  
There are three functions in the science of RP approach. For feature realization, project managers typically must consider various resource constraints. Usually, these constraints relate to either budget or effort resources, and all constraints include bounds on the maximum capacities available for each resource type. The authors of this approach assume that T resource types and capacities Cap(k, t) relate to all releases k = 1 … K and to all resource types t = 1 … T. Every feature f(i) requires an amount r(i, t) of resources of type t. Thus, each release plan x assigning feature f(i) to release k expressed as x(i) = k must satisfy the function(1)--(Sum r(i,t))<= Cap(k,t).

The planning objective is typically a mixture of different aspects such as value, urgency, risk, satisfaction or dissatisfaction, and return on investment. The explicit function’s actual form (equation 2) tries to bring together the different aspects in a balanced way. In the model of the paper provided, the authors assume the following:

- An additive function exists in which the total objective function value is determined as the sum of the weighted average satisfaction WAS(i, k) of stakeholder priorities for all features f(i) when assigned to release k.
- Each value WAS(i, k) is determined as the weighted average of the products of the two dimensions of prioritization described earlier. 
- Stakeholder S(p)’s degree of impact is determined by the relative importance (p).
- For each release option k, normalized parameters (k) describe each option’s relative importance. 
- A vector of urgency preference for each stakeholder and each feature, given as urgency(p, i) = (urgency(p, i, 1), urgency(p, i, 2), urgency(p, i, 3)).

According to these assumptions, the objective is to maximize a function F(x) among all release plans x subject to the satisfaction of resource constraints (described in equation 1) and dependency constraints (just given).

![fomula](https://lh3.googleusercontent.com/-K3SXWhkVbiY/WKG5PjxRryI/AAAAAAAAAIc/gXwj8PoJ82kOwJZ8itTZ7mNddSyE5MvnwCJoC/w287-h122-p-rw/1486993699%25281%2529.png)

In this case, we need assign a relative importance of λ(p) of stakeholder， project manager need to identify the relative importance of each version.  And stakeholders need to decide value(1-9) of each feature and vote for urgency for each feature

## Pros and Cons
Pros：
- A marriage of art and science as proposed above promises to carry release planning’s state of the practice to a higher level;
- This approach gives due consideration to recognize the need for a more sophisticated methodology;
- This approach introduces more formalism that lets organizations easily plan projects containing several hundred features;
- This approach formulates release planning objectives with several impacting criteria rather than concentrating only on the values of the features
- This approach also lets human decision makers easily evaluate formally generated release plans so they don’t have to deal with lots of information without much visibility into the problem’s structure, and proactively evaluate possible planning strategies to better understand the impact of varying problem parameters.

Cons:

- This approach really relies on the experience of stakeholders, since the stakeholders need to identify the value of each requirement and expected release version.
- There is no explanation and method to identify the relative importance of each release version and only project manager in charge of this decision. 
- The relative importance of each stakeholder is decided by authors without references. And the paper does not propose how the relative importance of each stakeholder are identified.

## Process of applying the approach

#### Number of Features
In this case, there are 104 features.
F={f(1),f(2),...,f(104)}.

#### Release Version
In this case, there are 6 releases.
x(i)={x(0.1),x(0.5),x(0.8),x(0.9),x(1.0),x(2.0)}

According to the paper, the relative importance of each relese version are defined by project manager, while there is not a clearly project manager. So I identified the relative importance of each release version:
- x(0.1)=0.3
- x(0.5)=0.2
- x(0.8)=0.2
- x(0.9)=0.1
- x(1.0)=0.2
- x(2.0)=0.2

The reasons are proposed as follows:

I think the first version is the most important. Version 0.9 is between Version 0.8 and Version 1.0, and there should not be a lot of updates, so the relative importance should be the lowest. Considering the resource, there is no documentation on the development team, and there is no assessment of the resources needed for each feature. So I assume that the resource satisfies any release planning, version iteration, and each version delivery feature is not subject to resource limitations. 

#### Importance of Stakeholders
There is no clear definition of the relative importance of stakeholders. The authors wrote “we can assign” in the paper. I searched a lot of databases, but I did not find any method to identify the relative importance of stakeholders. In my opinion, the importance of each stakeholder may be different in different projects. The project managers or experts may identify the relative importance of stakeholders in this approach. Based on the types of stakeholders in software engineering[1] and according to the limitation of my ability, I chose three type stakeholders to conduct the project, and they are development team, users, acquires. The rest of other stakeholders are either not involved in this project, or are not required.It should be noted that developer, tester, maintainers, product engineer are identified as one stakeholder called development team in this project. In addition, I invited a classmate as the representative of the user's stakeholder, and another friend as acquires. They are both software engineering students studying in BTH. I defined the relative importance of the three stakeholders:
- λ(acquire)= 5
- λ(development team)= 5
- λ(user)= 9

For each stakeholder, they need to identify the value of each feature and the urgency to each version.

| - | Stakeholder S(1 auquire) | Stakeholder S(2 development) | Stakeholder S(3 user) |
| :-------------: | :-------------: | :-------------: |:-------------: |
|Feature(1)| value(1,1)=8; urgency(9,0,0,0,0,0)|value(2,1)=9; urgency(9,0,0,0,0,0)| value(3,1)=6; urgency(7,2,0,0,0,0)|
|Feature(2)| value(1,2)=1; urgency(0,0,0,0,2,7)|value(2,2)=2; urgency(0,0,0,2,7,0)| value(3,2)=5; urgency(0,0,2,3,4,0)|
|Feature(3)| value(1,3)=7; urgency(8,1,0,0,0,0)|value(2,3)=8; urgency(7,2,0,0,0,0)| value(3,3)=5; urgency(2,2,2,2,1,1)|
|Feature(4)| value(1,4)=8; urgency(9,0,0,0,0,0)|value(2,4)=9; urgency(9,0,0,0,0,0)| value(3,4)=9; urgency(8,1,0,0,0,0)|
|Feature(5)| value(1,5)=7; urgency(6,3,0,0,0,0)|value(2,5)=9; urgency(7,1,1,0,0,0)| value(3,5)=8; urgency(8,1,0,0,0,0)|
|Feature(6)| value(1,6)=9; urgency(7,2,0,0,0,0)|value(2,6)=6; urgency(0,0,0,3,3,3)| value(3,6)=5; urgency(1,2,2,2,2,2)|
|Feature(7)| value(1,7)=9; urgency(9,0,0,0,0,0)|value(2,7)=9; urgency(0,0,7,2,0,0)| value(3,7)=9; urgency(8,1,0,0,0,0)|
|Feature(8)| value(1,8)=9; urgency(9,0,0,0,0,0)|value(2,8)=9; urgency(9,0,0,0,0,0)| value(3,8)=9; urgency(9,0,0,0,0,0)|
|Feature(9)| value(1,9)=7; urgency(9,0,0,0,0,0)|value(2,9)=9; urgency(7,1,1,0,0,0)| value(3,9)=8; urgency(8,1,0,0,0,0)|
|Feature(10)| value(1,10)=7; urgency(6,3,0,0,0,0)|value(2,10)=9; urgency(7,1,1,0,0,0)| value(3,10)=9; urgency(9,0,0,0,0,0)|
|Feature(11)| value(1,11)=3; urgency(0,0,0,5,4,0)|value(2,11)=5; urgency(0,1,1,3,4,0)| value(3,11)=5; urgency(0,5,4,0,0,0)|
|Feature(12)| value(1,12)=7; urgency(9,0,0,0,0,0)|value(2,12)=9; urgency(9,0,0,0,0,0)| value(3,12)=9; urgency(9,0,0,0,0,0)|
|Feature(13)| value(1,13)=6; urgency(3,5,1,0,0,0)|value(2,13)=4; urgency(0,0,5,4,0,0)| value(3,13)=9; urgency(7,2,0,0,0,0)|
|Feature(14)| value(1,14)=7; urgency(6,3,0,0,0,0)|value(2,14)=5; urgency(0,8,1,0,0,0)| value(3,14)=9; urgency(4,5,0,0,0,0)|
|Feature(15)| value(1,15)=9; urgency(9,0,0,0,0,0)|value(2,15)=9; urgency(7,1,1,0,0,0)| value(3,15)=9; urgency(9,0,0,0,0,0)|
|Feature(16)| value(1,16)=7; urgency(0,0,0,4,5,0)|value(2,16)=6; urgency(0,0,0,0,7,2)| value(3,16)=5; urgency(0,0,0,3,3,3)|
|Feature(17)| value(1,17)=9; urgency(9,0,0,0,0,0)|value(2,17)=9; urgency(9,0,0,0,0,0)| value(3,17)=9; urgency(9,0,0,0,0,0)|
|Feature(18)| value(1,18)=9; urgency(9,0,0,0,0,0)|value(2,18)=9; urgency(9,0,0,0,0,0)| value(3,18)=9; urgency(9,0,0,0,0,0)|
|Feature(19)| value(1,19)=7; urgency(0,8,1,0,0,0)|value(2,19)=3; urgency(0,0,0,3,3,3)| value(3,19)=9; urgency(7,2,0,0,0,0)|
|Feature(20)| value(1,20)=7; urgency(6,3,0,0,0,0)|value(2,20)=9; urgency(3,3,3,0,0,0)| value(3,20)=9; urgency(9,0,0,0,0,0)|
|...| ...|...| ...|
|Feature(104)| value(1,120)=5; urgency(3,6,0,0,0,0)|value(2,104)=6; urgency(0,4,5,0,0,0)| value(3,104)=3; urgency(1,4,4,0,0,0)|

The complete tables and calculated results are present in google form. According to the equation (2) and (3), the results of these are present in https://drive.google.com/file/d/0B-ZzbIX8Zcznc3p2OEtLb2FuejA/view?usp=sharing.

For example,feature 1=0.1 * (5 * 8 * 9 + 5 * 9 * 9 + 9 * 6 * 7)=342.9


## Experiences from using the selected release planning method, and using GitHub's issue tracker for working with requirements and release planning

The selected release planning method is easy to conduct, but the identification of each requirement is very large. Because the amount of data is very large and the law is limited, Excel needs to introduce Visual Basic programming to calculate. My computer does not have Visual Basic programming software, and I am not familiar with the Visual Basic programming, so I used Excel with a simple calculation function which leads that I spent a lot of time on calculating. And when I identify the value and urgency of each requirement, I have considered the relationship between each requirement. For example, the basic features are considered to release in earlier versions and similar features are considered to release in the same version.

The issue tracker is easy to use. It provides relatively complete version control tool, such as milestone. And the teammates could discuss the proposed requirements. Furthermore, it can create and apply labels to issues to assign to users or categorize. We also could prioritize the requirements. By the way, I think the issue tracker is more useful for a team rather than the individuals. And I notice that it can be not only used for requirements but also be used to propose for other 'code issue'.       
