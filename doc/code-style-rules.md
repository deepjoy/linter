General
=======
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

Statement Specific
==================
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

 
Directives
==========
- Group directives ( bool | {except: [import, library, package, part, part of, ...]})

- Directives on top (bool)

- Directives Order ( asc | dec | nat-asc | nat-dec )

- Newline before each directive type ( bool | all | [import, library, package, part, part of, ...] | {value: <>,except : ['first']);

Variable Declarations
=====================
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
 

Comments
========

- LineComment
  - Starts with space (bool)

  - NewLine Before (bool | except :[first])

- First character should be capitalized

Keywords
========
- Space before keywords (all | [])

   e.g ```else, while, catch, case```

- Space after keywords(all | [])

   e.g. ```do, for, if, else, switch, case, try, catch, void, while, return, function```

- NewLine before keywords (all | [])

   e.g. ```do, for, if, else```

Arrays
======
 - Elements on new line (int n=0 | bool  | overflow)
   enforce array elements are wrapped.
   allow arrays of upto (n) elements on a single line without wrapping

 - Square brackets on separate line ( none | both | start | end)
   enforce that the square brackets in array declarations are on their own 
   new line


Maps/Objects
============
- Object Key Order ( asc | dec | nat-asc | nat-dec )
    enforces that keys in object declarations are ordered

- Each key on new line (bool)

- Require space
  - before value

  - after key

- Require aligned values (bool, except (function, afterbreak)

- Allow linebreaks (int n>-1)

- Curly braces on separate line (none | both | start | end)

   Enforce that the curly braces in Object declarations are on their own new line

Execution Blocks
================
 - Curly braces on separate line (none | both | start | end | { value <>, except : [ conditional ,  functionarg ])

   Enforce that the curly braces in execution block are on their own new line. possible exceptions
  - `conditionals` : e.g. ``` if (true) { print 'hello';}; ```

  - `functionarg` : e.g. ``` foobar(() => { ... }); ```

 - Require newline before block (bool | {except: [first]})

 - Require newline after block (bool | {except: last, function call, constructor call, array element, object value})

 - EmptyBlocksAllowed (bool)

Function Call Arguments
========================
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



Function Declaration
====================
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

     ```var a = function () {}```

  - `declare` : require all named functions in executable code blocks to be of the type

     ```function a() {}```


