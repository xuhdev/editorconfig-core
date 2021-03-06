[EditorConfig][]
==============

[![Build Status](https://secure.travis-ci.org/editorconfig/editorconfig-core.png?branch=master)](http://travis-ci.org/editorconfig/editorconfig-core)

EditorConfig makes it easy to maintain the correct coding style when switching
between different text editors and between different projects.  The
EditorConfig project maintains a file format and plugins for various text
editors which allow this file format to be read and used by those editors.  For
information on the file format and supported text editors, see the
[EditorConfig website][EditorConfig].


Contributing
------------

This is the README file for the *EditorConfig core* codebase.  This code
produces a program that accepts a filename as input and will look for
`.editorconfig` files with sections applicable to the given file, outputting
any properties found.

When developing an editor plugin for reading EditorConfig files, the
EditorConfig core code can be used to locate and parse these files.  This means
the file locator, INI parser, and file globbing mechanisms can all be
maintained in one code base, resulting in less code repitition between plugins.


Installation
------------

To install the EditorConfig core from source see the `INSTALL` file.

Binary installation packages for the EditorConfig core can be found on the [downloads page on Github][downloads].


Getting Help
------------

For help with the EditorConfig core code, please write to our [mailing list][].
Bugs and feature requests should be submitted to our [issue tracker][].

If you are writing a plugin a language that can import C libraries, you may
want to import and use the EditorConfig library directly.  If you do use the
EditorConfig core as a C library, check the [documentation][] for help.


License
-------

Unless otherwise stated, all files are distributed under the Simplified BSD
license. The inih(`src/lib/ini.c` and `src/lib/ini.h`) and fnmatch
(`src/lib/ec_fnmatch.c` and `src/lib/ec_fnmatch.h`) libraries are distributed
under the New BSD license. See LICENSE file for details.


[EditorConfig]: http://editorconfig.org "EditorConfig Homepage"
[mailing list]: http://groups.google.com/group/editorconfig "EditorConfig mailing list"
[issue tracker]: https://github.com/editorconfig/editorconfig/issues
[documentation]: http://editorconfig.org/core-docs/ "EditorConfig Core C API documentation"
[downloads]: https://github.com/editorconfig/editorconfig-core/downloads
