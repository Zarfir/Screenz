# Screenz
This script is a multiple monitor manager that can allow you to:
- Automatically manage your monitors.
- Choose your monitors when they are connected.

# How to run Screenz ?
First of all you have to give the right of execution to screenz.
```
$ chmod +x ./screenz
```

Then you have to tell the script where your monitors will be located.
```
$ screenz -i
```

# How to use Screenz ?
To know how to use Screenz made :
```
$ screenz -h

NAME
	screenz - set the orientation or output to configuring multiple monitors

SYNOPSIS
	screenz [OPTIONS]

DESCRIPTION

OPTIONS
	-h	Print the different information of this programme.
	-i	Initialize information to set the program.
	-p	Automatic connection if there is an output.
	-c	Choose the output you want.

RETURN VALUE
	On success, screenz return 0.
	On error, screenz return 84.

OTHER
	This application generates a hidden file to run.
		'.screenz' is a hidden file that contains your parameters (do not modify).
```

# You can use Wzpaper with Screenz
If you have Wzpaper in your system application, the Screenz script will call Wzpaper each time you connect to a new monitor to avoid your wallpaper being unstructured by the change of monitor.

Wzpaper is another script that allows you to manage your wallpapers.

If you are interested, click [here](https://github.com/Zarfir/Wzpaper).


# How to autostart with i3 ?
In your i3 config file add these lines :
```
exec screenz -p
```

# To stop it
```
$ killall screenz
```