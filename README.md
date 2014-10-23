gvimServer
==========

This project is a collection of simple scripts to take advantage of VIM's server capabilities.

BTW, I completely don't use this any more as I do all my Vimming in a console now.

Requirements
------------

These are BASH scripts that call VIM, so BASH and VIM are the only requirements, which means no native Windows.

Installation
------------

Clone this project somewhere, most likely your ~/bin directory. Add a line to source the grc file in your .bashrc or .profile file. That's it.

Sourcing the grc file will extend your path to include the gvimServer directory and it creates two aliases: 'g' and 'gset'.

Usage
-----

gset - set the server name to use. Can be '.' to set to current working directory or '-' to reset to default. Any other values are used literally. Running gset with no parameters shows the current server name.

g - alias to GVIM using the current server name. Can also use -s to explicitly set the server name.

vim --serverlist to see the current operating servers.

See Also
--------

See the --servername, --remote-silent and --serverlist options to VIM.
