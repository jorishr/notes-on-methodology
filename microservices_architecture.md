# Microserivices

## The problem

In the traditional approach a (web) application's codebase is broken up into modules that represent a part of the functionality for better maintenance. Those modules are then compiled into one single application that is delivered to the server/end user.

- As the complexity of applications increases testing and redeploying a monolythic app after each minor update can become inefficient.
- Scalability: not every part of the codebase needs to scale at the same rate. For example, the shopping cart functionality of a web shop needs to be able to handle spikes in traffic but other parts of the website not so much.

## The microserives solution

Build an application that consists of a series (re-usable?) mini-applications that can maintained independently and deployed to their own server. That server can than scale elastically following the demand for each individual service.

All service need to be configured so they can talk to each other through an API. Here also lies a possible drawback, as that process needs to be thought through very well from an archeticual point of view. 

Usually, the use of microservice architecture is recommended only for large scale projects with a lot of people working on the various application inside that project. For small and medium size projects microservices will probably introduce unnecessary complexity.

The so-called sweet spot is to work with a monolythic app whereby you put the various databases in Docker containers.

## NodeJs Implementation Example with Docker and Nginx

See video playlist by Fredrik Christenson:
[Video1](https://www.youtube.com/watch?v=aWxR05rUoto)
[Video2](https://www.youtube.com/watch?v=QjhJs31h_4k)

