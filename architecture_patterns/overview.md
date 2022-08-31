# Overview of architecture patterns in enterprise software

## Layered pattern
The advantage is that lower layers can be used by multiple or different higher layers.
The disadvantage is that is less suitable for high performance because each request has to travel through multiple layers.

Usa cases: simple web apps and desktop apps.
```
    Presentation layer (UI)
    Application layer
    Business logic layer
    Data access layer
```

## Client-server pattern
Examples are email, online sharing and banking but you could argue that this is a broad pattern that is also present in more sophisticated approaches. Deciding what logic should be executed on the client or the server is a complicated task.

## Model-view-control pattern
Model contains the core functionality and data. View is the interactive display of data to the user. The controller handles the input of the user.

Web frameworks use this approach.

## Event-bus pattern
The four major components are: event source; event listener; event channel; and event bus. The listeners subscribe to event channels that connect to event sources via an event bus. While multiple event sources and event listeners can be added with ease, the event bus can become a bottleneck very fast.

Examples that use this type of architecture: notification services; nodejs.

## Microservices pattern
Each service is independently deployable and is connected to an API gateway that is accessed by various different clients.

## Broker pattern
Clients connect to a broker. That broker service directs the requests to the relevant server. This is scalable but requires standardization of the underlying services to fit the broker model.

This is used in message broker software such as RabbitMQ.

## Pipe-filter pattern
This is used in Gulp, for example. An event triggers a sequence of processing steps that perform a specific function.

Other examples are code compilers.

## Peer-to-peer pattern
See bitcoin or torrent services.

## Master-slave pattern
See database structures.