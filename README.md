# node-dev-box
A Vagrant powered virtual machine for NodeJS application development.

## Requirements

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

## How To Build The Virtual Machine

Building the virtual machine is this easy:

    host $ git clone https://github.com/skanukov/node-dev-box
    host $ cd node-dev-box
    host $ vagrant up

That's it.

After the installation has finished, you can access the virtual machine with

    host $ vagrant ssh

Default PostgreSQL port 5432 in the host computer is forwarded to port 5432 in the virtual machine.

Don't forget to look at some helper shell scripts for newbies.

## What's In The Box

* Ubuntu 16.04

* PostgreSQL 9.6

* NodeJS 6.9 LTS with Npm 3.10 and the latest stable Yarn

* The latest stable Git

## Note About Symlinks

To allow guest system to create symlinks, `vagrant up` command should be run as administrator.

## License

Released under the MIT License, Copyright (c) 2016 Sergey Kanukov, inspired by official [Rails dev box](https://github.com/rails/rails-dev-box).
