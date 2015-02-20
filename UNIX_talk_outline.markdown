# It's a UNIX system: an informal introduction to Unix history and usage

Hello all, sehqlr here, and here is an outline of a lecture to beginning
programmers and technologists that I think will help them in software
development and get a better understanding of computers in general.

## A Bit of Theory

Like all English majors, I'll begin with the Wikipedia definition:
>An operating system is software that manages computer hardware and software
>resources and provides common services for computer programs.

UNIX is a family of operating systems (OS) that began as one OS first invented
for mainframe computers, starting in 1969.
It is a platform from which many other technologies have been created,
and it has been the workbench of many programmers past and present.

Elements defined by the OS
* Memory
* Storage
* Installing New Programs
* Updating Old Programs
* Security
* Administration
* Device Drivers for Input/Output (I/O)
* And, it helps you fight velociraptors
[It's a UNIX system!](http://randar.com/post/92394210860/its-a-unix-system-i-know-this-jurassic-park)

*Here's where I tell a story at my family's expense*

## A Brief History

#### pre-UNIX OS

0. Early Hardware: toggles and knobs, paper tape and punch cards (and magnets!)
  0. ![Altair 8800](http://en.wikipedia.org/wiki/Altair_8800#mediaviewer/File:Altair_8800_at_the_Computer_History_Museum,_cropped.jpg)
  1. ![Colossus](http://en.wikipedia.org/wiki/Colossus_computer#mediaviewer/File:Colossus.jpg)
  2. ![Paper tape](http://en.wikipedia.org/wiki/Punched_tape#mediaviewer/File:Dg-papertapes.jpg)
  3. ![Punch cards](http://en.wikipedia.org/wiki/Punched_card#mediaviewer/File:IBM1130CopyCard.agr.jpg)
  4. ![Teletypewriters (TTY)](http://heritageinmaine.blogspot.com/2011/10/not-hearing-history-at-governor-baxter.html)
1. Resource management and automation leads to OS technology
  0. Computers got faster and important, so 'moniter' programs were written
  1. Multiple programmers lead to time-sharing issues, especially after TTY
  2. Machine -> Low Level -> High Level
  3. OS just a combo of earlier innovations bundled together

#### UNIX, C, and \*nix systems

![UNIX licence plate](http://en.wikipedia.org/wiki/Live_Free_or_Die#mediaviewer/File:Actual_DEC_UNIX_License_Plate_DSC_0317.jpg)

An amusing photo:
[Dennis Ritchie & Ken Thompson](http://cm.bell-labs.com/cm/cs/who/dmr/picture.html)

Highlights from [DMR's UNIX Notes](http://cm.bell-labs.com/cm/cs/who/dmr/notes.html)

0. UNIX
  0. Bell Labs R&D project
  1. Implemented in assembly, 1969 - 1971
  2. Reimplemented in C, 1971 – 1973
1. C programming language
  0. Imperative/procedural paradigm
  1. Text-based source, compiled to many different assemblies
  2. The language evolved with UNIX, made it portable and shareable
2. \*nixes: BSD, Linux, and OS X
  0. ![BSD](http://en.wikipedia.org/wiki/File:Bsd_daemon.jpg#mediaviewer/File:Bsd_daemon.jpg)
  1. ![Darwin (OS X)](http://en.wikipedia.org/wiki/File:Hexley_the_Platypus.svg#mediaviewer/File:Hexley_the_Platypus.svg)
  2. ![Linux](http://commons.wikimedia.org/wiki/File:Tux.svg#mediaviewer/File:Tux.svg)
  3. ![GNU](http://en.wikipedia.org/wiki/File:Heckert_GNU_white.svg#mediaviewer/File:Heckert_GNU_white.svg)

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
