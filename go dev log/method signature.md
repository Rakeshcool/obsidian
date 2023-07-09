Method signatures refer to the declaration of a method in programming, including the method's name, return type, and parameter types. The signature defines the unique combination of these elements that identifies a specific method within a program.

The general format of a method signature depends on the programming language, but it typically includes the following components:

1. Method name: This is the identifier used to refer to the method within the program. It should be unique within its scope.

2. Return type: It specifies the data type of the value that the method returns after its execution. In some languages, methods may not return a value, in which case the return type is typically specified as "void."

3. Parameters: These are variables or values passed to the method for it to perform its tasks. Each parameter includes a data type and a name. Multiple parameters are separated by commas.

Here are a few examples of method signatures in different programming languages:

Java:
```java
public int addNumbers(int num1, int num2)
```
In this example, the method name is "addNumbers," the return type is `int`, and it takes two integer parameters named `num1` and `num2`.

Python:
```python
def calculate_average(numbers: list) -> float:
```
In Python, the return type is specified using a "->" followed by the desired return type. This example shows a method named "calculate_average" that takes a list of numbers as a parameter and returns a floating-point value.

C++:
```cpp
void printMessage(string message);
```
Here, the method name is "printMessage," the return type is void (indicating no return value), and it takes a single parameter of type `string`.

It's important to note that method signatures may also include additional modifiers, access specifiers (e.g., public, private), exception handling, and more, depending on the programming language and its specific syntax and features.