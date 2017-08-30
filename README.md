Autocompletion for the xbps package manager
-----------------------
### Dependencies
**Depends on bash-completion because without it, it just doesn't work!**
*if you **can't** use bash-completion then you can just source them in your .bashrc:
```
source /path/to/xbps-install-completion
source /path/to/xbps-remove-completion
```
***One downsize is that it doesn't work with sudo (Unless you maybe change something in .bashrc)***

### Installation
```
git clone https://github.com/lynxcs/xbps-completion && cd xbps-completion
./xbps-completion-update.sh
```
**Copy xbps-install/remove-completion to /etc/bash_completions.d (create the folder if it doesn't exist)**
```
cp /path/to/xbps-install-completion /etc/bash_completions.d/
cp /path/to/xbps-remove-completion /etc/bash_completions.d/
```
**And occasionally run the included update script.**
(Or alias it to xbps-install so it runs after xbps finishes)
(Or do it on system startup)
(You get the idea, you need to run this once in a while.)
### TODO
- [x] Improve Speed (calling xbps-query everytime isn't the best)
- [ ] Improve Speed even further?
- [ ] Combine both completion files into one?
