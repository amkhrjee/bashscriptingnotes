# `!#`
The sha-bang ( `#!`) at the head of a script tells your system that this file is a set of commands to be fed to the command interpreter indicated. The `#!` is actually a two-byte magic number, a special marker that designates a file type, or in this case an executable shell script (type `man magic` for more details on this fascinating topic). Immediately following the sha-bang is a path name. This is the _path to the program that interprets the commands in the script_, whether it be a shell, a programming language, or a utility. This command interpreter then executes the commands in the script, starting at the top (the line following the sha-bang line), and ignoring comments. 