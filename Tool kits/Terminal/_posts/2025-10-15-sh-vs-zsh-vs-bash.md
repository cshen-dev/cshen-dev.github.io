---
layout: post
title: "💻 sh vs Zsh vs Bash Built-in Commands Comparison"
---


This table compares the built-in commands available in the original Bourne Shell (sh), Z Shell (Zsh), and Bourne Again Shell (Bash). Commands are organized alphabetically with notes on key differences.

| Command       | sh      | Bash | Zsh | Notes                                                      |
| ------------- | ------- | ---- | --- | ---------------------------------------------------------- |
| `.` (dot)     | ✓       | ✓    | ✓   | Sources a script file                                      |
| `:` (colon)   | ✓       | ✓    | ✓   | Null command (does nothing but returns success)            |
| `[`           | ✓       | ✓    | ✓   | Condition evaluation (alias for test)                      |
| `alias`       | Limited | ✓    | ✓   | Create command aliases; limited in original sh             |
| `autoload`    | ✗       | ✗    | ✓   | Zsh-specific: load functions on demand                     |
| `bg`          | ✓       | ✓    | ✓   | Resume jobs in the background                              |
| `bind`        | ✗       | ✓    | ✗   | Bash-specific: display or set readline key bindings        |
| `bindkey`     | ✗       | ✗    | ✓   | Zsh-specific: display or set key bindings                  |
| `break`       | ✓       | ✓    | ✓   | Exit from loops                                            |
| `builtin`     | ✗       | ✓    | ✓   | Execute built-in commands directly                         |
| `caller`      | ✗       | ✓    | ✗   | Bash-specific: return context of subroutine call           |
| `cd`          | ✓       | ✓    | ✓   | Change directory                                           |
| `command`     | ✓       | ✓    | ✓   | Execute command bypassing any aliases                      |
| `compdef`     | ✗       | ✗    | ✓   | Zsh-specific: define completion functions                  |
| `compgen`     | ✗       | ✓    | ✗   | Bash-specific: generate possible completions               |
| `complete`    | ✗       | ✓    | ✗   | Bash-specific: specify how to complete arguments           |
| `compopt`     | ✗       | ✓    | ✗   | Bash-specific: modify completion options                   |
| `compsys`     | ✗       | ✗    | ✓   | Zsh-specific: completion system initialization             |
| `continue`    | ✓       | ✓    | ✓   | Skip to next iteration of a loop                           |
| `declare`     | ✗       | ✓    | ✓   | Declare variables with attributes                          |
| `dirs`        | ✗       | ✓    | ✓   | Display directory stack                                    |
| `disown`      | ✗       | ✓    | ✓   | Remove jobs from current shell                             |
| `echo`        | ✓       | ✓    | ✓   | Display arguments as text                                  |
| `enable`      | ✗       | ✓    | ✗   | Bash-specific: enable/disable shell built-ins              |
| `eval`        | ✓       | ✓    | ✓   | Evaluate arguments as shell commands                       |
| `exec`        | ✓       | ✓    | ✓   | Replace current process with specified command             |
| `exit`        | ✓       | ✓    | ✓   | Exit the shell                                             |
| `export`      | ✓       | ✓    | ✓   | Set environment variables                                  |
| `false`       | ✓       | ✓    | ✓   | Return a failure status                                    |
| `fc`          | ✗       | ✓    | ✓   | Fix command (history editing)                              |
| `fg`          | ✓       | ✓    | ✓   | Resume job in foreground                                   |
| `float`       | ✗       | ✗    | ✓   | Zsh-specific: declare floating-point variables             |
| `function`    | ✗       | ✓    | ✓   | Define a function (sh uses different syntax)               |
| `getopts`     | ✓       | ✓    | ✓   | Process command-line options                               |
| `hash`        | ✓       | ✓    | ✓   | Remember command locations                                 |
| `help`        | ✗       | ✓    | ✗   | Bash-specific: display help for built-ins                  |
| `history`     | ✗       | ✓    | ✓   | Display command history                                    |
| `if`          | ✓       | ✓    | ✓   | Conditional statement                                      |
| `integer`     | ✗       | ✗    | ✓   | Zsh-specific: declare integer variables                    |
| `jobs`        | ✓       | ✓    | ✓   | List active jobs                                           |
| `kill`        | ✓       | ✓    | ✓   | Send signals to processes                                  |
| `let`         | ✗       | ✓    | ✓   | Evaluate arithmetic expressions                            |
| `local`       | ✗       | ✓    | ✓   | Declare local variables                                    |
| `logout`      | ✗       | ✓    | ✓   | Exit a login shell                                         |
| `mapfile`     | ✗       | ✓    | ✗   | Bash-specific: read lines into array variable              |
| `popd`        | ✗       | ✓    | ✓   | Remove directories from directory stack                    |
| `print`       | ✗       | ✗    | ✓   | Zsh-specific: more versatile version of echo               |
| `printf`      | ✗       | ✓    | ✓   | Format and print data                                      |
| `pushd`       | ✗       | ✓    | ✓   | Add directories to directory stack                         |
| `pwd`         | ✓       | ✓    | ✓   | Print working directory                                    |
| `read`        | ✓       | ✓    | ✓   | Read from stdin into variables                             |
| `readarray`   | ✗       | ✓    | ✗   | Bash-specific: read lines into array variable              |
| `readonly`    | ✓       | ✓    | ✓   | Mark variables as read-only                                |
| `rehash`      | ✗       | ✗    | ✓   | Zsh-specific: rebuild command hash table                   |
| `return`      | ✓       | ✓    | ✓   | Return from a function                                     |
| `set`         | ✓       | ✓    | ✓   | Set/unset shell options and positional parameters          |
| `setopt`      | ✗       | ✗    | ✓   | Zsh-specific: set shell options                            |
| `shift`       | ✓       | ✓    | ✓   | Shift positional parameters                                |
| `shopt`       | ✗       | ✓    | ✗   | Bash-specific: set/unset shell options                     |
| `source`      | ✗       | ✓    | ✓   | Execute commands from file (sh only has `.`)               |
| `suspend`     | ✗       | ✓    | ✓   | Suspend shell execution                                    |
| `test`        | ✓       | ✓    | ✓   | Evaluate conditional expression                            |
| `times`       | ✓       | ✓    | ✓   | Display process times                                      |
| `trap`        | ✓       | ✓    | ✓   | Trap signals and events                                    |
| `true`        | ✓       | ✓    | ✓   | Return a successful status                                 |
| `type`        | ✓       | ✓    | ✓   | Display command type                                       |
| `typeset`     | ✗       | ✓    | ✓   | Declare variables and their attributes                     |
| `ulimit`      | ✓       | ✓    | ✓   | Set resource limits                                        |
| `umask`       | ✓       | ✓    | ✓   | Set file creation mask                                     |
| `unalias`     | Limited | ✓    | ✓   | Remove command aliases                                     |
| `unfunction`  | ✗       | ✗    | ✓   | Zsh-specific: remove function definitions                  |
| `unhash`      | ✗       | ✗    | ✓   | Zsh-specific: remove command from hash table               |
| `unset`       | ✓       | ✓    | ✓   | Remove variables or functions                              |
| `unsetopt`    | ✗       | ✗    | ✓   | Zsh-specific: unset shell options                          |
| `wait`        | ✓       | ✓    | ✓   | Wait for job completion                                    |
| `whence`      | ✗       | ✗    | ✓   | Zsh-specific: describe command (similar to type)           |
| `which`       | ✗       | ✗    | ✓   | Zsh-specific: locate command                               |
| `zcompile`    | ✗       | ✗    | ✓   | Zsh-specific: compile functions/scripts for faster loading |
| `zformat`     | ✗       | ✗    | ✓   | Zsh-specific: format strings                               |
| `zle`         | ✗       | ✗    | ✓   | Zsh-specific: zsh line editor commands                     |
| `zmodload`    | ✗       | ✗    | ✓   | Zsh-specific: load zsh modules                             |
| `zparseopts`  | ✗       | ✗    | ✓   | Zsh-specific: parse options                                |
| `zpty`        | ✗       | ✗    | ✓   | Zsh-specific: pseudo terminal handling                     |
| `zregexparse` | ✗       | ✗    | ✓   | Zsh-specific: parsing based on regular expressions         |
| `zstyle`      | ✗       | ✗    | ✓   | Zsh-specific: set style for completion system              |

