# Seminar 0
###Qeustions
####• What is large scale requirements engineering?

Requirement engineering is the process of defining, documenting and maintaining requirements to the sub-fields of systems engineering and software engineering concerned with this process. Large scale means about 1000 orders of magnitude requirements.The requirements Managing a complete set of interdependencies is practically unfeasible, but feasible among small bundles of requirements[1]. 

####• What are the challenges in large scale requirements engineering?

A key challenge in construction of these support tools is how to scale them to handle a large volume of information. Particularly crucial are the ways in which large numbers of requirements and their interrelationships are presented to users[2].
When large organizations develop systems for large markets, the size and complexity of the work products of requirements engineering impose critical challenges[5]. And accoring to the summary of [5], the following are the challenges in large scale reuqirements engineering:
- Satisfy all project stakeholders vs. producing a balanced scope. 
- Scope reductions are difficult. 
- Wasting effort on de-scoped features. 
- Hard to get an overview or see the “big picture”.
- Requires deep knowledge of people and system.
- Acquire enough knowledge to be able to make the decision.
- Difficult to avoid late scoping decisions.
- Hard to satisfy all needs. 
- Unclear req.
- Too complicated to understand.
- Uncontrolled changes.
- Information cannot be trusted.
- Too complicated to understand.
- Unable to reuse the req.
- Unclear req.
- Difficult to make relevant grouping. 

####• What is the order of magnitude of the number of requirements we are discussing?

According to the B.Renell,  They defines orders of magnitude in RE based on the size of the set of requirements
that are managed by an organisation that develops software-intensive systems. The 1000 order of magnitude of the number of requirements are large scale. The 100 order of magnitude is medium scale requirements and the 10000 order of magnitude is very large scale reuiqrements engineering[1].

####• Read up on and summarise [Strategic] Release Planning

Release planning is a process applying various types of upstream decision-making that combine market considerations with implementation concerns. Release planning involves aspects such as selecting what features and requirements should be in a certain
release, when it should be released, and at what cost[3].

Release planning, the process of deciding which features and quality level should be included in which release [3], which is both a cognitively and computationally difficult problem, is classified as a wicked problem since different kinds of uncertainty make it difficult to formulate and solve the problem. Moreover, the objective of release planning is to ’maximize the benefit’; however, the difficulty lies in how to give a measurable definition of ’benefit’[4].

###Articles
####•The Art and Science of Software Release Planning

-The art of RP approach relies on human intuition, communication, and capabilities to negotiate between conflicting objectives and constraints. The science of RP approach formalizes the problem and applies computational algorithms to generate best solutions. The art of release planning addresses RP’s implicit and tacit aspects. The science of RP is primarily based on the belief that we can (at least approximately) formalize the problem, and that solving this formalized problem will produce meaningful results. 

-Resease planning is ad hoc and rarely based on sound models and methodologies. It is hard to select and scheule features. Planning and follow-up replanning leads many extra activities. Another problem is that the planning scope is often limited to just the next release. Even though there are guidelines exist for release plan in princple, they don't tell us how to operate.

-This approach formulates a series of problems, like Desicion variables, dependencies between feature, resource constraints, stakeholders, feature prioritization, objective function, as variants of the original formal model. This paper provides a hybrid approach based on integer linear programming.The solution algorithms the authors have adopted are based on solving a sequence of linear programming problems without integer conditions. Their approach formulates a series of problems as variants of the original formal model. In this way, art and science complement each other. Based on the art-based method to deal with the complexity of the number of factors that increase the difficulties and problems RP. Science-based method to deal with the complexity of the better, but you can not use the same analysis capabilities as human problems policymakers assessment.The authors improve their approach to perform a variety of tasks, modeling, exploration, and consolidation. After formalizing the problem, the decision maker can perform what-if scenarios and can base replanning on the results.

-The formulation:

- features F = {f(1), f(2), …, f(n)}.
- decision variables {x(1), x(2), …, x(n)}, where x(i) = k if we assign requirement i to release option k ∈{1, 2, … K}; otherwise, x(i) = 0.
- two types of dependency constraints: a coupling relation called C and a precedence relation called P
- T resource types and capacities Cap(k, t) relate to all releases k = 1 … K and to all resource types t = 1 … T. Every feature f(i) requires an amount r(i, t) of resources of type t. Thus, each release plan x assigning feature f(i) to release k expressed as x(i) = k must satisfy ∑x(i)=k r(i, t) <= Cap(k, t) (1) for all releases k and resource types t.
- a set of stakeholder S = {S(1), …, S(q)}
- a relative importance of λ(p)∈{1, …, 9} to each stakeholder p For the value proposition, each stakeholder is asked to assign an ordinal value, value(p, i) ∈ {1, 2, …, 9}, to each feature based on its assumed (relative) impact on the product’s overall value. So, value(p, i) = 1 and value(p, i) = 9 represent the lowest and highest values, respectively. Each stakeholder has nine votes for each feature,which we’ll distribute among three possible options: assign to release 1, assign to release 2, or postpone. An urgency vote urgency(p, i) = (9, 0, 0) indicates that stakeholder S(p) has assigned the highest possible urgency to feature f(i) and thus wants to include it in the first release.
- An additive function exists in which the total objective function value is determined as the sum of the weighted average satisfaction WAS(i, k) of stakeholder priorities for all features f(i) when assigned to release k.
- function F(x) among all release plans x subject to the satisfaction of resource constraints (described in equation 1) and dependency constraints (just given). F(x) is given as F(x) = ∑k = 1…K ∑i: x(i) = k WAS(i, k) (2). WAS(i,k) = ζ(k)[∑p=1…q λ(p)·value(p,i)·urgency(p, i, k)] (3)

