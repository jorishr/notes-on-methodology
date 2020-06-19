# SOA, Monolith, Microservices
Table of contents
- [SOA, Monolith, Microservices](#soa-monolith-microservices)
  - [The problem](#the-problem)
  - [SOA: Service Oriented Architecture](#soa-service-oriented-architecture)
  - [Microservices](#microservices)
  - [Example: Microservices mplementation in NodeJS with Docker and Nginx](#example-microservices-mplementation-in-nodejs-with-docker-and-nginx)

## The problem

In the traditional approach a (web) application's codebase is broken up into modules that represent a part of the functionality for better maintenance. Those modules are then compiled into one single application that is delivered to the server/end user.

- As the complexity of applications increases testing and redeploying a monolithic app after each minor update can become inefficient.
- Scalability: not every part of the codebase needs to scale at the same rate. For example, the shopping cart functionality of a web shop needs to be able to handle spikes in traffic but other parts of the website not so much.

Despite all the talk about microservices, most applications will start off as monolithic and move onto a more service oriented architecture as the codebase grows and more developers are involved.

## SOA: Service Oriented Architecture 
The service oriented architecture usually evolves from a growing monolithic codebase. Some part, for example, the code that handles orders in a webshop, will be put into own codebase. The end-user experience is exactly the same but now there is a seperate service that depends on the monolitic app to do its job.

## Microservices
There is no formal definition for microservices and it basically is a continuation of the SOA architecture. The difference is that the size or scope of each service is as small as possible. Thus,
you build an application that consists of a series (re-usable?) mini-applications that can be maintained independently and deployed to their own server. That server can than scale elastically following the demand for each individual service. 

All services need to be configured so they can talk to each other through an API. Here also lies a possible drawback as that process needs to be thought through very well from an architectual point of view. 

Usually, the use of microservice architecture is recommended only for large scale projects with a lot of people working on the various application inside that project. For small and medium size projects microservices will probably introduce unnecessary complexity.

The so-called sweet spot is to work with a monolythic app whereby you put the various databases in Docker containers.

## Example: Microservices mplementation in NodeJS with Docker and Nginx
See video playlist by Fredrik Christenson:
[Video1](https://www.youtube.com/watch?v=aWxR05rUoto)
[Video2](https://www.youtube.com/watch?v=QjhJs31h_4k)

