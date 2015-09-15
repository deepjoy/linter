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
# General
- Consistent Quotes ( bool '"' '\'' ) 

    enforce either all single or all double quotes. boolean will cause the first instance of a quote to be used for checking consistency

- Line breaks ( 'CR' 'LF' 'CRLF' 'file')

    enforce specific type of endlines or ensure each file is consistent

- Indentation (int n>=0 | 'tab' | { value: <>, except: [ 'comments','blankline'] }

- Line length (int n>0 | { value: <>, except: [ 'directives' 'string' 'comments' 'declare-fn' 'declare-class'] })

    Exceptions to the integer value
  - directive : exclude directive lines such as 'import', 'library', 'package', 'part', 'part of', etc.

  - string : lines ending in Strings, may include terminating semi-colons

  - comments

  - declare fn : function declarations

  - declare class : class declarations

- Line limit per file (int n >0)

- Context Keyword (String | List< String>)

   Assignment of `this` is limited to specific variable names

- Require Template String (bool | {except: ['string']}

    Enforce use of string templates
 - except when concatenating 2 strings literals

- Trailing Comma required (bool)
   for objects and arrays

- Trailing White Space allowed (bool)

- Multiple consecutive non-indent spaces allowed (int n)

- Mixed whitespace spaces and tabs allowed (bool)

- Multiple consecutive Endlines allowed (int n)

- Space inside parenthesis (bool | {except : ['nested', 'function'] })

   may require differentiation based on type of parenthesis?

     - function call arguments

     - function definition parameters

     - conditional/logical expressions

     - mathematical/bitwise expressions

- Space inside brackets (bool | {except : ['nested', '(', ')', 'function'] })

    may require differentiation based on type of brackets?
  - Array declaration

  - property Accessor

- Space inside braces (bool |  {except : ['nested', '(', ')'] })

- Space before comma (bool)

- Commas precede linebreaks when wrapped (bool)

- Require space before any comma

- New line at EOF (bool)

- Curly braces for single statements (bool | {except : [if else for while try catch case])

- Yoda Conditions (bool) ?

- Var Declarations on top ?
   May be irrelevant since Dart does not hoist variables. could still be a nice style to follow