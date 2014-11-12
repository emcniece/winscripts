winscripts
==========

A small package of Windows batch scripts for everyday use

=== tempclean ===
Empties old contents of a given folder. Things to edit:
 - "G:\temp" - directory to empty out
 - -10 - remove files older than 10 days
 
forfiles -p "G:\temp" -s -m *.* /D -10 /C "cmd /c del @path"