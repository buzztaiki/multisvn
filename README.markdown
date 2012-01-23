multisvn - SVN version auto detecter
====================================

Overview
--------

multisvn does detecting and running a svn for current working copy. It allows multi svn executable in your environment.

Installation
------------

1. Put multisvn script into `~/bin`

2. Configure `~/.subversion/config` file as followings:

        [multisvn]
        # svn1.6 executable
        svn16 = /usr/bin/svn
        # svn1.7 executable
        svn17 = ~/opt/svn-1.7/bin/svn
        # fall back to svn1.7 when current directory is not wc.
        svn = %(svn17)s

Usage
-----

Run `multisvn` instead of a `svn`. You also create an alias for `multisvn`.
