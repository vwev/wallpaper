Wallpaper Script
================

INSTALL
-------

	$ git clone https://github.com/vwev/wallpaper.git
	$ cd wallpaper
	$ mkdir -p ~/.config/wallpaper
	$ cp examples/config.example ~/.config/wallpaper/config
	$ cp examples/category.example ~/.config/wallpaper/category
	$ # edit the files according to comments
	$ ./wallpaper # or copy it to your PATH

If you want it to automatically change at a time interval, append the following line to crontab:

	# change wallpaper every 10 minutes
	*/10 * * * * ~/bin/wallpaper

CONFIGURATION
-------------

See the comments in examples [config.example](examples/config.example) and [category.example](examples/category.example).

USAGE
-----

	USAGE: wallpaper [ARG] [CATEGORY] ...

	ARG:
		-a, --add
			Add categories to wallpaper list.
		-o, --overwrite
			Replace categories in wallpaper list. [default]
		-l, --list
			print wallpaper list and exit

	CATEGORY:
		A list of files, directories or category file entries.

	ENVIRONMENT VARIABLES:
		WALLPAPER_PATH
			The path to wallpaper images.
	NOTE:
		When invoked with no arguments, it will set a random wallpaper
		from the list.
