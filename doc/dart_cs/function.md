[Index](README.md) |
[General](general.md) |
[Statement Specific](statement.md) |
[Directives](directive.md) |
[Variable Declarations](variable.md) |
[Comments](comment.md) |
[Keywords](keyword.md) |
[Arrays](array.md) |
[Maps/Objects](map.md) |
[Execution Blocks](block.md) |
[Function Call Arguments](call.md) |
[Function Declaration](function.md)

---
# Function Declaration
- Parameter Separators (',' | ' ,' | ' , ' | ', ')

   Enforce the given value for parameter separation

- Parameter on new line (int n | bool | overflow)

   Enforce parameters are wrapped. 
 - `n` : allow up to (`n`) parameters on a single line without wrapping

 - `true` : same as n=0

 - `false` : same as overflow

 - `overflow` : allow as many parameters as possible without going over `Line Length` check

- Space before parenthesis (bool)

- Space before shortHand (bool)

- Space before curly (bool)

- Require shorthand function declarations (bool | always | never)

- Shorthand declaration requires curly braces (bool | always | never)

- Function assignment ( assign | declare)
  - `assign` : require all named functions in executable code blocks to be of the type

     ```
     var a = function () {}
     ```

  - `declare` : require all named functions in executable code blocks to be of the type

     ```function a() {}```

