```go
package proxy

import "fmt"

type Driven interface {
        Drive()
}

type Car struct{}

func (c *Car) Drive() {
        fmt.Println("Car being driven")
}

type Driver struct {
        Age int
}

type CarProxy struct {
        car    Car
        driver *Driver
}

func (c *CarProxy) Drive() {
        if c.driver.Age >= 16 {
                c.car.Drive()
        } else {
                fmt.Println("Driver too young")
        }
}

func NewCarProxy(driver *Driver) *CarProxy {
        return &CarProxy{Car{}, driver}
}

func main() {
        car := NewCarProxy(&Driver{12})
        car.Drive()
}
```

***

![Proxy Pattern](images/proxy.png)

***


[Proxy in Go](https://refactoring.guru/design-patterns/proxy/go/example#:~:text=Proxy%20is%20a%20structural%20design,request%20to%20a%20service%20object.)

Proxy is a structural design pattern that provides an object that acts as a substitute for a real service object used by a client. A proxy receives client requests, does some work (access control, caching, etc.) and then passes the request to a service object.



![Example](images/proxy_in_go.png)
