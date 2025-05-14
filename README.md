# ZSH Config with TMUX
> I used arch for configuring :)
> 
> (that means installation and the whole process will only be document for Arch :()

This project is for people who find it hard to just get a default tmux config with zsh on kitty. The config covers that kitty autostarts tmux and that the shell is being set to zsh. __REMINDER:__ the tmux autostart executes when kitty is starting and __NOT__ when zsh is starting. __WHY:__ There are probably 100 better other ways but in my opinion,this is the fastest and when booting in arch, my terminal couldnt open. 

> the config for tmux is mostly cyan because i like it and theprimeagen said ~~2023~~ 2025 is the year of CYAN
## 1.Installation
### Git
git is essential for this part cause of the oh-my-zsh config so it install it via

```
sudo pacman -S git
```
### 1.1 kitty
normaly kitty is already installed on arch but we can also check it by typing
```
kitty -v
```
if it returns a version, we are ensured that kitty is installed :)

so now we can navigate to .config/kitty and in there we can create a file called __kitty.conf__. If you dont know how to create a file, its just "touch kitty.conf" or if you have vim installed you can also type "vim kitty.conf".
### 1.2 zsh
for the theme and everything we are using oh-my-zsh
theyre github repo: https://github.com/ohmyzsh/ohmyzsh.
zsh is a shell that is mostly already installed but we can check by typing
```
zsh --version
``` 
if it isnt installed we need to type
```
sudo pacman -S zsh
``` 
now that we have it installed we can set it to the default shell
It can be set to default shell by typing this 
```
chsh -s $(/bin/zsh)
``` 
if it doesnt work, here is a link for preciser documentation
https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

now we can check by typing
```
echo $SHELL
```
this echos (prints) the environment variable for the shell

now we can install oh-my-zsh for the theme that we are going to use.first we check if we have curl installed by typing
```
curl --version
```
now we can type:
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
now that we have installed everything, we can finally configure the shell. To do that we need to create a file called .zshrc in the directory ~/ (its the user directory and the config is also going to be for that one user. If you want to use it systemwide, you can check out official documentation) In that file we are going to paste my config that is in the repo (the file is also called .zshrc)
NOW WE GOT ZSH WORKING WUHUU!!!

### 1.3 TMUX 