-This paper propovide a sophisticated methodology let the organization easily plan the release plans and consider the impact of varying problem parameters.

####•Introducing Support for Release Planning of Quality Requirements -An Industrial Evaluation of the QUPER Model

-QUPER model is developed for supporting release planning and roadmapping of quality requirements.This paper presents one case of QUPER tailoring, implementation, and most important evaluation, conducted at Sony Ericsson. The QUPER model was developed in three main steps: 1. Problem definition help understand different requirement decision scenarios; 2.Model definition based on first step and including a benefit view, a cost view, a roadmap view, and the concepts of benefit breakpoints and cost barriers; 3. Experts are ivolved in Model validation. And we can observe that quality is continuous and non-linear from these views.

-The authors tailored the QUPER model and define 4 steps as following 1. Define quality aspects. 2. Estimate your product’s current quality (for a given release) and the competing products’ quality (at present or envisioned). 3. For each quality aspect and for each relevant qualifier, estimate the breakpoints. 4. Estimate candidate targets and discuss and decide on actual targets for coming releases. They involved in improving the practice of release planning of quality requirements by introducing the QUPER model. There are three steps, Interview, Workshop and Interview again. In Interviews, they collected and analyzed data. In Workshop, they applied QUPER in real projects. Besides, they took some meastures to increase validity. 

-QUPER works well in the four areas, Network access, Email, Video systems and Positioning. But there are still some challenges, like Difficult to identify differentiation and saturation breakpoints in Network access area, people may interpret the breakpoints differently in Email area, people spend too much time on applying QUPER and so forth. Other challenges were how to specify
performance requirements that are quantifiable, representative of the “real world”, and under what conditions they should be fulfilled and specification of performance requirements. And during the interviews, one more challengs are proposed which is difficulties to identify the values of the differentiation and saturation breakpoints.

-I learnd a lot from this artcle. First is the real platform development process from Sony Ericsson. It comprises the roadmap extraction, selection of features on the roadmap, definition of initial scope, prioritizition and project priority for the platform project. Second, I understand some concepts deeper like QUPER, PR(performance requirement), competitor analysis and so on. Third, each model and method may works well in somw aspects, we still need understand these model or method may lead some challenges. We should analyze if it worth to apply them. 

####•A Case Study Evaluation of the Guideline-Supported QUPER Model for Elicitation of Quality Requirements

-it is important to plan the product’s releases so that they can reach the market as early as possible with a competitive level of quality compared to its competitors’ products, but the core question is that when is the quality level good enough? There are only two strategic release planning methods address quality constraints: The quantitative Win-Win model [28] addresses effort and time constraints, but not the quality level of QR, while the only method to address quality and cost constraints of QR is the QUPER model. This paper provides practical guidelines of how to apply QUPER in practice, adds step of how to incorporate cost dependencies between QR and evaluates the complete version of the QUPER model.

-Guidelines:1.Identify candidate QR(Once feature has been identified, the consequences for the particular QR should be consider)；2. Define scale and unit(e.g. 'time' is scale, 'minutes' is unit).3.Identify reference levels(Reference levels can be based on competing
as well as own products (Qref));4.Elicit quality breakpoints(the market expectations should be defined in terms of the values of quality breakpoints)；5.Estimate cost barriers(identify and estimate several cost barriers for each QR);6.Set candidate requirements(One way to specify a requirements quality interval is by using both a Good and a Stretch target);7.Identify cost dependencies(If cost dependencies among QR are considered important to identify for cost estimations, then, for each top-n QR, identify which modules (architectural components/parts) that needs to be changed if that QR is to be improved beyond the ”next” breakpoint (either utility or differentiation depending on its current position)).

-Evaluation:Two evaluations of the complete QUPER model was carried out using a qualitative research approach.A) The authors designed interview instrument and questionnaire for evaluating QUPER with 4 product managers, 2 project managers, 1 software architect, 1 test manager, 1 head of software quality, and 2 senior software engineers. Then the practitioners follow the practical guidelines to apply QUPER in practice. Finaly,the practitioners answered the self-administrated questionnaire, followed by questions (from the interview instrument) about applying the complete QUPER model in practice, which was discussed in detail. Besides, the collocted data was analyzed using content analysis form other paper.B)The second evaluation was conducted with 13 new practitioners,6 product managers, 3 project manager, 2 senior software engineers, 1 test manager, and 1 software developer. And the steps are similar. In general, the practitioners agree that the QUPER model is easy to understand, that the detailed guidelines work in an industrial environment, and the model does not take too much time to apply in practice. And the order of importance of these three views from most to least are roadmap view, benefit view, and cost view from the result of evaluation. Besides,  the identification of breakpoints in the benefit view is viewed as neither difficult, nor easy.

-One threat is related to the selection process of subjects for interviews, and another is incorrect data (internal validity). The ability to generalize the results beyond the actual study (external validity) is a threat to validity. This paper present a complete QUPER model. And as the results of evaluation, three views of QUPER are helpful and QUPER model will not take too much time to practice. But in my opinion, we still need more cases to prove that QUPER is useful. According to the identification of breakpoints, we can know if the statistical methods and standards are clear, identifying breakpoints is not so difficult. 

####•A Market-Driven Requirements Engineering Process: Results from an Industrial Process Improvement Programme

