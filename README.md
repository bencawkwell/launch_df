launch_df
=========

Simple script to launch Dwarf Fortress without having to first cd into the df_linux directory.

Installation
------------

Copy the dwarffortress file into your PATH, for example /bin.

The default assumption is that you want to launch /df_linux/df. You can change this by creating the file /etc/dwarffortress.conf. Use the dwarffortress.conf.example file as an example.

Usage
-----

    dwarffortress

Todo
----

* Allow for some setting in init.txt to be overridden using command line arguments.
* An argument to update existing saves with the raw directory from the df_linux directory (useful when a new tile set has been added).