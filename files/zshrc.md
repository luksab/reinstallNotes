append

```
# Set keymap to de everytime - incase a keyboard is hotplugged
setxkbmap de

# search history with up and down arrow
autoload -U history-search-end
zle -N history-beginning-search-backward-end history-search-end
zle -N history-beginning-search-forward-end history-search-end
bindkey "^[[A" history-beginning-search-backward-end
bindkey "^[[B" history-beginning-search-forward-end

# Map pen and touch to the internal screen
xinput --map-to-output "pointer:ELAN2514:00 04F3:2809" eDP1
xinput --map-to-output "pointer:ELAN2514:00 04F3:2809 Pen (0)" eDP1
```