-REPEAT(Requirements Engineering ProcEss At Telelogic）is used in-house at Telelogic for eliciting, selecting and managing requirements on a product family called Telelogic Tau - a software development environment for real-time systems, used by many of the
world's largest telecommunication systems providers in their software development. It covers typical RE activities, such as elicitation, documentation, and validation, and has a strong focus on requirements selection and release planning. The actors involved in REPEAT include: Requirements Management Group (RQMG), Issuer, Customers and users and Requirements team, Construction team, Test team, Expert, Requirements Database (RQDB). The states of a requirement in the REPEAT process is: New, Assigned, Classified, Rejected, Selected, Applied.

-Process of REPEAT: 1.Elicitation phase, which includes collection and classification. Collection of requirements is made by an issuer that fills in a web form and submits the requirement for storage in RQDB(requirement database). Requirements are described using natural language and given a summary name by the issuer. When a new requirement has arrived, RQMG issues a classification of the requirement by assigning it to an expert. The expert classifies the requirement by assigning to it a rough estimate of its cost (C) and impact (/).2. Selection phase. This phase selects requirements to implement in the current release and specifies the selected requirements in more detail, and validates the requirements document.3.Change management phase, During change management, the RQMG takes decisions on changing the RD caused by new incoming requirements with priority = 1(the lowset priority). When the RD is changed, and a new requirement is allowed to enter the must-list, and a set of requirements amounting to the same effort as the new requirement must be deselected. After construction and verification, there will be entered conclusion phase.

###Reflections to the seminar discussion questions.

Seminar 0 disscused what requirement is and how to work with them. The papers of Seminar 0 presents tow methods on requirements, QUPER and PEPEAT. These two methods both can be used in the almost process of requirements engineering, except collecting original requirements. For instance, first step of QUPER is problem definition, which is similar with the elicitation phase of REPEAT, which both need define original requirements. QUPER help understand different requirement decision scenarios, while REPEAT collect and classify requirements from requirement database by issurer and expert. The second phase is about roadmapping of requirements release. According to the detail specification of requirements(REPEAT) and three views(QUPER) of requirements, I can decide the release plan of requirements. Finally, the QUPER model will involve expert to ensure the validation of the model. And if the requirements change, the new requirements will be constructed and verrificated, then enter into conclusion phase. What's more, the art and science of release plan promises to carry RP’s state of the practice to a higher level.

#### Reference  

[1]B. Regnell, R. B. Svensson, and K. Wnuk, “Can we beat the complexity of very large-scale requirements engineering?,” in Requirements Engineering: Foundation for Software Quality, Springer, 2008, pp. 123–128.

[2]M. S. Feather, S. L. Cornford, and M. Gibbel, “Scalable mechanisms for requirements interaction management,” in Requirements Engineering, 2000. Proceedings. 4th International Conference on, 2000, pp. 119–129.

[3]Introducing Support for Release Planning of Quality Requirements -An Industrial Evaluation of the QUPER Model

[4]A Case Study Evaluation of the Guideline-Supported QUPER Model for Elicitation of Quality Requirements

[5]Scaling Up Requirements Engineering –Exploring the Challenges of Increasing Size and Complexity in MarketDriven Software Development
# Seminar 1

###Qeustions
####•what tools are avaliable for Continuous Integration?未完还有一 实践

- Jenkins was created after a falling out between Hudson project contributors and the company that acquired Sun Microsystems.
- Developed in Python, Buildbot is based on the Twisted framework. It started as an alternative to the Tinderbox project and is now used in Mozilla, Webkit, Chromium, and others.
- Travis CI is probably one of the easiest CI servers to get started with.
- Strider is written in Node.JS and JavaScript, and uses MongoDB as a backing store. MongoDB and Node.js are prerequisites for installing Strider.
- Go was created and then open sourced by ThoughtWorks. As with other advanced CI servers, Go lets you distribute your builds across different systems and monitor them all in one place.
- Built on Ruby, Integrity needs Ruby 1.8.7 or newer, RubyGems 1.3.5 or newer, and Git 1.6 or newer. 

reference: https://opensource.com/business/15/7/six-continuous-integration-tools

####•what is technical product management?

Product management is the organizational structure within a business that manages the development, marketing and sale of a product or set of products throughout the product life cycle. It encompasses the broad set of activities required to get the product to market and to support it thereafter.（http://www.businessdictionary.com/definition/product-management.html）In my opinion, technical product management should be relative to a concept of marketing management. It consider the software development process from the perspective of technical. But Market-Driven Requirements Engineering (MDRE) handles the continuous flow of requirements in an engineering effort, and is not limited to a development instance but part of technical product management as a whole. The market-driven environment generates large amounts of requirements from multiple sources, internal and external, threatening to overload the technical management of products.[1]

[1]REQUIREMENTS ENGINEERING SUPPORTING TECHNICAL PRODUCT MANAGEMENT

####•What is roadmapping? How can you do it large scale?

Roadmapping is a powerful technique for planning an organisation’s technological capabilities to ensure they meet its commercial or strategic goals[1]. Roadmaps present products and technologies required to realize these products, as well as their mutual relationship over a period. Teamwork, integral involvement by the organization and good communication are essential characteristics of the process. Benefits include a shared product–technology strategy and a cross-functional approach to product and technology planning and vision building. The roadmap drafting process can be supported by such tools as maturity grid, Quality Function Deployment and the Innovation Matrix[2]. First of all, roadmapping in large scale is not a Gantt chart. Secondly, considering the roadmapping of requirement engineering with large scale, I will  take more business oriented decision when e.g. eliciting and analyzing requirements or when performing release planning[3]. From long-term perspective, roadmaps have a long term perspective, it is important to frequently update and review marketing information. The detail process of applying  roadmapping in large scale:
- Analyze market segments
- Market and competitor analysis
- Eliciting and negotiating requirements from key customers
- Planning product launches and marketing campaigns
- Identifying and analyzing Critical Success Factors (CSF)
- Identify bases of competitive advantage[3]


[1]http://www.ifm.eng.cam.ac.uk/roadmapping/

[2]Roadmapping Integrates Business and Technology

[3]Market-Driven Requirements Engineering Process Model, version 1.0
###Articles
####•A Cost–Value Approach for Prioritizing Requirements/Karlsson & Ryan

(Comment: Misses many of the points of the paper, i.e. the novel use of pair-wise comparisons (AHP) to prioritise requirements. Also, the importance of viewing requirements in multiple dimensions (cost /and/ value))

AHP is a process to decide the priority of requirements. First, we need make a n*n matrix, the n is the number of requirements. Then, we need compare each requirement, and n(n-1)/2 comparisons are required. Thirdly, Use averaging over normalized columns to estimate the eigenvalues of the matrix. And we need the sum of each the rows, as the priority matrix. The fourth step assign each requirement its relative value based on the estimated eigenvalues. While the results may not match the priority of requirements we identify. The consistency index (CI) is a first indicator of result accuracy of the pairwise comparisons and CI = (λ max− n)/(n −1). And there is a consistency indices from the scale 1 to 9 are called RI. The ratio of CI to RI for the same-order matrix is called the consistency ratio (CR), which defines the accuracy of the pairwise comparisons. As a general rule, a consistency ratio of 0.10 or less is considered acceptable.1 This means that our result here is less than ideal. In practice, however, consistency ratios exceeding 0.10 occur frequently.

To improve the early phases of the software engineering process, the RAN project use the cost-value approach to prioritize requirements. A group of experienced project members prioritize requirements, make pairwise comparisons, choose the scale to be used, and decide how many comparisons would be needed. Each requirement’s determined value and cost are relative and based on a ratio scale. The author divided the cost-value diagrams into thress distinct areas to discuss the cost and value of certain requirements. And based on the categories, the software managers were able to effectively and accurately prioritize their requirements. In general, by not implementing the requirements that contribute little to stakeholder satisfaction, you can significantly reduce the cost and duration of development. In other case PMR project, the author use cost-value approach to priority those suggesting added functionality. This rate is in line with the effort on the RAN project. The cost-value approach is a useful first step to help the trade-off analysis that is always part of multidisciplinary systems engineering. While there are some issues need to be taken into accout, like interdependencies between requirements, the number of pairwise comparisons is of O(n2). 

####•Requirements Abstraction Model/Gorschek & Wohlin

-RAM, with four abstraction levels, was developed as a response to the industrial need. The model allows for placement of requirements on different levels and supports abstraction or break down of requirements to make them comparable to each other. As the sources of the requirements vary and the equirements themselves are both direct and indirect in ature it is not surprising that they come in different hapes and forms, at multiple levels of abstraction, and escribed on varying levels of refinement. RAM is modeled towards a product perspective, supporting a continuous requirement engineering effort, aimed at taking requirements of multiple types (abstraction level) as input, and offers a structure for the work-up of these requirements. Through work with RAM, requirements on a high level of abstraction (comparable to product strategy) and a low level of abstraction (good enough as input to a project) are available. In addition, as several levels of abstraction are offered, a richer understanding can be obtained as to the purpose of a requirement, its origin and so on, by looking at requirements over the abstraction level boundaries.

-Advantage of RAM:1.offering an assurance that requirements do not violate the overall goals set by the management;2.All requirements are broken down to an abstraction level where they are good enough for initiating a development effort (project);3.Work-up of requirements means that they are formulated on the same level of abstraction, and hence they can be compared and set against one another. The ability to compare requirements is a prerequisite to effective release planning and prioritization;4.All requirements can be followed through several levels of abstraction giving a richer understanding of each requirement, and thus better decision support can be obtained for all professionals, from management to developers.

-This paper introduces a case from DHR(The DHR develops and sells software and hardware equipment for navigation, control, fleet management and service for automated guided vehicle (AGV) systems.). The authors present three issue packages during the process assessment conducted at DHR, which includes nine major improvement identified and formulaterd issues. The three issure packages are Issue-1: Abstraction level and contents of requirements;Roles and responsibilities: RE process;Requirements upkeep during and post project. What's more, this paper presents the motivation of creation and evolvement of RAM, and Evolvement of the Requirements Abstraction Model. 

-RAM process: the following three basic steps: The first step (Specify) involves specifying the initial requirement and eliciting enough information about it to specify a number of attributes. The second step (Place) is centered around what abstraction level the now specified requirements resides on and last (Abstraction) each requirement goes through a work-up. At first step, there are four attributes: Description, Reason/Benefit/Rationale, Restrictions/Risks and Title. At second step, RAM consists of a number of abstraction levels (the driving motor of the model). This step involves analyzing what level a requirement is on and placing it on this level. The Abstraction levels are Product level(goal),Feature level(features), Function level(functions/actions) and Component level(details- consists of). This third step of RAM involves abstracting and/or breakdown of a requirement, depending on the initial placement of the original requirement. The work-up process involves creating new requirements (called work-up requirements hereafter) on adjacent abstraction levels or linking to already existing ones, depending on the situation. Besides, there are another 10 attributes, such as Requirement Source, Requirement Owner, Requirements Manager and so forth.

-Tailoring RAM.This paper also provide a tailoring model for RAM: Abstraction levels (and usage of them) are a fundamental part of RAM;The number of abstraction levels needed depends on the product and organization. Three levels may suffice in some cases where requirements are generally only caught/elicited on three levels.The same reasoning applies to the abstraction degree of each level. It is dependent on the number of abstraction levels used, i.e., the jumps between levels are greater if few levels are used and vice versa. As a rule,  caught/elicited requirements and the need for work-up of the requirements determine the number of abstraction levels and the abstraction degree of these levels. Attributes need to be reviewed and adapted to the needs of the organization. As different organizations (products) are dependent on different vocabularies, domains, technical terminology, Example driven is used to descript RAM. Attributes need to be reviewed and adapted to the needs of the organization. Naming of abstraction levels, attributes, roles and so on should be adapted to fit the vocabulary of the organization. If an organization has heterogeneous products several tailored versions of RAM may be beneficial, which is called Product Focus. Beside, there are Support material to guide a result of
the other tailoring points described above. The number of abstraction levels, abstraction degree, relevant examples and so on.

-Validation of RAM: The validation is divided into two main parts, static and dynamic. Fisrt step is to identify roles. In this case, there are seven roles, Product Manager, Orderer, Project Manager, System Engineer, Developer, System Test, Upper Management. The first four roles are involved in Static Validation One and the rest roles are involved in Static Validation Two. Both validations were carried out in the form of unstructured interviews and lasted between 1 and 2 h each. Static Validation One mainly influenced RAM pertaining to size and complexity and Static Validation Two mainly influenced RAM pertaining to process-related issues. Static Validation Two validation can be divided into two main parts: RAM-produced requirements and RAM general process. The Dynamic validation was conducted in a live development. There are some questions to validate the abstraction levels and the usabolity of RAM. Still, there are some limitations of dynamic validation,e.g., difficulties of performing actul continuous requirements over a long time period which means the continuous requirements was not really tested. Besides, according to the Requirements distribution over sources and abstration levels, most of the requirements came in on Feature Level, Customer and Management groups dominated this abstraction level. The Developer group proposed most of requirements on Function Level and a fair share on Component Level as well. Management group has relatively high representation on low abstraction levels. When it comes to challenges of RAM itself, the difficulties in inventing new and completely relevant requirements may lose focus and create additional requirements that were semi-relevant.  The work-up (i.e., abstraction and breakdown) of requirements was considered beneficial since it implied analysis, refinement and completion of requirements in a structured way, and work-up requirements were comparable. The potential problems with the model were not directly associated with RAM, but rather the infrastructure needed to support RAM.

-Conclusion. This paper introduces a model RAM, which could satisfy needs identified in industry and the lack of an appropriate model to address these needs. The RAM is feasible(taloring model) and can be modified in different situations and organizations. RAM works positively in industry, All parties working with development can compare requirements, as they are homogenous regarding abstraction level and are not forced to decide between an abstract requirement and a detailed one. As flexibility and  adaptability of RAM, maybe we can modify a lightweight RAM in the future, and keep effectiveness of RAM.


####•Requirements engineering: In search of the dependent variables/Gorschek & Davis

This paper provide a framework of dependednt variables to assess quality of requirements engineering and other higher levels,  whether the project was successful, whether the resulting product was successful, whether or not the company was successful and whether there
was a positive or negative impact on society as a whole. The authors of this paper think the effect of requirements engineering transcends project instances, and attempt to change the way requirements engineering is conducted and expect that positive outcomes will result. They present a framework of dependent variables, each of which can serve as a requirements engineering quality assessment basis. The levels of requirements process change dependent variables from center to outside are Requirements Phase, Project, Product, Company and Society.

Requirements phase is the easiest measurement among companies and it inlucdes dependent variables that related to requirements cost and requirements quality. As the easiest of the five levels to measure, many researchers has proposed their theories and methods related to measures of quality of requirements sepecifications. Project level is normally equal to 'project success' and it includes dependent variables that related to project cost and time, project estimates and degree of requirements change. Project performance that related to requirements are estimation techniques, match between requirements specified and requirements satisfied, evolving requirements, and management. Procduct level determines the degree of product success, which related to requirements selection and degree of impact. There are two issues proposed, requirements selection and product strategies for measuring the success or failure of requirements engineering at the prodcut level, the authors present several methods for requirements priority, such as AHP, triage, negotiation and so forth. And the PARSEQ method is used to measure the success of the requirement selection process. GAP ananlysis and Customer Value Analysis is used to measure selection quality post-release.The requirements selection should be done within the boundaries set by product strategies. Requirements selection within the boundaries of product strategy does not guarantee success, as the strategies followed can be flawed.Internal Value Analysis (IVA) is a technique to measure whether or not a product is in line with the product strategies (and the company strategies). However, whether or not the product is really successful requires taking more factors, like revenue, resources used,etc. In company level, one product or one project success does not mean that company success. The company level includes such measures as portfolio management, strategic alignment, and degree of impact. It is closely to product scope.The main idea at the company level is to maximize the total economic benefits of several products, as opposed to the product perspective of maximizing the benefits of a particular product. Many of the same tools, e.g., GAP, CVA, and IVA, can be used. Boston Consulting Group Matrix is used to visualize the placement of individual products in relation to market maturity, as well as in relation to each other. But it is extremely difficult to assess the degree to which requirements contribute to the satisfaction of quality at the levels of company and society. Besides, it need take positive and negative externalities (reap benefits/bear costs, good-will) into account from society level. Project that contributes to a company’s bottom line but pollutes the environment or kills people must be considered a failure in society level.

A large number of dependent variables are used to assess whether a change in the requirement process has a positive or detrimental effect on the activities of the requirements phase or the success of the project. However, in order to enable us to improve requirements practices, in fact, we need to invent new dependent variables for all levels, which can provide a basis for finding an appropriate balance between technologypush and market-pull in a product development organization. Because the distance between the independent and dependent variables increases, it is not easy to build research the correlation between the RE process change and dependent variables.

It is worth noting that a process change that is highly successful at the requirements phase and project levels can be a total disaster if it results the creation of a product that nobody will buy or use. This paper create the taxonomy of a framework of dependent variables for assessing quality of requirements engineering. The framework could provide support for product strategies, but we need realize the complexity of assessment of requirements engineering process change and  the cost of requirements engineering work cannot be calculated based on what is done in association with a development instance. 

###Reflections to the seminar discussion questions.

Question of Seminar 0 has explained large scale requirements engineering. To some extent, market-driven requirements engineering is often equated to large scale requirements engineering. I did not find clear definition of MDRE and continuous requirements engineering from the papers of this seminar. According to [1], the market-driven approach to requirements engineering (market-driven requirements engineering) is the case applicable to software organizations that develop software to a market, which can be a combination of a number of known customers or, on another extreme, a mass market where customers cannot be clearly pinpointed. When looking at the term "continuous requirements engineering", there is a limited number of sources using this term in different collections of scientific papers[2]. Requirements engineering has to become a continuous activity instead of being just a part of temporary information systems projects in Continuous requirement engineering. In my opinion, this is also a software development trend that all development activities are continuous, in order to adapt to the market. There are many unique challenges in these three requirement enginering. For instance, the dependence of each requirement in LSRE is complexity, the changes of market in MDRE and  limited possibilities to see the relationship between information circulation in business processes and information life cycle in information storage systems[2]. To deal with LSRE, MDRE and continuous RE, the most important thing, I think, is to keep development process flexible, in other words, as far as possible to adapt to changes of requirements. The release planning is work for deciding which requirements really matter based on many constraints, such time and budget. The most important goal of software development is to meet the needs of stakehodler, so do release planning. Accordint to Karlsson & Ryan, they use THE ANALYTIC HIERARCHY PROCESS to prioritize the requirements so that they can decide the releas planning of requirements. But we still need to identify their relative value by ourselves. The frequency of releasing should be different, depending on the different types of software. By the way, in my opinion, the regular updates (maybe not release some new requirements) is helpful for increasing user activity. Finally, The core of release planning is considering the cost and value of each requirements, in other words, balancing the cost and value when deciding whether a requirements should be released.  

[1]Market-Driven Requirements Engineering Process Model, version 1.0

[2]Enterprise Architecture and Knowledge Perspectives on Continuous Requirements Engineering

# Seminar 2

###Qeustions
####•Read up on the Boston Matrix(add reference)

reference 

http://www.oxlearn.com/arg_Marketing-Resources-The-Boston-Matrix_11_35

####•How do you connect your requirements to your architecture?（wrong answer）

Architectural design is the point at which the requirements process overlaps with software or systems design and illustrates how impossible it is to cleanly decouple the two tasks.In many cases, the software engineer acts as software architect because the process of analyzing and elaborating the requirements demands that the components that will be responsible for satisfying the requirements be identified. This is requirements allocationthe assignment, to components, of the responsibility for satisfying requirements.[1]

[1]http://www.computer.org/portal/web/swebok/htmlformat

####•Can you connect all requirements directly? What do you do if you cannot?（weak answer）

    
###Articles
####•Are you biting off more than you can chew? A case study on causes and effects of overscoping in large-scale software engineering/Wnuk et al.

-Introduction 

There are many challengs in LSRE, such as continuously shifting market needs with a large number of new and changing requirements caused both by a capricious market situation and by evolving technologies, project scope at a large software company changed significantly throughout the entire project life cycle and the causes and effects of overscoping even though requirements engineering (RE) decision making is an acknowledged challenge. The main goal of this paper is to increase the understanding of factors involved in overscoping and thereby highlight this risk and take a step towards addressing and avoiding overscoping of projects. The contribution of the presented work includes eight main causes of overscoping complemented by a number of root causes, and nine main effects of overscoping.

-Related work

This part of this paper introduce some risk in requirements engineering, unrealistic schedules and budgets, overloading projects with scope, scope that is extended beyond the formal requirements by the developers, i.e. scope creep. This paper also mentions that there are two characteristics of MDRE which further aggravates RE decision making, namely a lack of actual customers with which to negotiate requirements and a continuous inflow of requirements from multiple channels. Scope management is considered as one of the core functions of software release planning and a key activity for achieving economic benefits in product line development 

-Case

The case study has been conducted at a large marketdriven software development company that has started to shift towards a more agile way of working. The case company has around 5000 employees and develops embedded systems for a global market using a product line approach. Several organizational units within the company are involved in the development. the requirements unit that manages the scope and the requirements; the software unit that develops the software for the platform; the product unit that develops products based on the platform releases; and usability design unit responsible for designing the user interface.The company used a stage-gate model. There were milestones (MS) for controlling and monitoring the project progress. In particular, there were four milestones for the requirements management and design (MS1–MS4) and three milestones for the implementation and maintenance (MS5–MS7). For each of these milestones,
the project scope was updated and baselined. The new development process has been influenced by ideas and principles from the agile development processes eXtreme programming (XP) and Scrum. The agile RE practices are:One continuous scope and release-planning flow (P1); Cross-functional development teams (P2); Gradual and iterative detailing of requirements (P3); Integrated requirements engineering (P4);and User stories and acceptance criteria (P5).

-Research method

- Previous research: the authors define the "RQ1: What causes overscoping?" and "RQ2: What are the effects?" for phase-based process, and "RQ3: How may agile RE practices impact the causes & effects?" for agile development process.
- Case study: 1)Phase one: pre-study and hypothesis generation: the experience of one of the authors (who has worked at the case company) was used to identify possible (assumed) causes and effect of overscoping. 5 assumed causes: continuous requirements inflow via multiple channels (C1); no overview of software resource availability (C2); low DT involvement in early phases (C3); requirements not agreed with DT (C4); and detailed requirements specification is produced upfront (C5). 2)Phase two: an interview study at the case company: semi-structured interviews with a high degree of open discussion between the interviewer and the interviewee were held. The hypothesis provided a framework that helped to discuss, explore and enrich the understanding of this complex phenomenon. 9 practitioners with roles and experiences throughout life cycle. 3)Phase three: validation of results via questionnaire. The validity of the results from 6 (other) practitioners.

