# Domain Driven Development
The basic idea is simple and similar to separation of concerns: you separate code into models and assign functionality to those models that corresponds with part of the business logic.

## Example
A web shop has a user model and an order model. You can add all functionality to the user model class but that becomes problematic when you have a lot of functionality propped into one single class. Each new instance of that class is bloated. It may be better to spread that out to other classes. 

For example, the confirmation email, where does it go?

A purchase class could hold all functionality about user adding product to cart and completing order.

The email service can be a separate domain as well, triggered by the purchase service.

Thus you avoid of 'God' class whereby the user class can do almost anything in the system. A user class will contain the functionality for updating and deleting the account but the service related functionality can found in separate modules.