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
```
