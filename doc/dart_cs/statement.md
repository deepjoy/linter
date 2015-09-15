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
# Statement Specific
- For Statement, space after semi colon (bool)

- Conditional Expression
  - Space afterTest: (bool | '\n')

  - Space before consequent (bool | '\n')

  - Space after consequent (bool | '\n')

  - Space before alternate (bool | '\n')

  - Not operator allowed (bool)
    
- Unary Operators, requires spaces (bool | {except: 'pre'})

- Binary Operators, requires spaces (bool | all | before | after | none)

- Operators precede linebreaks when wrapped ('always' | 'never' | [':', ...])

- Operators succede linebreaks when wrapped ('always' | 'never' | [':', ...])

- Named anonymous functions (bool, except : ['describe', 'it', 'test', ...])

- Capitalized classnames (bool | { except : [] })
