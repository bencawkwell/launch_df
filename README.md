launch_df
=========

Simple script to launch Dwarf Fortress but allows using arguments to set certain settings in the ini.txt config file before launch.

Usage
-----

The following command will launch Dwarf Fortress residing in the df_linux directory setting PRINT_MODE to TEXT and INTRO to NO in init.txt, making Dwarf Fortress run in the console while skipping the intro:

    launch_df.sh -p TEXT -s df_linux/df

If you use dfHack, you can launch that instead:

    launch_df.sh -s df_linux/dfhack

Todo
----

* Restore configuration file after exit.
* Tests