-Interview results

1.causes of overscoping,还有每一个cause 的分析 root cause analysis
2. effects of overscoping
3.Impact of agile RE practices
-Validation，可以一笔带过

-Interpretation and discussion
-Conclusions and further work


####•An industrail Survey of Requirements Interdependencies in Software Product Release Planning/Carlshamre et al.(加结论)
####•Scaled Agile Framework/Leffinwell

http://www.scaledagileframework.com/ 没有免费文章

###Reflections to the seminar discussion questions.

• Roadmapping
– What is a roadmap?
– How does it connect with release planning?
– How does it connect with architecture runway?
– How can you roadmap several products at once?
• Portfolio Management
– How should we manage several products?
∗ Technically, we may do it with a product line architecture, but
what about the requirements?
∗ One Req. DB? One per product? Overlapping features?
– How do we deal with overlap between products?
∗ Cf. Gorschek & Davis
∗ Collaborative / Competitive
– How do you distribute resources between your products?


# Seminar 3
###Reflections to the seminar discussion questions.

• Into the Projects
– How do you transform epics into reasonable chunks of work?
– How do you distribute requirements between (more than) several
teams?
– How do you coordinate the development?
• Requirements and Architecture Decisions
– How do you use requirements to take decisions on construction?
– How do you find and deal with legacy requirements when designing
for a new requirement?


