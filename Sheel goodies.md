# Sheel goodies

Shell aliases and shell functions can not be used in subshells. You can make the alias global via `alias -g myalias="…"` or
`export -f my_function` to make available to child processes.

You might still need to call your function with `bash -c 'my_function "$1"'`.

Ref.: https://github.com/sharkdp/fd#command-not-found-for-aliases-or-shell-functions
