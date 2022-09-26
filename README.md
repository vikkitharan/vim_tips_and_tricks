# vim tips and tricks

## Read man page from vim

Pressing ``K`` from the word (in normal mode) opens the man page for the word. But it has disadvantages, like being unable to see the man page and the text, unable to open multi word man page (for example ``man git diff``) or unable to copy text from the man page.

The **trick** is vim inbuilt plugin called **man**. 
1. First, load the man filetype plugin
	``:runtime! ftplugin/man.vim``
2. Run Man command
	``:Man git diff`` or
  ``:Man 3 echo``

To find out more
``:h find-manpage``