# Seminar 4
###Qeustions
####- tools for requirements management:

There are large number of tools for requirement management. And many of them are avalible for Agile.

- Trace Cloud: Web-based requirements management software for agile and scrum project teams.
- SpiraTest: Web-based software to help you write better requirements, manage your test cases and track defects.
- Blueptint: Blueprint’s Storyteller addresses these challenges, facilitate engagement and collaboration across the organization, ensure better Business & IT alignment and get everybody writing good, effective and consistent user stories.
- Agile manager: Agile project management solution to plan, execute and track Agile projects.
- Aligned Elements: the Medical Device ALM, management and traceability of requirements as well as other Design Control Items.
- Gatherspace.com: Requirements and Product management in the cloud. Allows product team to beautifully collaborate and share requirements.
- iPlan: Enterprise project management including requirements, personnel, defect, timesheet, quality, metrics and document management.
- Rational DOORS: a requirements management application for optimizing requirements communication, collaboration and verification throughout your organization and supply chain. This scalable solution can help you meet business goals by managing project scope and cost. Rational DOORS lets you capture, trace, analyze and manage changes to information while maintaining compliance to regulations and standards.
- Accompa: Mid-market Requirements Management Tools.

cr：http://www.capterra.com/requirements-management-software/
    http://makingofsoftware.com/resources/list-of-rm-tools

