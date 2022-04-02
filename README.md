# zsh_config

# Install ohmyzsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# Install zplug
```
curl -sL --proto-redir -all,https https://raw.githubusercontent.com/zplug/installer/master/installer.zsh | zsh
```
```
vim .zshrc

source ~/.zplug/init.zsh                                               
zplug "zsh-users/zsh-history-substring-search"                      
zplug "zsh-users/zsh-syntax-highlighting"               
zplug "zsh-users/zsh-autosuggestions"    
zplug "plugins/git",   from:oh-my-zsh    
                                                            
if ! zplug check --verbose; then                                        
    printf "Install? [y/N]: "                                      
    if read -q; then                                              
        echo; zplug install                                    
    fi    
fi                                                                  
                          
zplug load
```
