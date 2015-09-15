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
# Function Call Arguments
- Argument Separators (',' | ' ,' | ' , ' | ', ')

   Enforce the given value for argument separation

- Argument on new line (int n > 0 | bool | overflow)

   Enforce arguments are wrapped. 
 - `n` : allow up to (`n`) arguments in a funcation call without wrapping

 - `true` : same as n=1

 - `false` : same as overflow

 - `overflow` : allow as many arguments as possible without going over `Line Length` check

- Parenthesis on separate line  (none | both | start | end | wrappedstart)

   Enforce that Parenthesis in Function calls are on their own new line

- Indentation when arguments are wrapped  (inherit | double | parenthesis | first)
  - `inherit` : from `Indentation` config
      <pre>
        foobar('1',
          '2');
      </pre>

  - `double` : indent by double the `Indentation` config
      <pre>
        foobar('1',
            '2');
      </pre>

  - `parenthesis` : indent by double the `Indentation` config
      <pre>
        foobar('1',
              '2');
      </pre>

  - `first` : indent by double the `Indentation` config
      <pre>
        foobar('1',
               '2');
      </pre>

- Space before parenthesis (bool)
