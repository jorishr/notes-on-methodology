# Overview of the Web development process
- [Overview of the Web development process](#overview-of-the-web-development-process)
  - [The web development process](#the-web-development-process)
  - [Time estimations](#time-estimations)
  - [Getting familiar with existing code base](#getting-familiar-with-existing-code-base)
  - [Testing, design patterns and workflows](#testing-design-patterns-and-workflows)
  - [Code optimizations](#code-optimizations)

## The web development process
1. Analysis
- website purpose
- website goals
- website target audience

2. Planning
- site map
- structure
- tech stack

3. Design
- wire frame models
- visual style
- usability of ui/ux

4. Content
- copywriting
- photos and videos
- SEO

5. Development
- HTML/CSS/JS
- responsiveness
- databases: Define and set up the tables/objects in your database. Write the code that connects database and UI.

6. Testing
- technical tests
- browser compatibility
- website purpose check

7. Deployment
- monitoring
- bug fixes
- maintenance

Submit small pieces of code for review, don't wait for large chunks that might be rejected.

## Time estimations
The rule of thumb is to add 50% on top of all your projections. The key part is to get a precise picture of all the requirements. A simple task may be much more complex then originally anticipated and that can turn a one day task into an entire week. 

## Getting familiar with existing code base
To get really comfortable, count on 3 months
- ask questions about what is needed: database and tools
- check the dependency tree in package.json and identify key packages
- start analyzing the code at *the most used part of the application*: which network requests are being made; store urls; entry points of the system; link from entrypoint to database.

## Testing, design patterns and workflows
Test Driven Development (TDD) and Domain Driven Development (DDD) are *usually* not really part of the front-end development workflow. Especially in front-end, the way things are done can vary widely from company to company. It is useful to know about these things, but they are not a priority.

## Code optimizations
One can find a lot of tweaks, tips and tools to optimize front-end code. For example, how to optimize your React app. This is indeed an important topic because users expect a smooth experience. On the other hand, processing power on the average phone or laptop today can handle the most common React Apps or JS code without any issues, even without specialized optimizations. 
The true bottleneck is usually the read and write operations on the database. Look up stored procedures for SQL databases. It's a specialized skill and can most of the time do more than tiny tweaks for front-end code.