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

* [9p2000 RFC (wip)](https://github.com/ericvh/9p-rfc) - WIP drafting of a 9p2000 (and friends) RFC document
* [Writing a 9p server from scratch](https://blog.aqwari.net/9p/) - Three post series on implementing 9p file servers in Go
* [Linux's v9fs 9p2000.L documentation](https://www.kernel.org/doc/Documentation/filesystems/9p.txt)

## Libraries

*Libraries which provide some kind of 9p functionality.*

### C

* []() - 

### Go

* [styx](https://github.com/droyo/styx) - Droyo's library focusing on servers
* [go-p9p](https://github.com/docker/go-p9p) - Docker's performant 9p library

## Servers

*Operational 9p file servers.*

### Learning

*9p file servers created to assist in understanding how to write 9p file servers as a beginner.*

* [jsonfs](https://github.com/droyo/jsonfs) - JSON as a fs
* [semfs](https://bitbucket.org/henesy/9intro/src/default/ch13/semfs/) - Semaphores as a fs by Nemo
* [asemfs](https://bitbucket.org/henesy/9intro/src/default/ch14/asemfs/) - Semaphores as a fs by Nemo with authentication support
* [rngfs](TODO) - [prng](https://en.wikipedia.org/wiki/Pseudorandom_number_generator) as a fs
* [simplefs](https://bitbucket.org/henesy/simplefs) - Demonstrative fs that's a reduction of the framework shown in semfs by Nemo
* [bankfs](https://bitbucket.org/henesy/bankfs) - Demonstrative fs which features gross abuse of the [9pfile(2)](http://man.cat-v.org/9front/2/9pfile) library

## Clients

*Operational 9p clients.*

* []() - 

## Implementations

*Implementations or derivatives of the 9p protocol.*

* [9p2000.L](https://github.com/torvalds/linux/tree/master/fs/9p) - 9p2000.L Linux kernel module
