- comparison:
  - Feature                             |                         Responsible Component
  - Syntax error detection before build |                 ✅ Roslyn (C# compiler) in the editor
  - Real-time feedback                  |                       ✅ IntelliSense + Roslyn
  - Build errors                        |                    ✅ C# compiler (during build)
  - Runtime errors                      |                    ✅ CLR (when running the app)

- Short Circuit (&&, ||)
  - true || true || true || true || true || true || true || true || true || true     ---> if first condition is true, no need to check the rest. (it saves execution time)
  - true | true | true | true | true | true | true | true  ---> it will check all of them. even if the first condition is true.

- s1 == s2     ---> it should be false (s1_address is equal s2_address??)

- array_name[2..^2] ---> starting from 2 including all elements until the element before the second one from the last. counting from back starting from 1. the date type of the value 2..^2 is range.

- bounds checking ---> it is made by CLR. it is checking in the runtime whether the indexing is out of bounds or not and if it is, an exception will be thrown.

- void expression:
  - Console.WriteLine("Hello World!");
 
- ??   ---> null coalescing operator

- null reference exception:
  - case: s1.ToUpper(); and s1 is null
  - solution: s1?.ToUpper();  ---> if it is not null, then call ToUpper method otherwise return null.
  - another solution: s1 is null? null : s1.ToUpper();
 
- c++ ---> print then increment
- ++c ---> increment then print

- for is better in performance than for each

- everything in .NET derived from Object datatype

- boxing ---> from value type to reference type
- unboxing ---> from reference type to value type

- PadLeft(8, '0');

- char[] CharArrayName = string_name.ToCharArray();

- default class modifier ---> internal

- Class members:
  - fields ✅
  - constants ✅
  - properties
  - method
  - event
  - operator
  - indexer
  - constructor
  - finalizer
  - nested type

- Accessing constant from a class is in this way: class_name.const_name

- object = instance of a class

- static and const is stored in an area of heap called "high frequency heap"

- (instance vs static) method