####- tools for agile requirements management:

Trace Cloud, Blueptint,  Agile manager 

###Articles
####•Assessing challenges of continuous integration in the context of software requirements breakdown: a case study/Debbiche & Dienér(This is not a readable summary of the work.)

1.introduction: 
- Changing requirements and pressure to release more often bring continuous integration.
- To support more frequent integration, requirements need to be broken down small enough.
- A case study at Ericsson, explores the challenges of continuous integration and requirements break down and how the latter influences the implementation of a continuous integration process.

2.Related work: 
- Lean software developemnt infuluences Agile Methodologies, Agile Methodologies employ continous integration, and continuous integration enable continuous deployment. Continuous integration emphasises requirement breakdown.
- The scope of this paper is continuous integration and requirement breakdown.
- Software requirement breakdown: 1)Identify direct and indirect stakehoders. The stakehoders decides the requirements. 2)Elicited requirements(funtional and non-functional) need to be prioritized. 3)RAM. Adequate leves of abstractions is essential for breaking down requirements in continuous integration process. 4)These quality and attributes in RAM do not guarantee that requirements have been broken down enough.

3.Research approach
- Research question: challenges of continuous integration process, requirement breakdown in practice and how requirement influences 
continuous integration process.
- Research methodology:case study in Ericsson
- Data collection: interview(including protocol).
- Data analysis: collected qualitatve data are  classified and analysed.

