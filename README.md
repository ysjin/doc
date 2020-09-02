# doc

## mosh
```bash
ps aux | grep mosh # kill mosh server
```


## tmux
```zsh
tmux detach -a # detach all other tmux sessions.
```


### random one liner

```zsh
rg -A10 "INSN PC=0x423d0100" csl.log | grep "index=7.*" -o |sort # search something and print the next 10 lines and grep another text, but print only matching text and then sort.
```


###
// delete emtpy pending changelist
p4 changes -s pending -c yongseok_trace | cut -d " " -f2 | xargs -n1 p4 change -d
