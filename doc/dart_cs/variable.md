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
# Variable Declarations
- Newline after variable declarations (last | all)

- Variable declaration require distinct per variable
      <pre>
        var a;
        var b=10;
        var c;
      </pre>

- Newline on assignment when declaring multiple variables
      <pre>
        var a,b=10,
          c;
      </pre>

- Variable format (upper-snake | lower-snake | upper-camel | lower-camel | mixed-snake)

- Static variable format (upper-snake | lower-snake | upper-camel | lower-camel | mixed-snake)

- Constant name format (upper-snake | lower-snake | upper-camel | lower-camel | mixed-snake)

- Allow dangling underscores [none | pre | post | all]