# BookOS
***
### Table of contents
1. [General Info](#general-info)
2. [How To Install](#how-to-install)
***
### General info
BookOS is a simple to use, lightweight, open source command line interface (gui may come later) operating system designed to help do some simple tasks. It is still in development and not yet finished, so **may** be unstable.

***
## How to install

* Download all of the files and folders from this github repository
* Install [docker](https://www.docker.com/)
* Install a virtual environment

#### Windows
* Run the follwoing commands:
```bash
docker build buildenv -t {name}
# Command prompt
docker run --rm -it -v %cd%:/root/env {name}
# Powershell
docker run --rm -it -v "${pwd}:/root/env" {name}
```

### Linux or MacOS
* Run the following commands:
```bash
docker build buildenv -t {name}
docker run --rm -it -v "$pwd":/root/env {name}
```

***
## How to run the OS

By now, you should have a `.iso` file located in `dist\x86_64`. Open up your choice of virtual machine software and select that as the `iso` file. Once you start the virtual machine, you will have BookOS running.
