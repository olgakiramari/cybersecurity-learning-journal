# Linux Practice — Week 2
end of linux journey commannd line

start of text fu -
stdout
stdin
stderr
pipe and tee 
env
cut
paste
head
tail
expand and unexpandt
join and split
sort
tr(translate)
uniq
wc and nl
grep
 μπηκα advanced text fu kai eknaa regex,text editors, vim, vim search patterns, vim navogation,vim inserting and appending text
 vimtutor in terminal chapter 1

learned about emacs and finished advamced text fu

# Linux Log Investigation Lab

A small Linux command-line lab I completed to review the skills I learned
through Linux Journey.

## Tasks

- Navigated and managed files/directories
- Searched for files and log entries
- Filtered ERROR and failed login events
- Analyzed users and IP addresses
- Practiced stdout/stderr redirection
- Combined commands using pipes
- Used Vim to create and edit investigation notes

## Commands Practiced

`grep`, `cut`, `sort`, `uniq`, `find`, `cat`, `head`, `tail`, `cp`, `mv`,
`ls`, `wc`, `vim`, pipes and redirection.

## Example

    grep "Login failed" security.log | cut -d ' ' -f6 | sort | uniq -c

This lab helped me practice combining multiple Linux commands to analyze
log data instead of using each command individually.





# Linux Practice — Week 3

Continued my Linux fundamentals through Linux Journey, focusing on user management, ownership, file permissions, and special permission bits.

## User Management

- Learned how Linux identifies users and groups using UIDs and GIDs
- Practiced `id`, `groups`, and `getent passwd`
- Learned the difference between primary and supplementary groups
- Studied the root account and the significance of UID 0
- Learned how `sudo`, `su`, and `su -` differ
- Learned how `/etc/passwd` stores local account information
- Studied service accounts and login shells
- Learned basic account and password management concepts

## File Permissions & Ownership

- Learned how Linux `r`, `w`, and `x` permissions work for user, group, and others
- Practiced reading file and directory permissions with `ls -l` and `ls -ld`
- Used symbolic permissions with `chmod`
- Used octal permissions such as `640` and `750`
- Practiced changing file ownership and group ownership with `chown` and `chgrp`
- Learned how directory permissions differ from file permissions
- Learned how parent directory permissions affect file deletion
- Studied `umask` and how it affects permissions on newly created files and directories

## Special Permissions

- Learned how SetUID allows an executable to run with the file owner's effective UID
- Learned how SetGID works on executables and how SetGID directories can make new files inherit the directory's group
- Learned how the Sticky Bit protects entries inside shared writable directories
- Learned who can remove or rename entries inside a directory protected by the Sticky Bit
- Practiced recognizing SetUID (`s`), SetGID (`s`), and Sticky Bit (`t`) in permission strings

## Commands Practiced

`id`, `groups`, `getent`, `sudo`, `su`, `ls -l`, `ls -ld`, `chmod`, `chown`, `chgrp`, `umask`

## Key Takeaway

This section helped me understand how Linux controls access through users, groups, ownership, standard permissions, and special permission bits such as SetUID, SetGID, and the Sticky Bit.
