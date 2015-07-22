# Emacs cheat-sheet


##Help

LISP function | Key binding | description
--- | --- | ---
help-for-help | C-h ? | navigate the help system
describe-key | C-h k | describe a key sequence
describe-bindings | C-h b | show all key bindsings


## Oops!!!
LISP function | Key binding | description
--- | --- | ---
undo | C-x u |
keyboard-quit | C-g | emergency exit
suspend-frame | C-z | whatever you do, DO NOT push this shiny red button.
view-lossage | C-h l | view a complete history of all the commands you've entered so far
list-command-history | M-x list-command-history | view a history of mini-buffer commands you've entered



##Files
LISP function | Key binding | description
--- | --- | ---
find-file | C-x C-f | READ: Switch to buffer containing specified file
find-alternate-file | C-x C-v | Replace buffer contents with specified file
insert-file | C-x i | Insert contents of file into buffer
find-file-other-window | C-x 4 C-f | Read contents of file into next window
find-file-other-window | C-x 4 f | Read contents of file into next window
find-file-read-only-other-window, | C-x 4 r | Read contents of file into next window (read only)
save-buffer | C-x C-s | SAVE: Save the current buffer to its file
write-file | C-x C-w | Save a buffer to a specified file
save-some-buffers | C-x s | Save any or all buffers to their files


##Windows
LISP function | Key binding | description
--- | --- | ---
delete-window | C-x 0 | kill the current window
delete-other-windows | C-x 1 | delete all windows except selected window
split-window-below | C-x 2 | split selected window vertically
split-window-right | C-x 3 | split selected window horizontally
other-window | C-x o | switch to the other window


##Buffers
LISP function | Key binding | description
--- | --- | ---
list-buffers | C-x C-b | see a list of all Buffers
switch-to-buffer | C-x b | display a different buffer in the selected window
kill-buffer | C-x k | kill (delete) a buffer


##Cursor Movement

LISP function | Key binding | description
--- | --- | ---
backward-char | C-b | Move back one character
forward-char | C-f | Move forward one character
backward-word | M-b |
forward-word | M-f |
forward-word | M-5 M-f | Move forward 5 words
previous-line | C-p |
next-line | C-n |
move-beginning-of-line | C-a
move-end-of-line | C-e |
backward-sentence | M-a |
forward-sentence | M-e |
scroll-up-command | C-v |
scroll-down-command | M-v |
beginning-of-buffer | M-< |
end-of-buffer | M-> |



## Make it more purty
LISP function | Key binding | description
--- | --- | ---
linum-mode | N/A | show line numbers


## Region: Select it
LISP function | Key binding | description
--- | --- | ---
set-mark-command | C-SPC | set mark to current location of point
exchange-point-and-mark | C-x C-x | interchange mark and point
mark-paragraph | M-h | put region around paragraph
mark-whole-buffer  | C-x h | put region around entire buffer
mark-word | M-@ | set mark after next word (do not move point)
mark-word  | M-2 M-@ | set mark after next 2 words (do not move point)
  

## Region: Do stuff to it									
LISP function | Key binding | description
--- | --- | ---
kill-ring-save | M-w | COPY
yank  | C-y | PASTE
kill-region  | C-w | CUT: kill (erase) all the characters  
downcase-region  | C-x C-l | convert the characters to lowercase
upcase-region | C-x C-u | convert all characters in region to uppercase
count-words-region | M-= | count lines, words and characters
shell-command-on-region | M-\| wc -l | run a shell command, use characters as data
shell-command-on-region | M-\| sort -u | run a shell command, use characters as data
  

##Editing
LISP function | Key binding | description
--- | --- | ---
open-line | C-o | open a new line


##DELETE commands
LISP function | Key binding | description
--- | --- | ---
delete-backward-char | DEL | delete character to the left of point
delete-backward-char | M-3 DEL | delete 3 characters to the left of point (KILL command)
delete-char | C-d | delete character to the right of point
delete-char | M-5 C-d | delete 5 characters to the right of point (KILL command)
delete-horizontal-space | M-\ | delete spaces & tabs around point
just-one-space | M-SPC | delete spaces & tabs around point; leave one space
delete-blank-lines | C-x C-o | delete blank lines around current line
delete-indentation | M-^ | join two lines (delete newline + surrounding spaces)


##KILLin
LISP function | Key binding | description
--- | --- | ---
kill-line | C-k | kill from cursor to end of line
kill-word | M-d | kill a word forward
kill-word | M-3 M-d | kill a 3 words forward
backward-kill-word | M-DEL | kill a word backwards
backward-kill-word | M-5 M-DEL | kill 5 words backwards
kill-sentence | M-k | kill from cursor to end of sentence
backward-kill-sentence | C-x DEL | kill backward to beginning of sentence
kill-region | C-w | kill the region
zap-to-char | M-z char | kill through next occurrence of char
 

##Yankin
LISP function | Key binding | description
--- | --- | ---
yank | C-y | yank most recently killed text
universal-argument, yank| C-u C-y | same as C-7, cursor at beginning of new text
yank-pop | M-y | replace yanked text with ealier killed text
yank-pop  | C-y M-y | use if "previous command was not a yank"
yank-pop  | C-u -1 M-y | cycle backwards by 1 jump through the kill-ring
kill-ring-save | M-w | copy region to kill ring
append-next-kill | M-C-w | append next kill to newest kill ring
describe-variable | C-h v |
 | C-h v kill-ring | display the actual values in the kill ring
 
##Fixin stuff
LISP function | Key binding | description
--- | --- | ---
delete-backward-char | DEL | delete one character to the left of cursor
backward-kill-word | M-DEL | kill the previous word
backard-kill-sentence | C-x DEL | kill to the beginning of the sentence
negative-argument | M-- | do the opposite of what comes next
 | M--M-u | change the previous word to uppercase
 | M--M-l | change the previous word to lowercase
transpose-chars | C-t | transpose two adjacent characters
transpose-words | M-t | transpose two adjacent words
transose-lines | C-x C-t | transpose two consecutive lines

 