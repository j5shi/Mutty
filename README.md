# Mutty 

![Mutty](http://i.imgur.com/ZMpvcNH.png)

Mutty is a [Cygwin](http://cygwin.com) Terminal emulator with tabs. It is useful for Windows and
Cygwin users who want a powerful terminal.

Mutty is based on [mintty](https://github.com/mintty/mintty). The main difference to mintty is that
you can run multiple session in single window using tabs.

* Most features from mintty should work
- To create new tabs: `Ctrl + Shift + T`
- To close the current tab: `Ctrl + Shift + W`
- To switch to the left tab: `Ctrl + Shift + A`
- To switch to the right tab: `Ctrl + Shift + D`

If you find bugs (there are probably many), you may report them on Github or send pull requests

## Installation

Building MuTTY requires recent version of gcc and g++ for Cygwin. It can not be built with a MinGW
compiler, because it relies on some Unix facilities that are not available on plain Windows, in
particular pseudo terminal devices (ptys).

Prerequisites for Cygwin:

* gcc
* g++
* make
* w32api-headers
* git

Then, in Cygwin terminal run following commands:

    git clone https://github.com/j5shi/Mutty.git
    cd Mutty 
    make 
    cp src/mutty.exe /bin

You can then try running it by typing `mutty`.



