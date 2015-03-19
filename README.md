Toccata
=======

A Clojure-inspired Lisp dialect that compiles to native executable using the Clang compiler

This is very much WFM code. Not suitable for any useful purpose.

You can learn more about Toccata by following the [blog here](http://toccata.io)

Quick Start
===========

Make sure the Clang compiler is installed and runnable
  On OSX, it's part of the Xcode package. You can run 'clang -v' to check.

Install the Boehm Garbage Collector v. 7.2 from [here](http://www.hboehm.info/gc/gc_source/gc-7.2f.tar.gz). You can build it by doing something like ./configure, make, sudo make install, mv gc-7.2 boehm, cd boehm, ln -s /usr/local/lib lib

  Toccata's 'build' script expects to find it in ~/boehm

Clone this repo

cd to the repo directory

run the 'scripts/build' script.
  This will compile the 'toccata' executable and then use that to compile 'examples/hello.toc' and execute it. You should see 'Howdy, Universe!!!' as the final output.

Rebuilding Toccata core.c and toccata.c from toccata.toc
=========

Run './toccata toccata.toc > toccata.c'

Then you can re-run the 'build' script.

Good luck!!!
