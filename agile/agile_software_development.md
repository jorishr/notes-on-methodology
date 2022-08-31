# Software development methodology
Table of contents
- [Software development methodology](#software-development-methodology)
	- [Agile](#agile)
	- [Agile in practice](#agile-in-practice)
	- [SCRUM](#scrum)
		- [Scrum Events](#scrum-events)
		- [Scrum Roles](#scrum-roles)
		- [Scrum Artifacts](#scrum-artifacts)
	- [Agile Techniques](#agile-techniques)
		- [Extreme Programming (XP)](#extreme-programming-xp)
		- [User Stories](#user-stories)
		- [Epics and themes](#epics-and-themes)
		- [Estimations](#estimations)
		- [DevOps](#devops)
		- [Agile Reporting](#agile-reporting)
	- [Agile at Scale](#agile-at-scale)

## Agile
The goal of modern software development methodologies is to avoid two major problems of traditional development: no market feedback until advanced development stages and top down management whereby developers only follow checklists with gated stages of development that lack flexibility and feedback.

Instead of a waterfall approach whereby discovery of requirements, design, development and deployment are chained next to each other you go through cycles of sprints that are repeated multiple times and each iteration provides feedback and new input that may make the end-product better. 

You get a minimum viable product MVP in front of the client and/or end-user as soon as possible and observe how they use it. 

The biggest difference with a waterfall approach is that programmers are involved with content and navigation from the beginning. Individual challenges are addressed as they arise during each cycle. Thereby avoiding possibly large-scale changes at an advanced stage. 

Beta launches have also become standard in order to start collecting feedback as early as possible. Maintenance is viewed as equally important to all of the other steps.

## Agile in practice
The agile process introduces a daily evaluation of the information that comes from writing the actual code. The original plan will be updated or adapted to the issues that arise. Its is iterative and incremental.

Important is to focus on the principle of agility and ability of the organization to adapt rapidly to new information. The procesal implementation should not be sacred, i.e. a daily stand-up may become an unproductive ritual when roadblocks are not adequately addressed or suggestions take a long time be actually being implemented in a revised plan. 

One hypothetical example: you can build atomic elements in one sprint (large HTML/CSS components), in the next you make the basic connection into molecules (CSS page section modules). Then you create organisms (chained page-sections). Next step is to have a fully functional template ready. Final sprint is to swap dummy content for actual text and images. 

## SCRUM
Scrum is an incremental and interactive AGILE process or framework. The setup has three main roles: product owner, dev team member and scrum master. Five events (...) and three artifacts or deliverables (...).

A scrum team builds a product iteratively and incrementally during subsequent SPRINTS of maximum 30 days or less. Each sprint is a product iteration. Each sprints begins with a sprint planning session wherein the dev team members discusses with the product owner which items from the product backlog will be build. This results in a sprint backlog with the items selected from the product back log.

### Scrum Events
The dev team evaluates their progress on a daily basis in a DAILY SCRUM session. At the end of the sprint the dev team delivers a PRODUCT INCREMENT which is the usable product at that point in time. A SPRINT REVIEW is conducted with a group of stakeholders and future sprint is planning is discussed. The sprint cycle ends with a SPRINT RETROSPECTIVE, the team discusses how it can be more efficient in future sprints.

### Scrum Roles
- Product Owner: represents business stakeholders and decides what has to be build (product requirements) and in what order, defined in a product backlog. Needs to be informed of the changes that may be made by the dev team.

- Development Team has multiple functions: design, coding, testing, documentation writing. They convert a product backlog selection (sprint backlog) into a product increment during a sprint. Usually a team between 3 and 9 members. The dev team should be self-organized and takes ownership of a sprint backlog.

- Scrum master is the person that guides or coaches the product owner and dev team on how to implement Scrum. They usually work at enterprise level.

### Scrum Artifacts

- Product Backlog: list with all the features that have to be build in order of priority. It can contain: product requirements, user stories, defects, enhancement request and new features.

Big feature items are hard to estimate and should be groomed or refined to better determine the scope. For example, adding data analytics or payment options to a website. That is not specific enough and needs further clarification to be able to be broken down into manageable tasks. When turned into a user story, for example, we get a clearer view of what should be done. This refining process could be considered to be another scrum event. This could be a daily or weekly event or larger meeting at the beginning of the sprint.

- Sprint Backlog: list of features that is chosen during the sprint planning event by the dev team to be completed in the next sprint cycle. Developers independently assign priority and time estimates for each task and evaluate after each sprint in the sprint retrospective event.

- Product Increment: current done version of the product and should be usable or demonstrate some business value.

## Agile Techniques
### Extreme Programming (XP)
Can be use within the Scrum framework and uses a weekly cycle within each quarter. Usually the customer hands in a set of requirement that the dev team converts into user stories. The dev team then divides the user story into specific tasks that have to be done by the end of the week. No overtime, only work at sustainable pace, use of pair-programming for instant code review. Informative workspace whereby all necessary info is readily available to all team members (physical or electronic dashboard).

The code is writing process is usually test driven with lots of incremental refactoring.

### User Stories
Usually a three part sentence on and index card that describes, from the perspective of the end user, what should be accomplished by the application. A card is written with the description. Around that card you have a discussion within the dev team to refine the user story into specific tasks. Confirmation is to process of checking whether the user story does what the description intended for.

### Epics and themes
An epic is a large user story that includes a workflow too complex to be estimated. For example, as an administrator I should be able to set up an account for a new member. The basic version may be just to store personal data in a database but this user story usually includes more complex tasks such as storing and processing payment details, sending emails and sending data to accounting software.

Themes are groups of user stories. For example, grouping together of all payment related stories or personal information stories.

### Estimations
Absolute units of time can be used to estimate a task in hours, days or weeks. But usually a relative measure is introduced to determine the difficulty of a tasks in either exponential or Fibonacci sequence numbers: 1,2,4,8,16 or 1,2,3,5,8,13 and a question mark to indicate tasks that cannot be estimated at this point. A zero can be used to indicate trivial tasks or tasks that have already been completed. During the sprint planning a consensus should be reached about the relative difficulty of a story. 

### DevOps
The traditional sequence of events is that the developed code base is tested by a Quality Assurance team and once that stage is passed the IT operations team deploys the code on the servers into a production environment. This can create issues by itself because of the differences in development and production environments and this becomes even more problematic if a dev team pushed changes frequently with potential for new issues to arise on each update.

DevOps tools should make this process from development, over quality assurance to deployment in production more streamlined through the use of various build tools.
Continuous Integration, CI, refers to committing frequent changes to the code base. Each commit triggers a series of tasks that check the code for quality and validates the code base, using automated tests, dependency checks, code quality metrics, etc.

Continuous Delivery, CD, refers to the capability to always keep the product stable after every change so that is shippable.

Continuous Deployment refers to an automated process to deploy a product increment to a production environment.

### Agile Reporting
Reporting tools such a JIRA can allow you to track the dev teams progress through graphical representations. This may allow you to identify bottlenecks and detect problematic time estimates.

## Agile at Scale
Three basic rules apply: 
- only scale when necessary as adding additional teams or people will increase complexity. The existing team will have to set aside time for these coordination efforts.
- scale slowly
- have architectural and development standards in place.

Frameworks for scaling are usually about coordinating various SCRUM teams. Examples are Nexus, LeSS, Scrum@Scale, SAFe.