# Design Patterns in Go

* [Go Patterns](https://github.com/tmrts/go-patterns)
* [All Design Patterns in Go (Golang)](https://golangbyexample.com/all-design-patterns-golang/)
* [Design Patterns in Go](https://refactoring.guru/design-patterns/go)
* [GoF Design patterns that still make sense in Go](https://dev.to/mauriciolinhares/gof-design-patterns-that-still-make-sense-in-go-27k5)

***

## Creational Design Patterns (ABF-P-S)

* [Abstract Factory](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/abstract_factory/abstract_factory.md)
* [Builder](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/builder/builder.md)
* [Factory Method](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/factory/factory.md)
* [Prototype](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/prototype/prototype.md)
* [Singleton](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/singleton/singleton.md)
* [Object Pool](https://github.com/muarshad01/Design_Patterns_Go/blob/master/creational_design_patterns/object_pool/object_pool.md)

***

## Structural Design Patterns (ABCD-F2-P)

* [Adapter](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/adapter/adapter.md) -- Database / SQL package
* [Bridge](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/bridge/bridge.md)
* [Composite](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/composite/composite.md)
* [Decorator](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/decorator/decorator.md) -- Adding buffers to IO classes
* [Flyweight](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/flyweight/flyweight.md)
* [Facade](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/facade/facade.md)
* [Proxy](https://github.com/muarshad01/Design_Patterns_Go/blob/master/structural_design_patterns/proxy/proxy.md)

***

## Behavioural Design Patterns (C2-I-M2-O-S2-TV)

* [Chain of Responsiblity](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/chain_of_responsibility/chain_of_resp.md) -- Passes request along a chain-of-potential-handlers (type Handler Interface{})
* [Command](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/command/command.md)
* [Iterator](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/iterator/iterator.md) -- sql.Rows
* [Memento](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/memento/memento.md) -- Take Snapshots and Restore Later
* [Mediator](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/mediator/mediator.md) -- Facilitates indirect communication
* [Observer](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/observer/observer.md) -- Notification Service (Channels: Produce & Consumer(s))
* [State](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/state/state.md)
* [Strategy](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/strategy/strategy.md)
* [Template Method](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/template/template.md) -- Sorting objects is a pretty typical example of Template Method still in action in Go.
* [Visitor](https://github.com/muarshad01/Design_Patterns_Go/blob/master/behavioral_design_patterns/visitor/visitor.md)

***

## UML Diagram

* [How to turn your Golang programs into UML Class diagrams](https://www.reddit.com/r/golang/comments/ccc3cd/how_to_turn_your_golang_programs_into_uml_class/)
* [GitHub goplantuml](https://github.com/jfeliu007/goplantuml)
* [PlantUML](https://www.plantuml.com/plantuml/uml/SyfFKj2rKt3CoKnELR1Io4ZDoSa70000)


```go
$ go get github.com/jfeliu007/goplantuml/parser
$ go install github.com/jfeliu007/goplantuml/cmd/goplantuml@latest

$goplantuml $GOPATH/src/patterns/proxy > proxy.puml
```

***

## Useful Links

* [Welcome To Golang By Example](https://golangbyexample.com/)
* [Awesome Go](https://github.com/avelino/awesome-go)

## Ohter
* [Python Design Patterns](https://python-patterns.guide/)
