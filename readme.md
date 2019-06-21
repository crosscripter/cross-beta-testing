# Cross Beta Testing

This repository is for tracking the issues, code and files used during the
Cross beta testing program.  Please log any issues or commit any files to
this repository.

Questions, comments or suggestions?
Email me at <a href="mailto:crosscripter@gmail.com">crosscripter@gmail.com</a>


# Known Issues

## Shell

### Repl
- Deleted character buffer off by one issue (only some host shells)
- Syntax highlight overlapping, (ie. keywords in comments, numbers in strings etc.)
- Auto indent doubles exponentially on blank input (maybe only on some host shells?)

### Electron Shell
- Clear screen hides prompt
- Missing headers / blank screen on start
- Electron (Linux) Style rendering issues

## Compiler

### Lexer 

### Parser
- Scope tracking and definition mapping
- Indent level errors on blank lines within blocks
- Contextual keywords (ie. fun next(), class use, exit = 1 etc.)
- Child branches should NOT be parsed as blocks (ie. elif x == 3: ..., of 3: log(3) etc.)
- Module resolution order when parsing imports (ie. use a, (in a) use b, (in b) use c, etc.)

### Compiler
- Add distinction between functions and method code generation (ie. fun a(), class A: fun a(): ...)
- Add distinction between local and block/this scoped variables (ie. x = 3, this.x = 3 etc.)


# Suggestions

## Language Design
- Ben - Change the keyword `fun` to `func`

## Website
- Matthew - Add secure sign up beta testing form/application instead of email
