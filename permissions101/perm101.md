# Perms 101
  
  Please remember this outline was created to assist you in taking notes during our study group. 

## FS Permission Basics
    
`drwxrwxrwx.` 

* `d` rwxrwxrwx. 
* d`rwx`rwxrwx.
* drwx`rwx`rwx.
* drwxrwx`rwx`.
* drwxrwxrwx`.`

## Using chmod, chown

`chown root:root file`

`chown root: file`

`chown root file`

`chown :root file`

### chmod
The chmod command changes the mode or the permission set of a file.

Mode can be represented in symbolic or octal notations
Symbolic	rwx, rw, r-x
Octal	755, 644
chmod - Examples

* The following are some examples of how we can use chmod

        chmod 755 file
        chmod u+rwx
        chmod g-rwx
        chmod o=rw


* The following are some examples of how we can use chmod

        chmod 755 file # Change the permissions to 755
        chmod u+rwx
        chmod g-rwx
        chmod o=rw

* The set uid and set gid bits configure a command so that it is executed as said owner or group

* The sticky bit designates that only the owner can delete the file

* These permissions are set with the chmod command.

* Using chmod with a capital -X denotes to only set the execute bit if the execute bit is already set elsewhere in the permissions


## umask & /etc/skel

The umask is what determines what permissions is a new file created with. They are specifying which bits are turned off by default.

    umask
    umask -S
    umask -p

* The umask is set in /etc/profile but can also be set per user or in /etc/skel

## FACLs Introduction

* Defaults are set on a directory and they will carry through to each file under the directory.

* Defaults are set by adding the -d, --default flag indicating the operations are for the default

`setfacl -d -m u:rack:rwx ./testdir/`

### C.R.U.D on FACLs

* Create	setfacl -m u:rack:rwx file
* Read	getfacl file
* Update	setfacl -x u:rack / setfacl -m u:rack:rw
* Delete	setfacl -x -k -b file

## Review and Expand
