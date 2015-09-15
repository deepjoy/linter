[Index](index) |
[General](general) |
[Statement Specific](statement) |
[Directives](directive) |
[Variable Declarations](variable) |
[Comments](comment) |
[Keywords](keyword) |
[Arrays](array) |
[Maps/Objects](map) |
[Execution Blocks](block) |
[Function Call Arguments](call) |
[Function Declaration](function)

---
# Execution Blocks
 - Curly braces on separate line (none | both | start | end | { value <>, except : [ conditional ,  functionarg ])

   Enforce that the curly braces in execution block are on their own new line. possible exceptions
  - `conditionals` : e.g. ``` if (true) { print 'hello';}; ```

  - `functionarg` : e.g. ``` foobar(() => { ... }); ```

 - Require newline before block (bool | {except: [first]})

 - Require newline after block (bool | {except: last, function call, constructor call, array element, object value})

 - EmptyBlocksAllowed (bool)