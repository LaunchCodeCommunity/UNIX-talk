# It's a UNIX system: an informal introduction to Unix history and usage

Hello all, sehqlr here, and here is an outline of a lecture to beginning
programmers and technologists that I think will help them in software
development and get a better understanding of computers in general.

## A Bit of Theory

I'm going to begin by asking myself a few, easily answered questions, then
conveniently answering them.

1. What is this lecture about?

This lecture is about UNIX, argueably one of the most important technologies
from the 20th century; one that has greatly shaped the 21st. More specifically,
it is a platform from which many other technologies have been created,
and it has been the workbench of many programmers past and present.

2. OK, but what is UNIX?

[Well, It helps you fight velociraptors](//randar.com
/post/92394210860/its-a-unix-system-i-know-this-jurassic-park)

UNIX is a family of operating systems (OS) that began as one OS first invented
for mainframe computers, starting in 1969.

3. OK, but what is an Operating System?

Like all English majors, we begin with the Wikipedia definition:
>An operating system is software that manages computer hardware and software
>resources and provides common services for computer programs.

Elements defined by the OS
* Input
* Output
* Memory
* Storage
* Installing New Programs
* Updating Old Ones
* Security
* Administration
* Device Drivers
* etc

#### A story at my family's expense

#### Thesis
The what, the history, and the why of OS
UNIX's influence and pervasiveness (INTERNET)
Why it matters to me

## A Brief History

#### pre-UNIX OS

1. Early Hardware: toggles and knobs, paper tape and punch cards (and magnets!)
  1. [Altair 8800](//en.wikipedia.org/wiki/Altair_8800
     #mediaviewer/File:Altair_8800_at_the_Computer_History_Museum,_cropped.jpg)
  2. [Colossus](https://en.wikipedia.org/wiki/Colossus_computer
     #mediaviewer/File:Colossus.jpg)
  3. [Paper tape](https://en.wikipedia.org/wiki/Punched_tape
     #mediaviewer/File:Dg-papertapes.jpg)
  4. [Punch cards](//en.wikipedia.org/wiki/Punched_card
     #mediaviewer/File:IBM1130CopyCard.agr.jpg)
  5. [Teletypewriters (TTY)](//heritageinmaine.blogspot.com/2011/10/
     not-hearing-history-at-governor-baxter.html)
2. Resource management and automation leads to OS technology
  1. Computers got faster and important, so 'moniter' programs were written
  2. Multiple programmers lead to time-sharing issues, especially after TTY
  3. Machine -> Low Level -> High Level
  4. OS just a combo of earlier innovations bundled together

#### UNIX, C, and \*nix systems

[UNIX licence plate](//en.wikipedia.org/wiki/Live_Free_or_Die#mediaviewer/
File:Actual_DEC_UNIX_License_Plate_DSC_0317.jpg)

An amusing photo:
[Dennis Ritchie & Ken Thompson](//cm.bell-labs.com/cm/cs/who/dmr/picture.html)

Highlights from [DMR's UNIX Notes](//cm.bell-labs.com/cm/cs/who/dmr/notes.html)

1. UNIX
  1. Bell Labs R&D project
  2. Implemented in assembly, 1969 - 1971
  3. Reimplemented in C, 1971 – 1973
2. C programming language
  1. Imperative/procedural paradigm
  2. Text-based source, compiled to many different assemblies
  3. The language evolved with UNIX, made it portable and shareable
3. \*nixes: BSD, Linux, and OS X
  1. [BSD](en.wikipedia.org/wiki/File:Bsd_daemon.jpg
     #mediaviewer/File:Bsd_daemon.jpg)
  2. [Darwin (OS X)](//en.wikipedia.org/wiki/File:Hexley_the_Platypus.svg
     #mediaviewer/File:Hexley_the_Platypus.svg)
  3. [Linux](//commons.wikimedia.org/wiki/File:Tux.svg
     #mediaviewer/File:Tux.svg)
  4. [GNU](//en.wikipedia.org/wiki/File:Heckert_GNU_white.svg
     #mediaviewer/File:Heckert_GNU_white.svg)

## Usage: the almighty Terminal

#### GUI versus TUI

There exists a continuum of different user interfaces (UI)
but for simplicity's sake, we'll use to categories: GUI and TUI

1. Graphical User Interface (GUI)
  1. This is how most people use computers
  2. most of the OS details are hidden
  3. Takes UI/UX design, and is easy to get wrong and follow fads
  4. Instructions rely on spatial descriptions or screenshots
2. Text-based User Interfaces
  1. Geared towards knowledgeable 'power users'
  2. Reveals many more details, sometimes badly
  3. No UI/UX design, unless you use ASCII art
  4. Instructions can be literally copy & pasted, even downloaded

Text-based tools are preferred for many use cases. GUI-based macros
can be used sometimes, but they are often translated into text!
[Selenium]

#### Getting to know the terminal

Cheat sheets and muscle memory, and tab completion and arrow keys!

0. Command Prompt
  0. CONTROL C
  1. Learning the commands (echo, cat, and touch)
    1. Using it... sometimes
    2. --help (-h)
    3. man (and info)
    4. whereis (helps find docs on computer)
  2. ENV variables
    0. . and ..
    1. $HOME
    2. $?
    3. $PATH
1. Navigating
  1. ls (LIST)
  2. cd (CHANGE DIRECTORY)
  3. tree (if you can install it)
  4. find & grep
  5. history
    1. history
    2. history | grep "search"
    2. <C-R> "search"
    3. !!
3. I/O, redirection, and piping
  1. STDIN, STDOUT, STDERR
  2. Directing STDOUT/STDERR into file
  3. Directing file into STDIN
  4. Piping
5. Peek at advanced stuff
  1. .bashrc
