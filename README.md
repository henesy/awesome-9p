# Awesome 9p

A curated list of awesome 9p(2000)-related documents, libraries, and software

### Contributing

Please do.

PR's welcome for all edits or new projects. 

### Contents

- [Awesome 9p](#awesome-9p)
  - [Resources](#resources)
  - [Libraries](#libraries)
  - [Servers](#servers)
  - [Clients](#clients)
  - [Implementations](#implementations)

## Resources

*Useful documents, blogs, etc. that relate to 9p.*

* [9p2000 RFC (wip)](http://ericvh.github.io/9p-rfc/rfc9p2000.html) - WIP drafting of a 9p2000 (and friends) RFC document
* [9p2000.u RFC (wip)](http://ericvh.github.io/9p-rfc/rfc9p2000.u.html) - WIP drafting of a 9p2000.u RFC document
* [Writing a 9p server from scratch](https://blog.aqwari.net/9p/) - Three post series on implementing 9p file servers in Go
* [Linux's v9fs docs](https://www.kernel.org/doc/Documentation/filesystems/9p.txt) - 9p2000.L documentation
* [The Styx Architecture for Distributed Systems](http://doc.cat-v.org/inferno/4th_edition/styx)
* [Cron as a file system](https://blog.gopheracademy.com/cron-filesystem/)

### Manuals

#### Plan9Port

* [intro(4)](http://man.cat-v.org/p9p/4/intro) - Introduction to writing file servers in Plan9Port
* [9pclient(3)](http://man.cat-v.org/p9p/3/9pclient) - The 9pclient library helps client programs interact with 9P servers
* [post9pservice(3)](http://man.cat-v.org/p9p/3/post9pservice) - Library for posting 9p services for client consumption

#### Plan9

* [intro(5)](http://man.cat-v.org/9front/5/intro) - Introduction to the Plan 9 File Protocol, 9P
* [9p(2)](http://man.cat-v.org/9front/2/9p) - 9p(2) communication library
* [9pfile(2)](http://man.cat-v.org/9front/2/9pfile) - 9pfile(2) library for ease of fs development by wrapping 9p(2)
* [authsrv(6)](http://man.cat-v.org/9front/6/authsrv) - Authentication protocols for 9p2000 connections

## Libraries

*Libraries which provide some kind of 9p functionality.*

### C

* [Plan9 9p(2)](http://code.9front.org/hg/plan9front/file/tip/sys/src/lib9p) - 9front's 9p(2) 
* [Plan9Port 9p(2)](https://github.com/9fans/plan9port/tree/master/src/lib9p) - Plan9Port's 9p(2) 
* [Plan9Port 9pclient(2)](https://github.com/9fans/plan9port/tree/master/src/lib9pclient) - Plan9Port's 9pclient(2)
* [NinePea](https://github.com/echoline/NinePea) - Library for implementing 9p resources on Arduino
* [c9](https://github.com/ftrvxmtrx/c9) - 9p2000 client and server library
* [libixp](https://dl.suckless.org/libs/libixp-0.5.tar.gz) - 9p2000 client and server library based on Plan9's 9p(2)
* [libstyx2](https://github.com/bhgv/listyx2-9p-C-lib-and-plugins) - C/Lua 9p2000 library based on libstyx
* [pi9](https://github.com/Cloudef/pi9) - 9p2000 server library

### C#

* [Sharp9P](https://github.com/dave-tucker/Sharp9P) - 9p2000 library

### Go

* [styx](https://github.com/droyo/styx) - Droyo's library focusing on 9p2000 servers
* [go-p9p](https://github.com/docker/go-p9p) - Docker's performant 9p2000 library
* [go9p](https://github.com/knusbaum/go9p) - 9P2000 implementation in Go
* [ninep](https://github.com/lionkov/ninep) - Package for implementing 9p2000 clients and servers

### Haskell

* [network-ninep](https://github.com/elemir/network-ninep) - 9p2000

### Lua

* [libstyx2](https://github.com/bhgv/listyx2-9p-C-lib-and-plugins) - C/Lua 9p2000 library based on libstyx

### Python

* [space9](https://github.com/cea-hpc/space9) - Simple 9p2000 library 

### Ruby

* [r9p (deprecated)](https://dl.suckless.org/libs/r9p-0.4.tgz) - 9p2000 client implementation for Ruby

### Rust

* [rs9p](https://pfpacket.github.io/rust-9p/rs9p/) - Rust crate for 9p2000.L
* [rust-9p](https://github.com/pfpacket/rust-9p) - Rust library for 9p2000.L

### Scheme

* [chicken-9p](https://github.com/dspearson/chicken-9p) - CHICKEN Scheme library for 9p2000

## Servers

*Operational 9p file servers.*

### C

* [dawfs](https://github.com/ftrvxmtrx/dawfs) - A DAW as a file system

### Go

* [jobd](https://github.com/wkharold/jobd) - Cron as a file system
* [ghfs](https://github.com/sirnewton01/ghfs) - Represent GitHub as a file system

### Plan9

*9p file servers, most likely in Plan9's C dialect, for Plan9.*

* [archfs](http://code.9front.org/hg/plan9front/raw-file/tip/sys/src/cmd/archfs.c) - Mount mkfs(8)-style archive
* [bzfs](http://code.9front.org/hg/plan9front/file/tip/sys/src/cmd/bzfs) - Bunzip2 archives 
* [cdfs](http://code.9front.org/hg/plan9front/file/tip/sys/src/cmd/cdfs) - CD (.iso) 
* [cifs](http://code.9front.org/hg/plan9front/file/tip/sys/src/cmd/cifs) - Mount Microsoft™ SMB/CIFS shares
* [consolefs](http://code.9front.org/hg/plan9front/raw-file/tip/sys/src/cmd/aux/consolefs.c) - Serial console access
* [factotum](http://code.9front.org/hg/plan9front/file/file/sys/src/cmd/auth/factotum) - Authentication agent (key storage)
* [hammer2fs](https://github.com/driusan/hammer2fs) - Implementation of the hammer2 filesystem

TODO - more from intro(4)

### Learning

*9p file servers created to assist in understanding how to write 9p file servers as a beginner.*

* [jsonfs](https://github.com/droyo/jsonfs) - JSON as a fs
* [semfs](https://bitbucket.org/henesy/9intro/src/default/ch13/semfs/) - Semaphores as a fs by Nemo
* [asemfs](https://bitbucket.org/henesy/9intro/src/default/ch14/asemfs/) - Semaphores as a fs by Nemo with authentication support
* [rngfs](TODO) - [prng](https://en.wikipedia.org/wiki/Pseudorandom_number_generator)
* [simplefs](https://bitbucket.org/henesy/simplefs) - Demonstrative fs that's a reduction of the framework shown in semfs by Nemo
* [bankfs](https://bitbucket.org/henesy/bankfs) - Demonstrative fs which features gross abuse of the [9pfile(2)](http://man.cat-v.org/9front/2/9pfile) library
* [ramfs (lib9p)](http://code.9front.org/hg/plan9front/raw-file/973f85a881d0/sys/src/lib9p/ramfs.c) - Not to be confused with ramfs(4)

### Windows

* [ninefs](https://github.com/9nut/ninefs) - A 9p file system for windows using dokan

## Clients

*Operational 9p clients.*

### C

* [9mount](http://sqweek.net/hg/9mount/) - Mount 9p filesystems (no FUSE)
* [9pfuse](https://github.com/aperezdc/9pfuse) - Mount 9p file systems through FUSE
* [9p(1)](https://raw.githubusercontent.com/9fans/plan9port/master/src/cmd/9p.c) - Plan9Port's 9p(1) command for interacting with 9p file systems 

### Python

* [space9](https://github.com/cea-hpc/space9) - Simple 9p2000 client

## Implementations

*Implementations or derivatives of the 9p protocol.*

* [9p2000.L](https://github.com/torvalds/linux/tree/master/fs/9p) - 9p2000.L Linux kernel module
