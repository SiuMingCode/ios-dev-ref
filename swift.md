# Swift Cheat Sheet

Copy each blok of code into playground to see the result

## Comment
```swift
// Single-line comment

/* multiple-line 
comment */

/* nested comment
/* inner comment */
outer comment */
```

## Variable
* `let` is always preferred when appropriate

```swift
// declare but not init, type required
let constant: Int
var variable: Int
```

```swift
// declare and init, type inferred
let constant = 0 // Int
var variable = "hi" // String
```

```swift
let constant: Int
constant = 1 // must be initialized
constant = 2 // compile-time error for reassignment

var variable = 1
variable = 2 // ok
```

```swift
// string interpolation
let str = "The current value of variable is \(variable)"
// print in console
print(str)
```

### Number
* `Int` and `Double` are preferred in most cases even if it is known as non-negative

```swift
// base
let decimal = 1
let binary = 0b1
let octal = 0o1
let hex = 0x1

// exponent
let decExp = 1.25e2 // 1.25 * 10^2 = 125.0
let hexExp = 0x1p2 // 1 * 2^2 = 4

// formatting, syntax sugar
let padding = 0001
let currency = 1_000_000
```

### Tuple
```swift
// access tuple's element by index
let tuple = (0, 1)
tuple.0 == 0 // true

// destructuring
let (x, y) = tuple
x == 0 // true

// access tuple's element by name
let tupleWithNamedElements = (x: 0, y: 1)
tupleWithNamedElements.x == 0 // true
```
