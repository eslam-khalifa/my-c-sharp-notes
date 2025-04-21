- comparison:
  Feature                             |                         Responsible Component
  Syntax error detection before build |                 ✅ Roslyn (C# compiler) in the editor
  Real-time feedback                  |                       ✅ IntelliSense + Roslyn
  Build errors                        |                    ✅ C# compiler (during build)
  Runtime errors                      |                    ✅ CLR (when running the app)

- Short Circuit (&&, ||)
  - true || true || true || true || true || true || true || true || true || true     ---> if first condition is true, no need to check the rest. (it saves execution time)
  - true | true | true | true | true | true | true | true  ---> it will check all of them. even if the first condition is true.

- s1 == s2     ---> it should be false (s1_address is equal s2_address??)

- array_name[2..^2] ---> starting from 2 including all elements until the element before the second one from the last. counting from back starting from 1. the date type of the value 2..^2 is range.

- bounds checking ---> it is made by CLR. it is checking in the runtime whether the indexing is out of bounds or not and if it is, an exception will be thrown.
