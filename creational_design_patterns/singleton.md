
## Singleton Design Pattern

[Singleton in Go](https://refactoring.guru/design-patterns/singleton/go/example)

Singleton is a *creational* design pattern, which ensures that only one object of its kind exists and provides a single point of access to it for any other code.

Singleton has almost the same pros and cons as *global* variables. Although they’re super-handy, they break the modularity of your code.

You can’t just use a class that depends on a Singleton in some other context, without carrying over the Singleton to the other context. Most of the time, this limitation comes up during the creation of unit tests.

***

![Conceptual Example](https://github.com/muarshad01/Design_Patterns_Go/tree/singleton/creational_design_patterns/cdp_images/single_go.png)
