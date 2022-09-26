## 1. man pages from vim

Pressing ``K`` from the word (in normal mode) opens the man page for the word. But being unable to see the man page and the text, unable to open multi-words man page (for example ``man git diff``) or unable to copy text from the man page are some of the disadvantages.

The **trick** is vim inbuilt plugin called **man**. 
1. First, load the man filetype plugin
	``:runtime! ftplugin/man.vim``
2. Run Man command
	``:Man git diff`` or
  ``:Man 3 echo``

To find out more
``:h find-manpage``


## 2. List all key mapping
```
:redir! > vim_keys.txt
:silent verbose map
:silent verbose imap
:silent verbose vmap
:redir END
```

## 3. copy a line without a newline character
I used to visually select a line and yank the line (``Vy``), but it copies with the newline character.

The **trick** is ``^y$``
