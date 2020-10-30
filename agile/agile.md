# Agile software development
Table of contents
- [Agile software development](#agile-software-development)
  - [About Agile](#about-agile)
  - [JIRA example: stories, epics and sprints](#jira-example-stories-epics-and-sprints)
  - [Workshop: Agile inside out blueprint](#workshop-agile-inside-out-blueprint)
    - [Horizontal slicing approach](#horizontal-slicing-approach)
    - [Vertical slicing approach](#vertical-slicing-approach)
  - [Story slicing](#story-slicing)

## About Agile
Agile is software development methodology to break up large amounts of work into manageable pieces. By dividing work into smaller chunks a team can become more agile and output features more rapidly as it gives a better overview and understanding of what the build actually includes and how much time it may take to complete.

A resume of Agile: you focus on an iterative process whereby each iterations produce a minimally viable progression or addition. After each sprint the client gets an output they can comment upon. 

This is great for consultancies as they try to make the client happy on each interaction.

A possible drawback may be that there is not enough overall vision or strategy. 

Kanban and scrum are frameworks or guidelines on how to organize that agile methodology.

## JIRA example: stories, epics and sprints
Stories are the individual feature that have to be added. They include requirements and a description. For example, "As user, I want to share the blog post on twitter". 

Each story gets a difficulty level assigned to it (1,2,3,5,8)

Epics are a way to group pieces of work together to represent a more comprehensive feature. Adding authentication, for example, can group various stories such as "As a guest, I want to sign in through Google using OAuth" and "As an authenticated user, I want to change my password".

Sprints are a way of planning out how the work will actually get done. Sprints typically represent a period of time in which a particular chunk of work will be done. 

Difficulty points will roughly translate to an average amount of time of work for each developer. While 1 point for an experienced developer could be 1 hour, that same 1 point could mean 3 hours for a less experienced developer.

## Workshop: Agile inside out blueprint
- See Gary Straughan, Development that pays.

STEP I: Get specific with one agile framework: you pick either SCRUM or KANBAN

STEP II: Get complete (though not perfect)
See checklist for either SCRUM OR KANBAN. SCRUM is more widely adopted, KANBAN has less 'tasks' and 'roles' to be performed.

STEP III: Get visual
List the things to do. Split the things "in progress" into DESIGN, DEVELOPMENT, TESTING, before they are moved into DONE.

STEP IV: Get constraint
The work in progress needs to be limited. As a team you have to figure out what you are capable of delivering. This capacity is limited and should be taken seriously, don't overestimate or brag about.

STEP V: Get predictable
From an organizational prespective predictability is important, more so then fast delivery. Predictably putting out results is key,

### Horizontal slicing approach
- Sprint one: database; 
- Sprint two: back-end; 
- Sprint three: front-end;

The problem with this approach is that the customer probably only gets to see something after three sprint cycles.

### Vertical slicing approach
In the first sprint you do some rudimentary work on database, back-end and front-end to get something out to the customer and in subsequent sprints you refine the product.

## Story slicing
Attempt to combine both approaches: What are the options for delivering value to a customer as soon as possible?

- Example of narrowing down a problem

The question: 'What are some options for delivering to a customer the ability to pay bills online as soon as possible?', leads to uncovering customer-centric, independently implementable and valuable capability options such as: by PayPal, by credit card, by direct debit.

We can then judge and pick the simplest and quickest of the more precise options, and ask the same question again: 'What are some options for delivering to a customer the ability to pay bills online using PayPal as soon as possible?'

From there on you develop that option and show it to the client to get some feedback. In the next cycle you then add other payment options.