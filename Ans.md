## Var and Val 

**var** is a mutable variable and can be assigned multiple times 
while **val** is a **CONSTANT variable** and can not be assigned multiple times and can be Initialized only single time and is known as the immutable variable in Kotlin.

```kotlin

var School : String = "Command day Sec" // initial declaration
val State : String = "Lagos"  // Initial declaration

School = "Air force Sec" // reinitialization
println(School) // this print out "Air force Sec"

State = "Anambra" // This gives a declaration error stating it can't be reinitiated 

```

## Lateinit

While in Java and other programming languages,variables can be declared without initialisation, this is note freely done in KOTLIN, If you do not want to initialize a variable in the constructor instead you want to initialize it later on in the code, the variable can be declared using the lateinit keyword.

```kotlin
   lateint var Firstname : String // this will be initialised in the code before use. 
```

## Lazy

It means lazy initialization. Your variable will not be initialized unless you use that variable in your code.

**lazy()** is a function that takes a lambda and returns an instance of **Lazy<T>** which can serve as a delegate for implementing a lazy property: the first call to **get()** executes the lambda passed to lazy() and remembers the result, subsequent calls to get() simply return the remembered result.

**lazy can only be used for val properties**

```kotlin

val testvariable: String by lazy {
  "value"
}

```
