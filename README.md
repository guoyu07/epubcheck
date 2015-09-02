EpubCheck
=========

EpubCheck is a tool to validate EPUB files. It can detect many
types of errors in EPUB. OCF container structure, OPF and OPS mark-up,
and internal reference consistency are checked. EpubCheck can be run
as a standalone command-line tool or used as a Java library.


## Releases

Check the [release page](https://github.com/IDPF/epubcheck/releases) to get the latest distribution.

[EpubCheck 4.0](https://github.com/IDPF/epubcheck/releases/tag/v4.0.0) is the latest recommended version to validate both EPUB 2 and 3 files.


## Documentation

Documentation on how to **use** or how to **contribute** is available on the [EpubCheck wiki](https://github.com/IDPF/epubcheck/wiki).

Technical discussions are hosted on the [EpubCheck Google Group](https://groups.google.com/forum/#!forum/epubcheck)


## Credits

EpubCheck is a project coordinated by [IDPF](http://idpf.org/). Most of the EpubCheck functionality comes from the schema validation tool [Jing](http://www.thaiopensource.com/relaxng/jing.html) and schemas that were developed by [IDPF](http://www.idpf.org/) and [DAISY](http://www.daisy.org/). Initial EpubCheck development was largely done at [Adobe Systems](http://www.adobe.com/).

Authors and contributors to EpubCheck include:

 * Peter Sorotokin
 * Garth Conboy
 * Markus Gylling
 * Piotr Kula
 * Paul Norton
 * Jessica Hekman
 * Liza Daly
 * George Bina
 * Bogdan Iordache
 * Romain Deltour
 * Thomas Ledoux
 * Tobias Fischer
 * Steve Antoch
 * Arwen Pond
 * Masayoshi Takahashi
 * Satoshi KOJIMA

## License

EpubCheck is made available under the terms of the [New BSD License](http://opensource.org/licenses/BSD-3-Clause)

----

## Building EpubCheck
[![Build Status](https://travis-ci.org/IDPF/epubcheck.svg?branch=master)](https://travis-ci.org/IDPF/epubcheck/)

To build epubcheck from the sources you need Java Development Kit (JDK) 1.7 or above and [Apache Maven](http://maven.apache.org/) 2.3 or above installed.
On Windows, you should build in a git bash shell (see http://github.com help)

You will also need Python to be able to run the BookReporter and related tools.


Build and run tests:

```
$ mvn install
```
Will copy `.*jar` files and packages to `target/` folder...


## Translating EpubCheck

EpubCheck 4.0 now comes with *i18n* support. Feel free to translate the Java messsages file to your language and then open a Pull Request here.

Translations so far:
* `en` - English
* `ja` - Japanese
* `de` - German (Tobias Fischer, PR #462)
* `es` - Spanish (Emiliano Molina, PR #470, #482)
* `fr` - French (Vincent Gros, PR #472)
* `it` - Italian (Alberto Pettarin, PR #496)

To translate, simply copy the original (english) message file (`MessageBundle.properties` or `messages.properties`) located in
* [src/main/resources/com/adobe/epubcheck/messages/](src/main/resources/com/adobe/epubcheck/messages/)
* [src/main/resources/com/adobe/epubcheck/util](src/main/resources/com/adobe/epubcheck/util)
* [src/main/resources/com/thaiopensource/datatype/xsd/resources](src/main/resources/com/thaiopensource/datatype/xsd/resources)
* [src/main/resources/com/thaiopensource/relaxng/pattern/resources](src/main/resources/com/thaiopensource/relaxng/pattern/resources)
* [src/main/resources/org/idpf/epubcheck/util/css](src/main/resources/org/idpf/epubcheck/util/css)

to `MessageBundle_XX.properties` or `messages_XX.properties` in its respective folder and start translating.

Send us a PullRequest when you finished translation and think it's ready to merge...
