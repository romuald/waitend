waitproc
========

This command line tool for Unix executes a command when another process is 
ended.

usage: waitproc [-h] [--delay DELAY] [--mines] process cmd

Execute a command when another process is ended

positional arguments:
  process        the PID or the commandname of the pending process
  cmd            command executed when pid finished

optional arguments:
  -h, --help     show this help message and exit
  --delay DELAY  wait DELAY seconds between two process checks
  --mines        search only in processes owned by user


By default, waitproc waits 60 seconds between two checks.
The --mines could be useful when watchedProcess is a name.


Requirements
------------

 - Python 2.7
 - `ps`


Licence
-------

Released under GNU General Public License version 3 or (at your option) any
later version.

