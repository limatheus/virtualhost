# Easy Virtual hosts
-----
This script is based on the great [RoverWire/virtualhost](https://github.com/RoverWire/virtualhost) (thank's) and modified to my necessities.

This script allows you to create or delete nginx virtual hosts in a pretty easy way.

The base is the Nginx version and to create virtual hosts to my Laravel projects, but work's in *any project* type, just point to the folder where is placed your index.php / index.html.

-----

## Instalation
1. Download the script
```bash
$ wget https://raw.githubusercontent.com/limatheus/virtualhost/master/virtualhost
$ sudo chmod +x virtualhost
$ sudo cp virtualhost /usr/local/bin/virtualhost
```
----

## Usage
You need to be root to run the script.

Basic command line syntax:

```bash
$ sudo virtualhost [create | delete] [domain] [optional host_dir]
```

## Examples

> To create a new virtual host:

```bash
$ sudo virtualhost create mysite.dev
```

> To create a new virtual host with custom directory name:

```bash
$ sudo virtualhost create anothersite.dev my_dir
```
Or

```bash
$ sudo virtualhost create anothersite.dev my_dir/public
```

> To delete a virtual host

The script asks you if want delete the root directory.

```bash
$ sudo virtualhost delete mysite.dev
```

> To delete a virtual host with custom directory name:

The script asks you if want delete the root directory.

```bash
$ sudo virtualhost delete anothersite.dev my_dir

```

### Credits
Based on [RoverWire/virtualhost](https://github.com/RoverWire/virtualhost)

