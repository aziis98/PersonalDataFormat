# PersonalDataFormat
In this repo I describe my personal format for storing data

There is also a EBNF file in this repo with the full definition of the format.

# The Format

A file is a **Document**, a **Document** is made up of **Expressions**.

An **Expression** generally is ended by a new line or by a closing character (this second type will be covered later) or by a `;`.

An **Expression** is a sequence of **Value**s separated by a series of white spaces.

A **Value** can be a **Symbol**, a **Number**, a **String** or a **List**.

## Values

A **Symbol** is a sequence of non spaced alphanumeric characters with the inclusion of `-` and `_`.

A **Number** can be an **Integer** or a **Decimal**.

An **Integer** is a sequence of digits.

A **Decimal** is a sequence of at least one digit followed by a `.` and another sequence of least one digit.

A **String** is a sequence of any char delimited by quotes.

### Examples

    a-symbol

    1000

    3.1415

    "A String"
 
## Lists

A **List** is a **Value** delimited by curly braces (`{` and `}`) and can contain one or more expressions separeted by new lines (as sad before) or by ";".

### Examples

An expression composed of a symbol and a list, the list contains three expression that are in this case a single integer value.

    my-list { 1 ; 2 ; 3 } 
  
This list instead contains only one expression composed of three integer values. 

    my-list { 1 2 3 }
 
# Conclusion
 
TODO
 
 
 
 
 
 
 
 
