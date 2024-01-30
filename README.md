# The Regression Test Harness for the OpenJDK platform: `jtreg`

* For details on writing tests for `jtreg`, see
  [The JDK Test Framework: Tag Language Specification][tagspec].

* For details on building `jtreg`, see
  [doc/building.md](doc/building.md).

* For additional details about `jtreg`, see
  [The `jtreg` FAQ][faq].

* For details on running JDK tests using the JDK _make test_ framework, see
  [Using "make test" (the run-test framework)][make-test].

[faq]: https://openjdk.java.net/jtreg/faq.html
[tagspec]: https://openjdk.java.net/jtreg/tag-spec.html
[make-test]: https://github.com/openjdk/jdk/blob/master/doc/testing.md

## Using IntelliJ IDEA

The `jtreg` repo also contains a plugin for the IntelliJ IDEA IDE.
This is a convenience plugin which adds `jtreg` capabilities to the IDE.
With this plugin, OpenJDK developers can write, run, and debug `jtreg` tests
without leaving their IDE environment.  For more details, see the file
[plugins/idea/README.md](plugins/idea/README.md) in this repo.

## crashonly

The [https://github.com/openjdk/jtreg/commit/71838a66cbb8f1ab28844317b97e4fbb02730c42](https://github.com/openjdk/jtreg/compare/master...andrlos:jtreg:jtregCrashOnly) enhances the code with crashonly feature that only admits failures when jvm crashes.. This is meant to be used with debug jvm testing. 7.3 is intended for jdk11 and above and as such should be built on jdk11. A string notifying about changed result is in explanation of every testresult that has been changed by this piece of code: "Just a regular failure. Modified by crashonly code."
