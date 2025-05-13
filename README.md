# ZSH Config with TMUX
> I used arch for configuring :)
> 
> (that means installation and the whole process will only be document for Arch :()

This project is for people who find it hard to just get a default tmux config with zsh on kitty. The config covers that kitty autostarts tmux and that the shell is being set to zsh. __REMINDER:__ the tmux autostart executes when kitty is starting and __NOT__ when zsh is starting. __WHY:__ There are probably 100 better other ways but in my opinion,this is the fastest and when booting in arch, my terminal couldnt open. 

> the config for tmux is mostly cyan because i like it and theprimeagen said ~~2023~~ 2025 is the year of CYAN
## 1.Installation
### 1.1 kitty
normaly kitty is already installed on arch but we can also check it by typing

``` kitty -v ```

if it returns a version, we are ensured that kitty is installed :)

so now we can navigate to .config/kitty and in there we can create a file called __kitty.conf__. If you dont know how to create a file, its just "touch kitty.conf" or if you have vim installed you can also type "vim kitty.conf"



