# The Kitchen Drawer
This contains scripts, tools, and other oddments that users of ACENET and Alliance systems will find useful. 

Contents
--------
* **nsync** . This is a file transfer shell-script for transferring very, very large numbers of files where Globus 
is not an option. It utilises *rsync* to do the actual file transfer, but circumvents the slowdown typical of rsync
when transferring lots of files, by breaking up the transfer into chunks. It is also multithreaded. 
It will only work on files or directories which have a regular naming convention and are consecutively
numbered, eg. 'thisprefix_XXXXX.suffix' (the suffix is optional). This may change as nsync is developed. For a list of options, 
simply run the command without options or read the commented script.
