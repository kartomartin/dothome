dothome - Karto Martin's .home files
====================================

Karto Martin's home dir configuration files.


Software
--------

* zsh - 
* tmux -
* vim - 
* bash - 
* screen - 
* powerline


Misc Links
----------

### Powerline
https://github.com/powerline/powerline
https://github.com/powerline/fonts

### zsh syntax highlighting with dircolors in realtime
https://github.com/trapd00r/zsh-syntax-highlighting-filetypes.git

### A collection of LS_COLORS definitions; needs your contribution!
https://github.com/trapd00r/LS_COLORS.git

### 🔧 .files, including ~/.macos — sensible hacker defaults for macOS https://mths.be/dotfiles
https://github.com/mathiasbynens/dotfiles

### .files, including ~/.osx — sensible hacker defaults for OS X https://mths.be/dotfiles
https://github.com/BillSantos/dotfiles.git


https://github.com/zsh-users/zsh-autosuggestions#oh-my-zsh

https://github.com/sorin-ionescu/prezto.git




http://openshells.net/
http://newsbeuter.org/
http://www.commandlinefu.com
https://transfer.sh
http://sprunge.us/
http://www.downforeveryoneorjustme.com/www.dr.dk
https://gist.github.com/cirrusUK/35a7642f81097f4e5158#file-tmux-sh




Shell dotfile loading order
---------------------------

###  SH (BASH)
$ sh -l
/etc/profile
/etc/bashrc
~/.profile - $-=himBH       --- sets $ENV
~/.shrc - $-=himBH
$ sh
~/.shrc
$ sh script.sh #!/bin/sh
hello world
$ scp localhost:script.sh script.sh
script.sh    100%    0     0.0KB/s   00:00
$ exit
exit
$ logout
~/.bash_logout - $-=himBH

### BASH
$ bash -l
/etc/profile
/etc/bashrc
~/.bash_profile - $-=himBH  --- sources .bashrc
~/.bashrc - $-=himBH
$ bash
~/.bashrc - $-=himBH
$ bash script.sh #!/bin/sh
hello world
$ scp localhost:script.sh script.sh
~/.bashrc - $-=hBc
$ exit
exit
$ logout
~/.bash_logout - $-=himBH

### ZSH
% zsh -l
~/.home/zshenv - $-=569XZilm
~/.home/zprofile - $-=569XZilm
~/.home/zshrc - $-=569XZilm
~/.home/zlogin - $-=569XZilm
% zsh
~/.home/zshenv - $-=569XZim
~/.home/zshrc - $-=569XZim
% scp localhost:script.sh script.sh
~/.home/zshenv - $-=569X
% exit
% logout
~/.home/zlogout - $-=569XZilm







