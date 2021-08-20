#  Resource monitoring on Linux

## Memory 
`free`	Gives free RAM on your system

`free -m` Shows it in -mebibytes

`free -g` Shows it in -gigibytes

`df` Gives free Hardisk space on system

`df -h` Makes it more human readable

`df -i` Shoes INodes (Maximum number of files Allowed)

## Processes

`top` Details on all processes

`htop` Great way to manage processes

[`ps`](https://linuxize.com/post/ps-command-in-linux/) Shows running processes 

`pidof` Gives pid of a running process

`ps -aux` Shows all processes with Pid

`kill <PID>` Kills selected process (can use Htop for this (f9))

## Priority

`nice` Starts a Process with a given Priority

`renice` Changes priority of an already running process




