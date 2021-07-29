# GVim for Ubuntu

<br>


### Download 

```bash
sudo apt-get install gvim-gnome
```

### settings

```bash
vim ~/home/.vimrc
```

```bash
set expandtab  # tab to space
set ts=4  # 4 space  =  tab
set sw=4  #shiftwidth 
set nobackup #no Backup data 
colorscheme darkblue #background color
set autoindent 
set cindent #for c language
set hlsearch #for hilight

syn on # syntax 
set nu # line number 
set guifont=monospace\ 16 # font

autocmd BufNewFile,BufRead Makefile* :set noexpandtab #exception for Makefile
```
