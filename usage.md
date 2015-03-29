## Usage: the almighty Terminal

#### GUI versus TUI

There exists a continuum of different user interfaces (UI)
but for simplicity's sake, we'll use two categories: GUI and TUI

0. Graphical User Interface (GUI)
  0. This is how most people use computers
  1. most of the OS details are hidden
  2. Takes UI design, and is easy to get wrong and follow fads
  3. Instructions rely on spatial descriptions or screenshots
1. Text-based User Interfaces
  0. Geared towards knowledgeable 'power users'
  1. Reveals many more details, sometimes badly
  2. No UI design, unless you use ASCII art
  3. Instructions can be literally be copied & pasted, even downloaded

Many programming tools are built in a TUI due to these differences

#### Getting to know the terminal

Cheat sheets and muscle memory, and tab completion and arrow keys!

0. Command Prompt
  0. CONTROL C
  1. Learning the commands (`echo`, `cat`, and `touch`)
    0. Using it... sometimes
    1. `--help` (`-h`)
    2. `man` (and `info`)
    3. `whereis` (helps find docs on computer sometimes)
  2. ENV variables
    0. `.` and `..`
    1. `$HOME` and `~`
    2. `$?`
    3. `$PATH`
1. Navigating
  1. `ls` (LIST)
  2. `cd` (CHANGE DIRECTORY)
  3. `tree` (if you can install it)
  4. `find`
  5. `grep`
  6. `history`
    0. `history`
    1. `!!`, `!n`, `!-n`
    2. `history | grep "search"`
    3. `<Ctrl+R> "search"`
2. Users, Groups, and Permissions (briefly)
3. I/O, redirection, and piping
  0. `STDIN`, `STDOUT`, `STDERR`
  1. Redirection
    0. Read `<`
    1. Write `>`
    2. Append `>>`
  1. Piping
    0. `|`
    1. A different kind of redirect
    2. Chaining commands together
      0. Example from the `history` section
      1. `find ~ -name UNIX_talk_outline.markdown | xargs grep -n "UNIX_talk"`
4. A look at my `.bashrc`

## Questions

This talk is still a work in progress, and I'm always open for suggestions
and constructive criticism. I'm going to make this a full repository soon,
so stay tuned!
