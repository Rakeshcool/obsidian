In Go, method signatures are defined using a receiver type and a method name. Here is the general format for method signatures in Go:

```go
func (receiverType) methodName(parameter1 type, parameter2 type) returnType {
    // Method body
}
```

Let's break down each component:

1. Receiver Type: It specifies the type on which the method is defined. The receiver can be either a value receiver or a pointer receiver. Value receivers operate on a copy of the receiver instance, while pointer receivers modify the original receiver instance. The receiver type is placed in parentheses before the method name.

2. Method Name: It is the identifier used to refer to the method within the program. It should be unique within its scope.

3. Parameters: These are variables or values passed to the method for it to perform its tasks. Each parameter includes a type and a name. Multiple parameters are separated by commas.

4. Return Type: It specifies the data type of the value that the method returns after its execution. If the method doesn't return a value, the return type is specified as `void` or omitted altogether.

Here's an example to illustrate the method signature in Go:

```go
type Circle struct {
    radius float64
}

func (c Circle) calculateArea() float64 {
    return math.Pi * c.radius * c.radius
}
```

In this example, we define a type `Circle` with a single field `radius`. The `calculateArea` method is defined on the `Circle` type. It takes no parameters and returns a `float64` value representing the area of the circle.

It's worth noting that Go also allows defining methods on pointer receivers, which can be useful for modifying the original receiver instance. To define a method on a pointer receiver, the receiver type is specified with an asterisk `*` before the type name. Here's an example:

```go
func (c *Circle) setRadius(newRadius float64) {
    c.radius = newRadius
}
```

In this example, the `setRadius` method is defined on the pointer receiver `*Circle`. It takes a `float64` parameter `newRadius` and modifies the `radius` field of the original `Circle` instance.