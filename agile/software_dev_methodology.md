# Software development methodology
Table of contents
- [Software development methodology](#software-development-methodology)
	- [Agile](#agile)
	- [Agile in practice](#agile-in-practice)
	- [SCRUM](#scrum)
	- [Kanban](#kanban)
		- [Lean](#lean)
		- [Kanban board](#kanban-board)

## Agile
Instead of a waterfall approach whereby discovery, design, development and deployment are chained next to each other you go through cycles of sprints that are repeated multiple times and each iteration provides feedback and new input that may make the end-product better. 

You get a minimum viable product MVP in front of the client and/or end-user as soon as possible and observe how they use it. 

The biggest difference with a waterfall approach is that programmers are involved with content and navigation from the beginning. Individual challenges are addressed as they arise rather than waiting to make large-scale changes before launch. 

Beta launches have also become standard in order to start collecting feedback as early as possible. Maintenance is viewed as equally important to all of the other steps.

## Agile in practice
The agile process introduces a daily evaluation of the information that comes from writing the actual code. The original plan will be updated or adapted to the issues that arise.

Important is to focus on the priciple of agility and ability of the organisation to adapt rapidly to new information. The processal implementation should not be scacred, i.e. a daily stand-up may become an unproductive ritual when roadblocks are not adequately adressed or suggestions take a long time be actually being implemented in a revised plan. 

One hypothetical example: you can build atomic elements in one sprint (large HTML/CSS components), in the next you make the basic connection into molecules (CSS page section modules). Then you create organisms (chained page-sections). Next step is to have a fully functional template ready. Final sprint is to swap dummy content for actual text and images. 

## SCRUM
Scrum is an incremental and interative AGILE process or framework. The setup has three main components: product owner, scrum master and the dev team.

- product backlog: list with all the features that have to be build in order of priority

- sprint backlog: list of features that is chosen by the team to be completed in the next sprint cycle, SPRINT PLANNING. Developers independently assign priority and time estimates for each task AND evaluate after each sprint.

- scrum meetings: short, daily meetings to check in and set the course for the workday.

- scrum/agile master: responisble for managing communication between team members

- shippable increments: fully-functioning applications that showcase a feature or the final product. Ideally, each sprint will result in a shippable increment.

- sprint review: show off the new features to product owner.

- sprint retrospective: what can be learned from the previous sprint? Aim is to make the next sprint more efficient and effective.

## Kanban
Kanban too is a framework for Agile implementation. The difference hereis is the pull system. That is the way the product backlog gets converted into a product that the end-user can work with. 

KANBAN has no sprints and works as a continous process whereby a new item is pulled-out when done and a new item can be pulled from the back-log to be incorporated.

### Lean 
Lean comes from lean manufacturing principles whereby you focus primarily on those features that matter for what the end-user is using the product for. For example, you can load a page with tons of design css animations but if none of them really help the end-user to complete the purchase process then those features should not be given much time and attention.  

### Kanban board
A feature will go through a process: definition, build, review, testing, merge to master, done.

After a feature is created you are going to have a meeting or GROOMING session for that feature whereby you break the feature into smaller tasks and formulate a number of questions that come to mind about the specifics layout and functionality of the feature.

Once a task is completed you ADD PULL REQUEST ON GITHUB so someone can look at your code.