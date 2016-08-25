# Seminar 0
###Qeustions
####• What is large scale requirements engineering?

~1000  orders of magnitude requirements.The requirements Managing a complete set of interdependencies is practically unfeasible, but feasible among small bundles of requirements[1]. 

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

According to the B.Renell, The order of magnitude of the number of requirements are 1000. The 100 order of magnitude is medium scale requirements and the 10000 order of magnitude is very large scale reuiqrements engineering[1].

####• Read up on and summarise [Strategic] Release Planning

Release planning is a process applying various types of upstream decision-making that combine market considerations with implementation concerns. Release planning involves aspects such as selecting what features and requirements should be in a certain
release, when it should be released, and at what cost[3].

Release planning, the process of deciding which features and quality level should be included in which release [3], which is both a cognitively and computationally difficult problem, is classified as a wicked problem since different kinds of uncertainty make it difficult to formulate and solve the problem. Moreover, the objective of release planning is to ’maximize the benefit’; however, the difficulty lies in how to give a measurable definition of ’benefit’[4].

###Articles
####•The Art and Science of Software Release Planning

-A good release plan should provide maximum bussiness value, satisfy the most important stakerholders, be fesible with available resource and reflect dependencies among features.

-Resease planning is ad hoc and rarely based on sound models and methodologies.It is hard to select and scheule features. Planning and follow-up replanning leads many extra activities. Another problem is that the planning scope is often limited to just the next release. Even though there are guidelines exist for release plan in princple, they don't tell us how to operate.

####•Introducing Support for Release Planning of Quality Requirements -An Industrial Evaluation of the QUPER Model

-QUPER model is developed for supporting release planning and roadmapping of quality requirements.This paper presents one case of QUPER tailoring, implementation, and most important evaluation, conducted at Sony Ericsson. The QUPER model was developed in three main steps: 1. Problem definition help understand different requirement decision scenarios; 2.Model definition based on first step and including a benefit view, a cost view, a roadmap view, and the concepts of benefit breakpoints and cost barriers; 3. Experts are ivolved in Model validation. And we can observe that quality is continuous and non-linear from these views.

-The authors tailored the QUPER model and define 4 steps as following 1. Define quality aspects. 2. Estimate your product’s current quality (for a given release) and the competing products’ quality (at present or envisioned). 3. For each quality aspect and for each relevant qualifier, estimate the breakpoints. 4. Estimate candidate targets and discuss and decide on actual targets for coming releases. They involved in improving the practice of release planning of quality requirements by introducing the QUPER model. There are three steps, Interview, Workshop and Interview again. In Interviews, they collected and analyzed data. In Workshop, they applied QUPER in real projects. Besides, they took some meastures to increase validity. 

-QUPER works well in the four areas, Network access, Email, Video systems and Positioning. But there are still some challenges, like Difficult to identify differentiation and saturation breakpoints in Network access area, people may interpret the breakpoints differently in Email area, people spend too much time on applying QUPER and so forth. Other challenges were how to specify
performance requirements that are quantifiable, representative of the “real world”, and under what conditions they should be fulfilled and specification of performance requirements. And during the interviews, one more challengs are proposed which is difficulties to identify the values of the differentiation and saturation breakpoints.

-I leard a lot from this artcle. First is the real platform development process from Sony Ericsson. It comprisesthe roadmap extraction, selection of features on the roadmap, definition of initial scope, prioritizition and project priority for the platform project. Second, I understand some concepts deeper like QUPER, PR(performance requirement), competitor analysis and so on. Third, each model and method may works well in somw aspects, we still need understand these model or method may lead some challenges. We should analyze if it worth to apply them. 

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

#### Reference  

[1]B. Regnell, R. B. Svensson, and K. Wnuk, “Can we beat the complexity of very large-scale requirements engineering?,” in Requirements Engineering: Foundation for Software Quality, Springer, 2008, pp. 123–128.

[2]M. S. Feather, S. L. Cornford, and M. Gibbel, “Scalable mechanisms for requirements interaction management,” in Requirements Engineering, 2000. Proceedings. 4th International Conference on, 2000, pp. 119–129.

