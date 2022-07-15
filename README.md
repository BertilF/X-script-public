# X-script-public
Public part of X-script programming language
## X-script programming language
X-script is a programming language. The language is implemented in the file x.exe.  
The code is in one or more files with the extension .x.  
You can also write code directly in the X-window that opens when you start x.  
An x-command has the syntax <name arg1,arg2,...> or \<name>. 

Examples:  
\<date> - to return the current date.  
\<wcons hello world.> - to write "Hello world." to the X-window.  
\<help> - to see a list of existing commands.  
\<help (name)> -  to show help information for a specific command.

## States
Besides commands, there are also a format that is very convenient for handling streams of data, either from files or from connections. This format is called states. A state has the following format:

name  
\----

!"(preaction"!

(alternatives: ...)  
?"(input)"?  
!"(output)"!  
...

!"(postaction"!

A state is a list of input/output pairs, specifying what shall happen for each kind of input.
A state also has a preaction, that is executed when it is called, and a post action, that is executed when it is returned from


## Types
Everything in X is strings. The only variations to this is that there are plain strings,
created with <var $name>, arrays of strings created with <var $name[]> and
files.

Files can be loaded from the disk and stored to the disk.  
Files can also be double directed tcp/ip connections or serial connections.

Files can be opened as binary, in which case they will be visible in hexadesimal format instead of character format. 
