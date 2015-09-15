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
# Execution Blocks
 - Curly braces on separate line (none | both | start | end | { value <>, except : [ conditional ,  functionarg ])

   Enforce that the curly braces in execution block are on their own new line. possible exceptions
  - `conditionals` : e.g. ``` if (true) { print 'hello';}; ```

  - `functionarg` : e.g. ``` foobar(() => { ... }); ```

 - Require newline before block (bool | {except: [first]})

 - Require newline after block (bool | {except: last, function call, constructor call, array element, object value})

 - EmptyBlocksAllowed (bool)