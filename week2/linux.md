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