[3]Introducing Support for Release Planning of Quality Requirements -An Industrial Evaluation of the QUPER Model

[4]A Case Study Evaluation of the Guideline-Supported QUPER Model for Elicitation of Quality Requirements

[5]Scaling Up Requirements Engineering –Exploring the Challenges of Increasing Size and Complexity in MarketDriven Software Development
# Seminar 1

###Qeustions
####•what tools are avaliable for Continuous Integration?
####•what is technical product management?
####•What is roadmapping? How can you do it large scale?

###Articles
####•A Cost–Value Approach for PrioritizingRequirements/Karlsson & Ryan
####•Requirements Abstraction Model/Gorschek & Wohlin

-RAM, with four abstraction levels, was developed as a response to the industrial need. The model allows for placement of requirements on different levels and supports abstraction or break down of requirements to make them comparable to each other. As the sources of the requirements vary and the equirements themselves are both direct and indirect in ature it is not surprising that they come in different hapes and forms, at multiple levels of abstraction, and escribed on varying levels of refinement. RAM is modeled towards a product perspective, supporting a continuous requirement engineering effort, aimed at taking requirements of multiple types (abstraction level) as input, and offers a structure for the work-up of these requirements. Through work with RAM, requirements on a high level of abstraction (comparable to product strategy) and a low level of abstraction (good enough as input to a project) are available. In addition, as several levels of abstraction are offered, a richer understanding can be obtained as to the purpose of a requirement, its origin and so on, by looking at requirements over the abstraction level boundaries.

-Advantage of RAM:1.offering an assurance that requirements do not violate the overall goals set by the management;2.All requirements are broken down to an abstraction level where they are good enough for initiating a development effort (project);3.Work-up of requirements means that they are formulated on the same level of abstraction, and hence they can be compared and set against one another. The ability to compare requirements is a prerequisite to effective release planning and prioritization;4.All requirements can be followed through several levels of abstraction giving a richer understanding of each requirement, and thus better decision support can be obtained for all professionals, from management to developers.

-This paper introduces a case from DHR(The DHR develops and sells software and hardware equipment for navigation, control, fleet management and service for automated guided vehicle (AGV) systems.). The authors present three issue packages during the process assessment conducted at DHR, which includes nine major improvement identified and formulaterd issues. The three issure packages are Issue-1: Abstraction level and contents of requirements;Roles and responsibilities: RE process;Requirements upkeep during and post project. What's more, this paper presents the motivation of creation and evolvement of RAM, and Evolvement of the Requirements Abstraction Model. 

-RAM process: the following three basic steps: The first step (Specify) involves specifying the initial requirement and eliciting enough information about it to specify a number of attributes. The second step (Place) is centered around what abstraction level the now specified requirements resides on and last (Abstraction) each requirement goes through a work-up. At first step, there are four attributes: Description, Reason/Benefit/Rationale, Restrictions/Risks and Title. At second step, RAM consists of a number of abstraction levels (the driving motor of the model). This step involves analyzing what level a requirement is on and placing it on this level. The Abstraction levels are Product level(goal),Feature level(features), Function level(functions/actions) and Component level(details- consists of). This third step of RAM involves abstracting and/or breakdown of a requirement, depending on the initial placement of the original requirement. The work-up process involves creating new requirements (called work-up requirements hereafter) on adjacent abstraction levels or linking to already existing ones, depending on the situation. Besides, there are another 10 attributes, such as Requirement Source, Requirement Owner, Requirements Manager and so forth.

