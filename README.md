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

Another useful feature is the option to update the raw directory in your saved games, something you typically need to do after switching tile sets:

    dwarffortress --update-saves

Todo
----

* Add more settings to be modified using command line arguments.
* Restore settings after df quits.