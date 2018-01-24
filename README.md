Multi-TOR
=========

Tools for handling multiple TOR connections

* multitor.sh - opens multiple TOR instances
* tor_newid.sh - requests new identity (IP address) to multiple TOR instances

Changelog
-------------
* 2018-01-22	Fixed relative path issue
* 2013-09-09    Added tor_newid.sh

Dependencies
------------
* tor
* telnet	( just for ip renewal )

You may install both with "sudo apt-get install tor telnet"

Usage
------------
* multitor.sh	sh ./multitor.sh $1 where "$1" is the number of Tor instances.
		Example: "sh ./multitor.sh 5" this will open 5 instances.

* tor_newid.sh	sh ./tor_newid.sh N where "$1" is the number of Tor instances.
		NOTE that "$1" should be the same number used in multitor.sh

NOTE:	Both scripts works in a serial way starting from the first and prooceding until they meet the given number $1
