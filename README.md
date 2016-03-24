# Ubuntu Developer Docker Image

Ubuntu latest version with SSH & other development libraries support.

## Libraries installed

 - Debian Build Packages
 - Network Time Protocol
 - Mercurial SVN
 - Bazaar SVN
 - GNU C compiler
 - GNU C++ compiler
 - GNU Make
 - GNU assembler, linker and binary utilities
 - YACC-compatible parser generator
 - AXEL - light download accelerator - console version
 - dos2unix
 - Python 2.7.x
 - Node.js 5.x
 - NPM with following packages,
	 - Grunt
	 - CoffeeScript
	 - Bower
	 - Forever
	 - PM2

## Installation
```
$ docker build -t ahirmayur/ubuntu-dev .
$ docker run -d -p 22 ahirmayur/ubuntu-dev
5f1b7a6404c8

$ docker port 5f1b7a6404c8 22
0.0.0.0:32771

$ ssh root@localhost -p 32771 # when promoted for password enter 'root' (without quotes)
```