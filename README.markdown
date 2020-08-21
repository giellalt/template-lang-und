The __UNDEFINED__ morphology and tools
==========================================

This repository contains source files for the __UNDEFINED__ language
morphology and dictionary. The data and implementation are licenced
under __LICENCE__ licence, also detailed in the [LICENCE](https://github.com/giellalt/lang-__UND__/blob/develop/LICENCE). The authors named
 in the AUTHORS file are available to grant other licencing choices.




External documentation
----------------------

Some documentation can be found at:

-   <http://giellatekno.uit.no/__UND__doc/index.html>
-   <https://giellalt.uit.no/tools/docu-__UND__-manual.html>
-   <https://giellalt.uit.no/index.html>

Dependencies
------------

In order to compile and use __UNDEFINED__ language morphology and
dictionaries, you need:

- Xerox Finite-State Morphology tools, or
- Helsinki Finite-State Technology library and tools, version 3.8 or
  newer, or
- Foma finite-state tool

Optionally:

- VislCG3 Constraint Grammar tools

One way to install these dependencies is described in [apertium
wiki](https://wiki.apertium.org/wiki/Installation_of_grammar_libraries)

Downloading
-----------

The __UNDEFINED__ language sources can be acquired from [gthub
repository](https://github.com/giellalt/lang-__UND__/). The [core utilities
repository](https://github.com/giellalt/giella-cor/) needs to be downloaded and
initial setup performed first.

Installation
------------

[INSTALL](https://github.com/giellalt/lang-__UND__/blob/develop/INSTALL)
describes the GNU build system in detail, but for most users the usual:

```
./configure
make
(as root) make install
```

should result in a local installation and:

```
 (as root) make uninstall
```

in its uninstallation.

If you would rather install in e.g. your home directory (or aren\'t the
system administrator), you can tell ./configure:

```
 ./configure --prefix=$HOME
```

If you are checking out the development versions from github, you must first
create and install the necessary autotools files from the host system,
and check that your environment is correctly set up. This is done by
doing:

```
./autogen.sh
```

It is common practice to keep [generated files out of version
control](http://www.gnu.org/software/automake/manual/automake.html#CVS).

VPATH builds
------------

If you want to keep the source code tree clean, a VPATH build is the
solution. The idea is to create a build dir somewhere outside of the
source code tree, and call [configure]{.title-ref} from there. Here is
one VPATH variant of the standard procedure:

```
mkdir build && cd build
../configure
make
(as root) make install
```
This will keep all the generated files within the build/ dir, and keep
the src/ dir (mostly) free of generated files. If you are building from
the development version in git, you must run the ./autogen.sh script
BEFORE you take the steps above.

For further installation instruction refer to file
[INSTALL](https://github.com/giellalt/lang-__UND__/blob/develop/INSTALL), which
contains the standard installation instructions for GNU autoconf based software.
