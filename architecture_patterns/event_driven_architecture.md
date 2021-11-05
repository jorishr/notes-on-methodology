# Event Driven Architecture
In contrast to request-response architecture, the services in an event driven system don't interact directly with each other, they don't ask for specific information directly but subscribe to events that are deemed relevant to each service. 

The request by the user goes to a gateway service and from there onwards events determine whether other services come in to play. A change or event will signal that something has changed to the event bus and other services monitor those changes in order to determine whether they 'consume' the event as well and take action or trigger events themselves.

Each service stores a log of the events that it is subscribed to and can publish events that other services can be subscribed to. 

Examples of event driven architecture: GIT, React, NodeJs.