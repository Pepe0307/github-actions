# Go by Example: Detailed Topics

## 1. Hello World
- **Structure**: Basic Go program structure.
- **Components**:
  - `package main`: Declares the package as `main` for executables.
  - `import "fmt"`: Imports the `fmt` package for I/O functions.
  - `func main()`: Entry point of the program.
  - `fmt.Println("Hello, World!")`: Prints to the console.

## 2. Values
- **Data Types**:
  - **Integers**: `int`, `int8`, `int32`.
  - **Floats**: `float32`, `float64`.
  - **Booleans**: `true`, `false`.
  - **Strings**: Sequences of characters.

## 3. Variables
- **Declaration**:
  - `var x int = 10`: Explicit type.
  - `y := 20`: Type inference.
  - Multiple: `var a, b int = 1, 2`.

## 4. Constants
- **Immutable Values**:
  - `const Pi = 3.14`: Fixed values that do not change.

## 5. For Loop
- **Loop Constructs**:
  - Traditional: `for i := 0; i < 10; i++ { ... }`
  - While-like: `for i < 10 { ... }`
  - Infinite: `for { ... }`
  - Control: `break`, `continue`.

## 6. If/Else
- **Conditional Logic**:
  - Basic: `if x > 0 { ... } else { ... }`
  - Multiple: `else if`.
  - Short statement: `if x := f(); x < y { ... }`

## 7. Switch
- **Multi-way Branching**:
  - Basic: `switch x { case 1: ...; case 2: ...; default: ... }`
  - No condition: `switch { case x < y: ... }`
  - `fallthrough`: Continue to next case.

## 8. Arrays
- **Fixed-size Sequences**:
  - Declaration: `var a [5]int`
  - Initialization: `a := [5]int{1, 2, 3, 4, 5}`
  - Access: `a[0]`, `len(a)`.

## 9. Slices
- **Dynamic Sequences**:
  - Creation: `s := []int{1, 2, 3}`
  - Slicing: `s[1:3]`
  - Functions: `append(s, 4)`, `copy(dest, src)`.

## 10. Maps
- **Key-Value Structures**:
  - Creation: `m := make(map[string]int)`
  - Operations: `m["key"] = 10`, `delete(m, "key")`
  - Existence: `v, ok := m["key"]`.

## 11. Range
- **Iteration**:
  - Slices/arrays: `for i, v := range s { ... }`
  - Maps: `for k, v := range m { ... }`
  - Strings: `for i, c := range "hello" { ... }`.

## 12. Functions
- **Building Blocks**:
  - Declaration: `func add(x int, y int) int { return x + y }`
  - Multiple returns: `func swap(x, y string) (string, string) { return y, x }`.

## 13. Multiple Return Values
- **Return Pattern**:
  - Example: `func f() (int, error)`.

## 14. Variadic Functions
- **Variable Arguments**:
  - Declaration: `func sum(nums ...int) int { ... }`
  - Slice call: `sum(s...)`.

## 15. Closures
- **Captured Variables**:
  - Example: `func adder() func(int) int { sum := 0; return func(x int) int { sum += x; return sum } }`.

## 16. Recursion
- **Self-calling Functions**:
  - Example: `func factorial(n int) int { if n == 0 { return 1 }; return n * factorial(n-<span class="ml-2" /><span class="inline-block w-3 h-3 rounded-full bg-neutral-a12 align-middle mb-[0.1rem]" />