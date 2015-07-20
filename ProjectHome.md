# python-gflags #

This project is the python equivalent of [gflags](http://code.google.com/p/gflags), a commandline flag implementation for C++ originally written by Google.  It is intended to be used in situations where a project wants to mimic the command-line flag handling of a C++ app that uses [gflags](http://code.google.com/p/gflags), or for a Python app that, via swig or some other means, is linked with a C++ app that uses [gflags](http://code.google.com/p/gflags).

The `python-gflags` package contains a library that implements commandline flags processing.  As such it's a replacement for `getopt()`.  It has increased flexibility, including built-in support for Python types, and the ability to define flags in the source file in which they're used.  (This last is its major difference from `OptParse`.)

Documentation is at the top of [gflags.py](http://python-gflags.googlecode.com/svn/trunk/gflags.py).

## 18 January 2012 ##

I've just released python-gflags 1.8.  This fixes a bug, allowing
modules defining flags to be re-imported without raising duplicate
flag errors.

Administrative note: In the coming weeks, I'll be stepping down as
maintainer for the python-gflags project, and as part of that Google
is relinquishing ownership of the project; it will now be entirely
community run.  The remaining
[changes](http://python-gflags.googlecode.com/svn/tags/python-gflags-1.8/ChangeLog)
in this release reflect that shift.


### 20 December 2011 ###

I've just released python-gflags 1.7.  The major change here is
improved unicode support, in both flag default values and
help-strings.  We've also made big steps toward making gflags work
with python 3.x (while keeping 2.4 compatibility), and improving
--help output in the common case where output is a tty.

For a full list of changes since last release, see the
[ChangeLog](http://python-gflags.googlecode.com/svn/tags/python-gflags-1.7/ChangeLog).

### 29 July 2011 ###

I've just released python-gflags 1.6.  This release has only minor
changes, including support for multi\_float flags.  The full list of
changes is in the
[ChangeLog](http://python-gflags.googlecode.com/svn/tags/python-gflags-1.6/ChangeLog).

The major change with this release is procedural: I've changed the
internal tools used to integrate Google-supplied patches for gflags
into the opensource release.  These new tools should result in more
frequent updates with better change descriptions.  They will also
result in future `ChangeLog` entries being much more verbose (for
better or for worse).

### 26 January 2011 ###

I've just released python-gflags 1.5.1.  I had improperly packaged
python-gflags 1.5, so it probably doesn't work.  All users who have
updated to python-gflags 1.5 are encouraged to update again to 1.5.1.

### 24 January 2011 ###

I've just released python-gflags 1.5.  This release adds support for
flag verifiers: small functions you can associate with flags, that are
called whenever the flag value is set or modified, and can verify that
the new value is legal.  It also has other, minor changes, described
in the
[ChangeLog](http://python-gflags.googlecode.com/svn/tags/python-gflags-1.5/ChangeLog).

### 11 October 2010 ###

I've just released python-gflags 1.4.  This release has only minor
changes from 1.3, including support for printing flags of a specific
module, allowing key-flags to work with special flags, somewhat better
error messaging, and
[so forth](http://python-gflags.googlecode.com/svn/tags/python-gflags-1.4/ChangeLog).
If 1.3 is working well for you, there's no particular reason to upgrade.

### downloads now available ###

`.egg` and `.tar.gz` files are now available on the 'downloads' pane to the right.

### python-gflags 1.3 released ###

I just released python-gflags 1.3.  This is the first python-gflags release; it is version 1.3 because this code is forked from the 1.3 release of [google-gflags](http://code.google.com/p/google-gflags).

I don't have a tarball or .deb file up quite yet, so for now you will have to get the source files by browsing under the 'source' tag.  Downloadable files will be available soon.