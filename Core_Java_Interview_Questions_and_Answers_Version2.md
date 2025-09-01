# Core Java Interview Questions and Answers

---

## Basic Questions

### 1. What are the main features of Java?
- **Object-Oriented**, **Platform Independent**, **Simple**, **Secure**, **Robust**, **Multithreaded**.

### 2. What is JVM, JRE, and JDK?
- **JVM:** Executes Java bytecode.
- **JRE:** JVM + libraries to run Java applications.
- **JDK:** JRE + development tools.

### 3. Explain the difference between `==` and `.equals()`.
- `==`: Compares memory addresses.
- `.equals()`: Compares object content.

### 4. What is a constructor?
- A special method to initialize objects. Same name as class, no return type.

### 5. What is inheritance?
- Mechanism for a class to inherit properties and behaviors from another class.

### 6. Describe method overloading and overriding.
- **Overloading:** Same name, different parameters, same class.
- **Overriding:** Subclass redefines a method from superclass.

### 7. What is a static variable and static method?
- **Static variable:** Shared by all instances.
- **Static method:** Can be called without creating an object.

### 8. What is an interface?
- A reference type with abstract methods and static final variables.

### 9. What is exception handling?
- Managing runtime errors using `try`, `catch`, `finally`, `throw`, `throws`.

### 10. What is the purpose of the `final` keyword?
- **final variable:** Value can't change.
- **final method:** Can't be overridden.
- **final class:** Can't be subclassed.

---

## Intermediate Questions

### 11. What is the difference between ArrayList and LinkedList?
- **ArrayList:** Fast access, slow insert/delete.
- **LinkedList:** Fast insert/delete, slow access.

### 12. What is the difference between checked and unchecked exceptions?
- **Checked:** Checked at compile time.
- **Unchecked:** Checked at runtime.

### 13. What is encapsulation?
- Wrapping data and code together, restricting access via access modifiers.

### 14. What is polymorphism?
- Ability of an object to take many forms. Types: Compile-time (overloading), Runtime (overriding).

### 15. What is the `super` keyword?
- Refers to parent class members.

### 16. What is a package?
- Namespace for organizing classes and interfaces.

### 17. Explain the `this` keyword.
- Refers to the current object.

### 18. How does garbage collection work in Java?
- JVM automatically deletes unused objects to free memory.

### 19. What is the difference between `throw` and `throws`?
- `throw`: Used to explicitly throw an exception.
- `throws`: Declares which exceptions can be thrown by a method.

### 20. What are the types of inheritance in Java?
- **Single**, **Multilevel**, **Hierarchical**. Java does not support multiple inheritance via classes.

### 21. What is synchronization?
- Controlling access to shared resources in multithreading.

### 22. What are wrapper classes?
- Classes that convert primitives to objects (e.g., int to Integer).

### 23. What is the Collections Framework?
- Set of classes/interfaces for reusable data structures.

### 24. What is the difference between HashMap and TreeMap?
- **HashMap:** Unordered, allows null keys.
- **TreeMap:** Sorted, does not allow null keys.

### 25. What are the default values of primitive data types?
- **int, long, short, byte:** 0
- **float, double:** 0.0
- **char:** '\u0000'
- **boolean:** false
- **Object references:** null

---

## Advanced Questions

### 26. Explain Java Reflection.
- API for inspecting/modifying classes, methods, fields at runtime.

### 27. What is the significance of the `volatile` keyword?
- Ensures variable value is always read from main memory.

### 28. Difference between synchronized block and synchronized method?
- **Synchronized method:** Locks entire method.
- **Synchronized block:** Locks specific code block.

### 29. Explain `wait()`, `notify()`, and `notifyAll()`.
- **wait():** Makes thread wait.
- **notify():** Wakes one waiting thread.
- **notifyAll():** Wakes all waiting threads.

### 30. What is serialization and deserialization?
- **Serialization:** Object to byte stream.
- **Deserialization:** Byte stream to object.

### 31. What is the `transient` keyword?
- Fields marked transient are not serialized.

### 32. Purpose of `instanceof` operator?
- Checks if an object is of a specific type.

### 33. Difference between Array and ArrayList?
- **Array:** Fixed size, primitives/objects.
- **ArrayList:** Dynamic size, only objects.

### 34. What is autoboxing and unboxing?
- **Autoboxing:** Primitive to wrapper.
- **Unboxing:** Wrapper to primitive.

### 35. What is the diamond problem and how is it resolved in Java?
- Multiple inheritance ambiguity; Java avoids with interfaces, not classes.

### 36. What is a singleton class? How to implement?
```java
public class Singleton {
    private static Singleton instance;
    private Singleton() {}
    public static Singleton getInstance() {
        if(instance == null) {
            instance = new Singleton();
        }
        return instance;
    }
}
```

### 37. What are immutable objects?
- Cannot change after creation. Example: `String`.

### 38. What does `finalize()` do?
- Called before object destruction by GC. Use discouraged.

### 39. Deep copy vs. shallow copy?
- **Shallow:** Copies references.
- **Deep:** Copies actual objects.

### 40. What is `Optional` in Java 8?
- Container that may/may not hold a value. Prevents `NullPointerException`.

---

## Differences: String, StringBuilder, StringBuffer

- **String:** Immutable.
- **StringBuilder:** Mutable, not thread-safe.
- **StringBuffer:** Mutable, thread-safe.

---

## Access Modifiers

- **private:** Within class.
- **default:** Within package.
- **protected:** Package + subclasses.
- **public:** Everywhere.

---

If you need more details, code examples, or want questions on a specific topic, feel free to ask!