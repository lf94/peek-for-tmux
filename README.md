# peek-for-tmux
The most useful smallest tmux trick by yours truly.

Place this in your .bashrc:

`peek() { tmux split-window -p 33 "$EDITOR" "$@" || exit; }`

Restart your terminal.

Run `peek a_file_you_really_want_to_look_at.txt`

PS! Make sure you have set `export EDITOR=<your editor of choice>`, otherwise the split window will just open then close.