4.Case study
- Continuous integration:Teams working on SGSN-MME product use multiple branches: work branch-latest local version-pre test build-latest  stable version. Each new code need pass the test of the previous branch. For instance, pre-test bulid branch requires that the code to  pass the tests of latest local version branch.
- Requirements Breakdown:Ericsson is introduced XFT(cross functional team) and OPO(operational product owner). And it's largely up to XFT to decides how requirements breakdown.

5.Result

1) Continuous integration challenges:

a) Mindset:
- scepticism. Not everyone in developemnt team are postive about continuous intergration, but once they get the rewards of continuous integration, they will overcome the issues that they think might not good in continuous integration.
- change old habits. The continuous integration challenged the old habits that the developers are used to working.
- exposing work intention. Continuous integration emphasises early and frequent integrations.

b) Tool & Infrastructure:
- code review. Tools for reviewing integrated code has been reported to lack the nessacery features.
- maturity.These tools are not so efficient for a continuous integration process.
- regression feedback time. The feedback loops from autumated regression tests are too long.
- integration queue. Due to the SGSN-MME product(many people working at same time but in different place), it is difficult to manage the integration queue.
- Test automation. The support of test automation is lacking in the current infrastructure.

c) Testing:
- untable test case. Test cases at the studied company are sometimes unstable and may fail regardless of the code.
- too many manual tests. There are a lot of manual tests, which resulted in gaps in current testing frameworks.
- implementation and test dependencies. A problem related to writing test cases i syncing them with the code they are supposed to test.
- preserving quality. There are not so much docus on quality and a lot of developers working on this product which means guranteeing the qulity of continuous integration becomes challenging.

