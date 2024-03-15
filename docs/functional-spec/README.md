The as-planned spec for BCL.

Called "functional" because it focuses on capabilities and key interfaces, not on design.

However, since we're talking about a language, this spec shall include lots of examples of exact syntax, maybe also a complete grammar.  These are not design details, they are key functional interfaces.

Borrowing an outline that lived in my fingertips while at Microsoft:

1. Goals and Non-Goals
2. Assumptions, Environments
3. Key Concepts and Features
4. Open questions  
   Placed at the top of the spec for visibility
   1. Does BCL support "scripts" as anything more than a batch of command language statements? 
      1. if not, should make it easy to wrap a file of statements as a temporary function definition.
5. Interfaces
   1. Language
      1. Types, values
      2. Command language
         1. individual command syntax
            1. noun verb
            2. arguments, switches, values
            3. help
         2. pipelines of individual commands
         3. error handling
         4. table processing commands
         5. temporary environment override 
      3. Function definition
         1. type definitions for input, parameters, output
         2. Scripting language (only available in functions, not at command line)
            1. variables
            2. flow control (incl error handling)
            3. 
   2. Built-in commands and APIs  
        These are callable from elsewhere in the code, but also packaged as "commands" that can be invoked from functions or command line.
      1. History
      2. Completions
      3. OS environment
      4. ...
   3. Interactive Terminal
      1. Command line editing
      2. Formatted, colored output
   4. Wrapping native process (and executable)
      1. constructing captive stdin
      2. command invocation, arguments ...
      3. postprocessing stdout and stderr, error detection
   5. Standard suite of commands