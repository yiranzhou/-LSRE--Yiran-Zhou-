Overview: Everyone has worked to some degree on the existing requirements. All have created some new issues, and linked existing issues. All have used the labeling feature, and assigned themselves to some requirements. Some appear to have randomly assigned themselves to requirements, and others have had a clear strategy to take care of a specific sub-area.

From your comments in your respective rplog.md I understand that at least some of you had a meeting in late December to discuss the release planning, and used the MoSCoW methodology to prioritise the requirements and assign them to milestones. The reason why I wanted you to do this on It's Learning is so that I can see evidence of it, and the amount of contribution each of you put in. As it stands, I don't know which of you participated in the meeting, how much each of you contributed to the end result, or even if you actually /had/ a meeting at all. I am therefore going to disregard the meeting and only look at the evidence of the meeting in terms of what each of you present in your rplog file. There, I am going to look for a description of the methodology you used, and the results thereof.

On the use of MoSCoW: Your choice of method to prioritise the requirements is ok (even if left unmotivated). But so far (I've read 2/3 of your assignments) none of you describe how the results of prioritising the requirements were actually used as a means to assign the requirements to different releases. For example, I would expect all "must" and "should" requirements to be taken care of in the early milestones, leaving "could" requirements to later releases. Why you've scheduled to implement "won't" requirements in release 0.5 and 0.8, I don't understand.

Another issue that you have not considered in your release plan is the available resources. Some of you are assigned to plenty of issues in one release and almost none in the next -- how do you plan on keeping all of you equally occupied for the duration of the development project?

Reflections on RP assignment (rplog.md): F
Assignment Strategy: Random Assignment
Methodology for Release Planning: Not Presented


Todo in order to Pass:
- Decide on a methodology for conducting release planning and describe it (with relevant references) (1 page)
- List and discuss at least three pros and three cons with the selected release planning method (1 page)
- Apply it on the requirements in the LSRE-ReleasePlanningProject repository. Describe what you do, and why. (5 pages)
- Describe your experiences from using the selected release planning method, and your experiences from using GitHub's issue tracker for working with requirements and release planning (1 page)


The art and science of release planning.
根据公式和参数算出每个feature的优先级。

To conducte release planning for the system in this course, I chose a method from the recomended paper of Seminars, which name is “The Art and Science of Software Release Plan”. The art of RP approach relies on human intuition, communication, and capabilities to negotiate between conflicting objectives and constraints. The science of RP approach formalizes the problem and applies computational algorithms to generate best solutions. The art of release planning addresses RP’s implicit and tacit aspects. The science of RP is primarily based on the belief that we can (at least approximately) formalize the problem, and that solving this formalized problem will produce meaningful results. I will conduct the releasing planning by this approach.  There are three functions in sicience of RP approach, 
x(i)=kr(i,t)Cap(k,t)                    (1),(2),(3). 
For feature realization, project managers typically must consider various resource constraints. Usually, these constraints relate to either budget or effort resources, and all constraints include bounds on the maximum capacities available for each resource type. The authors of this approach assume that T resource types and capacities Cap(k, t) relate to all releases k = 1 … K and to all resource types t = 1 … T. Every feature f(i) requires an amount r(i, t) of resources of type t. Thus, each release plan x assigning feature f(i) to release k expressed as x(i) = k must satisfy the function(1).


The planning objective is typically a mixture of different aspects such as value, urgency, risk, satisfaction or dissatisfaction, and return on investment. The explicit function’s actual form (equation 2) tries to bring together the different aspects in a balanced way. In our model, we assume the following:


■ An additive function exists in which the total objective function value isdetermined as the sum of the weighted average satisfaction WAS(i, k) of stakeholder priorities for all features f(i) when assigned to release k.
■ Each value WAS(i, k) is determined as the weighted average of the products of the two dimensions of prioritization described earlier. 
■ Stakeholder S(p)’s degree of impact is determined by the relative importance (p).
■ For each release option k, normalized parameters (k) describe each option’s relative importance. 
■ A vector of urgency preference for each stakeholder and each feature, given as urgency(p, i) = (urgency(p, i, 1), urgency(p, i, 2), urgency(p, i, 3)).


According to these assumptions,the objective is to maximize a function F(x) among all release plans x subject to the satisfaction of resource constraints (described in equation 1) and dependency constraints (just given).  


In this case, we need assign a relative importance of 拉姆达(p) of stakeholder， project manager 还要identify 每个版本的相对重要性。 stakeholders 决定每个feature的价值（1-9），并且voting for urgency for each feature。


Pros：


Amarriage of art and science, such as the one we have proposed, promises to carry RP’s state of the practice to a higher level, giving due consideration to 
■ recognizing the need for a more sophisticated methodology, 
■ introducing more formalism that lets organizations easily plan projects containing several hundred features, 
■ formulating RP objectives with several impacting criteria rather than concentrating only on the values of the features, 
■ letting human decision makers easily evaluate formally generated release plans so they don’t have to deal with lots of information without much visibility into the problem’s structure, and 
■ proactively evaluating possible planning strategies to better understand the impact of varying problem parameters.






Cons ：
三个优点：1.根据公司收集到的数据，可以很快地算出现有的resource和。2.计算结果非常直观，方便制定release plan。3. 如果有很多的dependence的话，可以在计算结果之后，根据dependence调整release plan，非常方便。
三个缺点：1.非常依赖stakeholder的经验。2. project manager在这个方法中拥有很大的权力，需要决定每一个release的相对重要性，stakeholder的重要性。经理的经验，决策能力，领导能力非常重要。3.对于每个stakeholder的重要性的界定也是人为的，没有相关的资料说明。


Process of applying the approach


In this case, there are 120 feartures.
F={f(1),f(2),...,f(120)}.


In this case, there are 6 releases.
x(i)={x(0.1),x(0.5),x(0.8),x(0.9),x(1.0),x(2.0)}


文章中说，需要project manager来定义每个版本的相对重要性，因为这个项目没有明确的team。所有我假设每个版本的相对重要性分别是
x(0.1)=0.3
x(0.5)=0.2
x(0.8)=0.2
x(0.9)=0.1
x(1.0)=0.2
x(2.0)=0.2
我认为第一个版本很重要，版本0.9在0.8和1.0中间，更新时间相对来说比较近，所以应该不会有大的更新，相对重要性最低。
接下来考虑resource，要满足equation （1）。在这个项目中，没有关于开发团队的任何材料，对于每个feature所需要的资源的评估也没有。 所有我决定，在这个项目中，默认符合equation（1），即资源满足任何release planning，版本迭代和每个版本delivery的feature不受资源限制。
在文章中没有明确提出stakeholder的相对重要性由谁来定义，直说了“we can assign”。在我搜索了很多论文数据库之后，也没有找到相应的办法来定义stakeholder的相对重要性。在我看来，我认为这需要project manager来决定，或者引入expert来决定每一个case中的stakeholder的相对重要性。由【1】stakeholder的表格，并且基于这个项目的性质和我本人的能力所限，我选择了三个stakeholder来conducting 这个approach，development team, users, acquires. 剩余的那些stakeholder要么是这个项目不涉及，要么是不需要。需要说明的是，以我自己为例，由我独立开发的话，那么developer，tester，maintainers，product engineer都是我一个人, 所以我是作为development team的stakeholder。 除此之外，我请了一个同学作为user的代表的stakeholder， and another friend as acquires。 他们都是我们学校软件在读的学生。我定义了这三个stakeholder的相对重要性，分别是
拉姆达（acquire）=
拉姆达（development）=
拉姆达（user）=


接下来，就是根据equation（2）和（3）计算每一个feature的objective function value for each release。


得出结果之后，考虑feature 之间的dependence。然后得出最终的release planning。




Stakeholer(Acuire):value=(1,1)=a, 




| - | Stakeholder S(1) | Stakeholder S(2) | Stakeholder S(3) |
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
 