d) Domain applicability:
- process suitability. While taking a step towards more frequent integrations using continuous integration, the studied company has been experiencing problems using the same desired frequency throughout all parts of product.
- procudt complexity. SGSN-MME is a mature product and has been developed for over 15 years with around 30 teams.

e) Understanding:
- unclear goals. Setting up clear goals for the teams migrating towards continuous integration is currently an impediment for the SSN-MME program.
- increased pressure. The initiative to adopt continuous integration has resulted in increased pressure on the teams according to some interviewees.
- different interpretations. According to a line manager, most managers have their own understanding of what continuous integration i and should be.
- Bottom-up approach. The findings of this study indicate that continuous integration is being implemented with a bottom up approach as stated by a CI driver.

f) Code dependecies:
- integration coordination. The task of coordinating integration dependencies has been more difficult since the adoption of continuous integration.
- Dead code. Integrating partial code for a feature is currently an issue for the studied company. Tests will fail until all parts are in place.

g) Software requirement:
- requirement breakdown. The increased integration frequency has put further pressure on breaking down requiremnet.
- deliver feature growth. It is difficult to know whether small changes that do not directly add value to a frature are worth integrating.

2) Software Requirement Breakdown Challenges

a) Requirement abstraction:
- ambiguous requirements. The studied company faced ambiguous requirements.
- architectural design. It is a challenge that keep the architecture in mind when using continuous integration.
- product complexity. The SGSN-MME product has been identified as a challenge when breaking down requirements.
- large requirements. Several interviwees report on requirements being too large.
- low level requirements. One developer identifoed as a challenge the breakdown of low level requirements to allow higher integration frequencies.

b) Alignment of requirements and tests: implementation and test dependencies. Aligning the implementation of requirements and their tests is considered a problem by many developers.

c) Custormer value:
- access to customer.Sin the inroduction of continuous integration, collaborating with customer in regards to the requirements has been difficult according to some interviewees.
- delivering customer value. The studied company has introduced an addtional requirement abstraction level, more specifically "working scenarios". This allows requirements to be broken down into small pieces. But these working scenarios do not necessarily contain complete customer value.

d) Guiding princle:
- lack of guidance. The teams decide how to  break down software requirements instead of guidance.
- no unified process. Teams were given a lot of freedom, and they can set their own pace of integration and how requirements breakdown.
- ongoing esponsibility shift. Process and responsibility of breaking down software requirements is undergoing a total overhual.
- unfit process. The process used by teams is not mature enough and could be improved.

3) Software requirements breakdown's influence on continuous integration

a) The necessity of software requirements breakdown:
- maintenance versus feature development. Teams that are developing new features have been facing more difficulties while transitioning to continuous integration compared to teams that are mainly maintaining existing code and fixing bugs.
- Big impact requirements.As mentioned above, teams that are mainly involved in product feature development have more difficulties adopting continuous integration due to the issues in breaking down requirements.

b) Implications of software requirements breakdown:
- Implementation dependencies.Finding the right balance between small enough requirement units and high integration frequency without compromising the implementation unity is reported to be an issue at the studied company.
- Test dependencies.While breaking down software requirements into smaller units, it was found that test dependencies played an important role. These smaller tasks need to be individually testable if they are to be integrated separately.
- On Demand Software Delivery.Ericsson’s vision in the next couple of years is to implement On Demand Software Delivery (ODSD). While the connection of continuous integration to ODSD is not clear. The findings of this study show that continuous integration has at least a few implications on transitioning to ODSD.
- Integration scope.One implication of breaking down software requirements and integrating them in smaller chunks is that partial code might be integrated into the Pre-Test Build (PTB). This could potentially, cause exceptional behaviour to the product according to a line manager.

6.Conclusion

This study set out to identify the challenges of continuous integration and requirements break down and how the latter influences the 
implementation of a continuous integration process.

###Reflections to the seminar discussion questions.

Horizontal scaling: The Life of a Requirement
– What scope changes is likely to happen (Wnuk)?
– How do you support a released requirement?
– How do you deal with customer adaptations?
• Quality Requirements
– How do quality requirements impact other requirements?
– How do quality requirements evolve over time?
– How do you deal with differing quality requirements in a product line
setting?

