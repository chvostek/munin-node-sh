# This is munin-node-sh

It's a munin-node alternative written entirely in shell, with minimal dependencies.  *It doesn't work yet.*  Or at least, it may not.  YMMV.

Munin-node-sh is not associated with or part of the Munin project.

Munin-node-sh provides a number of plugins internally:

* df
* zfslist
* cpu
* if_
* if_err_
* load
* memory
* swap
* processes
* netstat
* uptime

Other plugins may be provided via the standard plugin directory ... the location of which is configurable.

## Requirements:

Munin-node-sh has pretty light-weight requirements.  No build should be required.  Available plugins are determined by configuration and the set of dependencies that are found.  For example:

Dependency | Services
---- | ----
`smartctl` | disk temperature
`zfs` | zfslist, for dataset usage (like df but better)
`zpool` | IO statistics for a given ZFS pool

## Provisos:

* At the moment, munin-node-sh handles only one node, the local machine (per `hostname`), and ignores any specification of node by the server. This may be adjusted in future versions, but probably not, in the interest of keeping munin-node-sh as light-weight as possible.

## See also:

* Munin lives at http://munin-monitoring.org/.
* [MuninLite](http://sourceforge.net/projects/muninlite/) is a Bourne shell replacement for munin-node and some plugins.  Looks like its goals are the same as munin-node-sh's goals.  Hasn't been updated since 2011.

