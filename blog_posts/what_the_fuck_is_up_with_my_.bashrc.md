# What the fuck is up with my .profile?
An annotated guide to cleaning up what looks like a messy piece of shit
```
### ~/.profile
##
# DELUXE-USR-LOCAL-BIN-INSERT (do not remove this comment)
## echo $PATH | grep -q -s "/usr/local/bin" if [ $? -eq 1 ] ; then
PATH=$PATH:/usr/local/bin export PATH fi test -r /sw/bin/init.sh && .
/sw/bin/init.sh

PATH=$PATH:/Ryan.rvm/bin # Add RVM to PATH for scripting

export PATH="$PATH:/Ryan.rvm/bin:/usr/local/lib/node_modules/grunt-cli/bin" #
Add RVM to PATH for scripting

# Custom Prompt
export PS1="\[$(tput setaf 2)\]\W\[$(tput sgr0)\] | \[$(tput setaf 4)\]\u \\$:
\[$(tput sgr0)\]"

## 
# ALIASES
##

## Commands alias prof='vi ~/.profile' alias la='ls -a '

## Applications alias keepalive='ssh root@192.241.219.193'

## Git Aliases alias gs='git status ' alias ga='git add ' alias gb='git branch
' alias gc='git commit' alias gcm='git commit -m ' alias gd='git diff' alias
go='git checkout ' alias gob='git checkout -b' alias gh='git hist ' alias
gha='git hist --all' alias gpom='git push origin master' alias gpru='git pull
--rebase upstream master'

##
# Folder Aliases
## alias cdnom='cd ~/code/nomad-theme' alias cdnom2='cd ~/code/nomad-2' alias
code='cd ~/code'


#THIS MUST BE AT THE END OF THE FILE FOR GVM TO WORK!!!  [[ -s
"/Users/Ryan/.gvm/bin/gvm-init.sh" ]] && source
```
## Sweet Jesus, who wrote this crap!?
The short answer is I have no idea. The long answer is that it's largely pieced together from various install scripts, and Stack Overflow answers, but I've made a few crummy modifications here and there. I'll try to go through and explain some of it and along the way, I hope I can help you, dear reader, add some handy-dandy shortcuts to your .profile that will make your life a lot easier.

```
##
# DELUXE-USR-LOCAL-BIN-INSERT (do not remove this comment)
## echo $PATH | grep -q -s "/usr/local/bin" if [ $? -eq 1 ] ; then
PATH=$PATH:/usr/local/bin export PATH fi test -r /sw/bin/init.sh && .
/sw/bin/init.sh
```

So I'm pretty