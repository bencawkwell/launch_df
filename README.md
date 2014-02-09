launch_df
=========

Simple script to launch Dwarf Fortress but allows using arguments to set certain settings in the ini.txt config file before launch.

A word of warning, this has barely undergone any kind of testing and is very sloppy when it comes to handling errors. Make backups before using this script.

Usage
-----

The following command will launch Dwarf Fortress residing in the df_linux directory setting PRINT_MODE to TEXT and INTRO to NO in init.txt, making Dwarf Fortress run in the console while skipping the intro:

    launch_df.sh -p TEXT -s df_linux/df

If you use dfHack, you can launch that instead:

    launch_df.sh -s df_linux/dfhack

Using tile sets
---------------

You can use the -t option to specify the path to a directory containing a custom tile set. For example the following will import the famous Phoebus tile set assuming you placed in a directory called myTilesets:

    launch_df -t myTilesets/Pheobus_34_11v01 df_linux/df

Before importing any tile sets the script will first create a backup of files that might get replaced by the tile set in df_linux/backup/curses. When the -t option is omitted then a cleanup is performed and the backup is restored. You might find this annoying if you have made custom changes to init.txt yourself. In this case make the changes to the init.txt files in the backup and in any tile sets you which to use.

In some tile sets, the configuration files sit in a sub directory under data/init. For example Phoebus ships with all the configuration files you need in data/init/Phoebus. In order for this tile set to be imported you will need to move all the files in data/init/Phoebus into data/init.

Todo
----

* More robust. Since I am writing this for a docker container I have so far invested no time into handling errors properly, and have only tested a few scenarios so the whole thing is very fragile.
* Restore configuration files and tile set data after exit.
* Tests