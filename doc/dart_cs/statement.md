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
