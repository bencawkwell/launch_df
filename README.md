launch_df
=========

Simple script to launch Dwarf Fortress without having to first cd into the df_linux directory. It also allows some settings to be changed in the init.txt file before launch based on arguments

Installation
------------

Copy the dwarffortress file into your PATH, for example /bin.

The default assumption is that you want to launch /df_linux/df. You can change this by creating the file /etc/dwarffortress.conf. Use the dwarffortress.conf.example file as an example.

Usage
-----

To get the list of available arguments:

    dwarffortress --help

For example to skip the intro:

    dwarf-fortress --skip-intro

Todo
----

* Add more settings to be modified using command line arguments.
* Restore setting after df quits.
* An argument to update existing saves with the raw directory from the df_linux directory (useful when a new tile set has been added).