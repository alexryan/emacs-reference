# Emacs cheat-sheet


##Help

LISP function | Key binding | description
--- | --- | ---
help-for-help | C-h ? | navigate the help system
describe-key | C-h k | describe a key sequence
describe-bindings | C-h b | show all key bindsings



##Cursor Movement & Scrolling

LISP function | Key binding | description
--- | --- | ---
next-line | C-n |
previous-line | C-p |
forward-word | M-f |
backward-word | M-b |
move-beginning-of-line | C-a
move-end-of-line | C-e
forward-char | C-f | Move forward one character
backward-char | C-b | Move back one character
scroll-up-command | C-v |
scroll-down-command | M-v |


#Editing
LISP function | Key binding | description
--- | --- | ---
open-line | C-o | open a new line
delete-backward-char | DEL | delete character to the left
delete-char | C-d | delete character to the right


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



##Miscellaneous
LISP function | Key binding | description
--- | --- | ---
keyboard-quit | C-g | emergency exit
