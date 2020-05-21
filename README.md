# googleapiclient dependency

This represents a "super-dependency" library for Sublime Text 3 that bundles
together all of the myriad libraries required to access Google API's via Python
from a Sublime Text 3 plugin.

In particular the libraries included here are version locked at the last known
versions that support Python 3.3; the dependency load order is specifically
set to load this dependency last to ensure that other explicit dependencies
(which may have backported changes) will be used before anything included here.

This is primarily intended only for Sublime Text 3 plugins; Sublime Text 4
includes a newer version of Python so newer libraries should be used for that
version. In addition at the current time Package Control doesn't support
dependencies for any packages using the newer Python runtime and when such
support is added, the scheme used is likely to not be similar to this.
