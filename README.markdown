The __UNDEFINED__ morphology and tools
==========================================

This repository contains source files for the __UNDEFINED__ language morphology
and dictionary. The data and implementation are licenced under __LICENCE__
licence, also detailed in the
[LICENCE](https://github.com/giellalt/lang-__UND__/blob/develop/LICENCE). The
authors named in the AUTHORS file are available to grant other licencing
choices.

[![GitHub issues](https://img.shields.io/github/issues-raw/giellalt/lang-__UND__)](https://github.com/giellalt/lang-__UND__/issues)
 [![Build Status](https://github.com/giellalt/lang-__UND__/workflows/Build%20Speller%20Archives%20and%20Bundles/badge.svg)](https://github.com/giellalt/lang-__UND__/actions)


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

Apertium wiki has good instructions on how to [install the dependencies for Mac
OS X](https://wiki.apertium.org/wiki/Apertium_on_Mac_OS_X) and how to [install
the dependencies on
linux](https://wiki.apertium.org/wiki/Installation_of_grammar_libraries)

Or just copy/paste this into your Terminal on **Mac OS X**:

```
curl https://apertium.projectjj.com/osx/install-nightly.sh | sudo bash
```

or terminal on **Ubuntu, Debian or Windows Subsystem for Linux**:

```
wget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash
sudo apt-get install cg3 hfst
```

Downloading
-----------

The __UNDEFINED__ language sources can be acquired from [github
repository](https://github.com/giellalt/lang-__UND__/). The [core utilities
repository](https://github.com/giellalt/giella-core/) needs to be downloaded and
initial setup performed first.

```
git clone https://github.com/giella-core
git clone https://github.com/giellalt/lang-__UND__
```

Installation
------------

[INSTALL](https://github.com/giellalt/lang-__UND__/blob/develop/INSTALL)
describes the GNU build system in detail, but for most users the usual:

```
./autogen.sh
./configure
make
(as root) make install
```

should result in a local installation.  For more details about the autotools
build system as it is used in the giellalt repository, please refer to
https://giellalt.uit.no/infra/Infrastructure.html.
