1. bash-1  
- [x] more greenhand-friendly, save for lots of terms  
- [x] Ask win user to use wsl or git bash(?? not tested)  
- [x] explain the processes between user inputing commands and kernel executing
- [x] rearrange bash syntax and tools sequence
- [x] bind and bindkey (expansion?)
- [x] redirect and pipeline illustrations  
- [x] shells comparison zsh,fish(optional)  


1. bash-2  

Regex

- [x] Introduce escapes in bracket patterns
- [x] Improve quiz quality
- [x] The pattern `{4,}` should mean "at least" instead of "more than" 
- [x] Explain the `-o` flag in the example with `grep`

`sed`

- [x] Explain `/g` explicitly

Bash scripting

- [x] explain that bash language is an interpretive language and bash interpreter execute commands and scripts.  
introduce shebang

- [ ] \#Variables: all are strings. Could be concatenated. 
Explain:
braces: for speration. e.g. `${VAR}REMANING_STRINGS`

double quote: prevent word splitting and globbing but replace vars with real values. e.g. `"* $VAR"` is one word and `*` is not expanded.  

single quote: literal interpretation.  

Reference: https://stackoverflow.com/questions/18135451/what-is-the-difference-between-var-var-and-var-in-the-bash-shell

(remove the Note in \#for startements: range)

- [ ] Special Variables(Before \#Exit status)  
Introduce `$0 $# $@ $* $?`
`$?` could be connected to \#Exit status

- [ ] completely remove `IFS=$'\n'` and add proper double quotes.
its very easy to abuse since it affect global bash expansion. The better approach is to use double quotes.  

Also, replace every `$(ls)` with `*`
`$(ls)` may have the expansion pitfalls and occupy more resources. 

- [ ] in "Print the odd numbered lines of 05-scripting/logos.txt." ex, introduce `$()` and state that `$(cat logos.txt)` is only for practice. Production will use `read`, `awk`, etc. 

- [ ] while loop
```bash
while [ condition ]; do
    # commands
done
```

- [ ] file accessibilities, chmod and chown  
- [ ] source script file vs execute script file(run in current session vs open a new session)  
- [ ] bashrc introduction and sample bashrc  
- [ ] extension: shutdown, reboot, ps, pgrep, pkill alias, etc 