-Tailoring RAM.This paper also provide a tailoring model for RAM: Abstraction levels (and usage of them) are a fundamental part of RAM;The number of abstraction levels needed depends on the product and organization. Three levels may suffice in some cases where requirements are generally only caught/elicited on three levels.The same reasoning applies to the abstraction degree of each level. It is dependent on the number of abstraction levels used, i.e., the jumps between levels are greater if few levels are used and vice versa. As a rule,  caught/elicited requirements and the need for work-up of the requirements determine the number of abstraction levels and the abstraction degree of these levels. Attributes need to be reviewed and adapted to the needs of the organization. As different organizations (products) are dependent on different vocabularies, domains, technical terminology, Example driven is used to descript RAM. Attributes need to be reviewed and adapted to the needs of the organization. Naming of abstraction levels, attributes, roles and so on should be adapted to fit the vocabulary of the organization. If an organization has heterogeneous products several tailored versions of RAM may be beneficial, which is called Product Focus. Beside, there are Support material to guide a result of
the other tailoring points described above. The number of abstraction levels, abstraction degree, relevant examples and so on.

-Validation of RAM: The validation is divided into two main parts, static and dynamic. Fisrt step is to identify roles. In this case, there are seven roles, Product Manager, Orderer, Project Manager, System Engineer, Developer, System Test, Upper Management. The first four roles are involved in Static Validation One and the rest roles are involved in Static Validation Two. Both validations were carried out in the form of unstructured interviews and lasted between 1 and 2 h each. Static Validation One mainly influenced RAM pertaining to size and complexity and Static Validation Two mainly influenced RAM pertaining to process-related issues. Static Validation Two validation can be divided into two main parts: RAM-produced requirements and RAM general process. The Dynamic validation was conducted in a live development. There are some questions to validate the abstraction levels and the usabolity of RAM. Still, there are some limitations of dynamic validation,e.g., difficulties of performing actul continuous requirements over a long time period which means the continuous requirements was not really tested. Besides, according to the Requirements distribution over sources and abstration levels, most of the requirements came in on Feature Level, Customer and Management groups dominated this abstraction level. The Developer group proposed most of requirements on Function Level and a fair share on Component Level as well. Management group has relatively high representation on low abstraction levels. When it comes to challenges of RAM itself, the difficulties in inventing new and completely relevant requirements may lose focus and create additional requirements that were semi-relevant.  The work-up (i.e., abstraction and breakdown) of requirements was considered beneficial since it implied analysis, refinement and completion of requirements in a structured way, and work-up requirements were comparable. The potential problems with the model were not directly associated with RAM, but rather the infrastructure needed to support RAM.

-Conclusion. This paper introduces a model RAM, which could satisfy needs identified in industry and the lack of an appropriate model to address these needs. The RAM is feasible(taloring model) and can be modified in different situations and organizations. RAM works positively in industry, All parties working with development can compare requirements, as they are homogenous regarding abstraction level and are not forced to decide between an abstract requirement and a detailed one. As flexibility and  adaptability of RAM, maybe we can modify a lightweight RAM in the future, and keep effectiveness of RAM.


####•Requirements engineering: In search of the dependent variables/Gorschek & Wohlin

# Seminar 2

###Qeustions
####•Read up on the Boston Matrix(加引用)
####•How do you connect your requirements to your architecture?（回答错了）
####•Can you connect all requirements directly? What do you do if you cannot?（weak answer）

###Articles
####•Are you biting off more than you can chew? A case study on causes and effects of overscoping in large-scale software engineering/Wnuk et al.
####•An industrail Survey of Requirements Interdependencies in Software Product Release Planning/Carlshamre et al.(加结论)
####•Scaled Agile Framework/Leffinwell

http://www.scaledagileframework.com/ 没有免费文章

# Seminar 4
###Qeustions
- tools for requirements management:

There are large number of tools for requirement management. And many of them are avalible for Agile.

- Trace Cloud: Web-based requirements management software for agile and scrum project teams.
- SpiraTest: Web-based software to help you write better requirements, manage your test cases and track defects.
- Blueptint: Blueprint’s Storyteller addresses these challenges, facilitate engagement and collaboration across the organization, ensure better Business & IT alignment and get everybody writing good, effective and consistent user stories.
- Agile manager: Agile project management solution to plan, execute and track Agile projects.

- tools for agile requirements management:


###Articles
####•Assessing challenges of continuous integration in the context of software requirements breakdown: a case study/Debbiche & Dienér(This is not a readable summary of the work.)



