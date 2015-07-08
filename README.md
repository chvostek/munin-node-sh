# This is munin-node-sh
It's a munin-node alternative written entirely in shell, with minimal dependencies.

Munin-node-sh is not associated with or part of the Munin project.

## Provisos:

* At the moment, munin-node-sh handles only one node, the local machine (per `hostname`), and ignores any specification of node by the server. This may be adjusted in future versions, but probably not, in the interest of keeping munin-node-sh as light-weight as possible.

## See also:

* Munin lives at http://munin-monitoring.org/.
* [MuninLite](http://sourceforge.net/projects/muninlite/) is a Bourne shell replacement for munin-node and some plugins.  Looks like its goals are the same as munin-node-sh's goals.  Hasn't been updated since 2011.

