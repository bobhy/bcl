# bcl
Bob's Command Language, a portable command language interpreter

The project is entirely conceptual at the moment, there is no usable code at the moment.
But contributors are welcome! See [CONTRIBUTING](./CONTRIBUTING)

It is influenced by many predecessors and lots of good thinking that went into [J[E]CL](https://en.wikipedia.org/wiki/Job_Control_Language#Job_Entry_Control_Language) ([DCL](https://en.wikipedia.org/wiki/DIGITAL_Command_Language)), [bash](https://git.savannah.gnu.org/cgit/bash.git/), [powershell](https://github.com/PowerShell/PowerShell) [xonsh](https://github.com/xonsh/xonsh) and [nushell](https://github.com/nushell/nushell).

BCL also provides some new innovations: 
* A departure from the VERB-NOUN imperative style championed by DCL and Powershell.  In BCL, the style is more NOUN-VERB, but the NOUN can sometimes be elided.
* A simplification of command line syntax by restricting most scripting language constructs to function definitions.  In theory, this makes composing a command line a much more intuitive effort without significant reduction in CLI capability. [^1]

[^1]: Note the distinction between "command line" and "command language", it's pervasive in this project.

I am not sure that any of the above considerations mean that BCL couldn't fairly be called a "shell".