## Shell Evolution and Feature Comparison

### Bourne Shell (sh)

The original Unix shell developed by Stephen Bourne at Bell Labs in 1979:

- Minimalist design with essential shell functionality
- Focus on scripting rather than interactive use
- Limited job control
- No command history
- No command line editing
- Basic built-in commands only
- POSIX-compliant (original reference implementation)

### Bash (Bourne Again Shell)

Developed by Brian Fox for the GNU Project in 1989:

- Direct extension of the Bourne shell
- Strong focus on POSIX compliance
- Enhanced scripting capabilities
- Command history and editing
- Job control
- Programmable completion
- Array support
- More advanced parameter expansion

### Zsh (Z Shell)

Developed by Paul Falstad in 1990:

- Extended feature set beyond Bash
- Modular design with loadable modules
- Highly customizable
- Advanced pattern matching and globbing
- Theming capabilities
- Spelling correction
- Sophisticated tab completion system
- Floating point arithmetic
- More extensive string handling
- Better interactive features

## Key Functional Differences

1. **Core Commands**:
   - **sh**: Provides minimalist but essential commands
   - **Bash**: Extends sh with interactive features
   - **Zsh**: Further extends with advanced customization
2. **Variable Handling**:
   - **sh**: Basic variable support
   - **Bash**: Added arrays and better variable manipulation
   - **Zsh**: Added specialized variable types (integer, float)
3. **Command Completion**:
   - **sh**: None or minimal
   - **Bash**: Programmable completion system
   - **Zsh**: Advanced, context-aware completion system
4. **Scripting Capabilities**:
   - **sh**: Basic scripting support
   - **Bash**: Enhanced scripting with more built-ins
   - **Zsh**: Most extensive scripting capabilities