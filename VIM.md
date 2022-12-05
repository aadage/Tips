# VIM Tips


## Resources For Discovering New Tips
Learn Vim  
- http://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/
- [Exploring VIM Series](https://dev.to/vintharas/exploring-vim-4k1i)
- Learn VIM VS Code Extension (Install the "Learn Vim" VS Code extension.  Launch it by typing "Learn Vim" in the command palette.)

Tutorial  
- http://www.openvim.com/tutorial.html

VIMCasts
http://vimcasts.org/


## How to display lines matching a filter  
- http://vi.stackexchange.com/questions/2280/show-only-matching-lines
:vimgrep/pattern/%  
:cwin  


## How to run a macro on all selected lines
:'<,'>normal @q


## How To Encrypt A VIM File
- http://usevim.com/2013/11/01/vim-encryption/
- When you've got an open buffer, before saving type :X in Normal mode. Vim will prompt you for an encryption key twice. Then you can save the file with :w.

 
## How to Install VIM Plugins
- http://howchoo.com/g/ztmyntqzntm/how-to-install-vim-plugins-without-a-plugin-manager


## Sort and Remove Duplicates
:sort u
 

## Fix cursor position while scrolling
:set scrolloff=1000
 
to restore normal scrolling:
:set scrolloff=0
 

## Identify which file/app set a particular setting
e.g.
:verbose set shiftwidth?
:verbose set textwidth

 

## Configure VIM to copy to system clipboard by default
:set clipboard=unnamed


## Ctrl+n
- Autocompletes a word if you type the first few letters then enter the ctrl+n key combination


 
## FOLDING_NOTES
http://vim.wikia.com/wiki/Folding

Essential folding commands
zi            switch folding on or off
za           toggle current fold open/closed
zc           close current fold
zR           open all folds
zM          close all folds
zv           expand folds to reveal cursor
zj            move down to the top of the next fold
zk           move to the bottom of the previous fold
zf  manually add a foldable area
zd  manually remove a foldable area
 
can map the toggle command to a single keystroke (like spacebar):

mapping:nnoremap <Space> za

:help fold-methods

:setlocal foldmethod=indent
 
More folding commands
zo           open current fold
zO          recursively open current fold
zc           close current fold
zC           recursively close current fold
za           toggle current fold
zA           recursively open/close current fold
zm          reduce `foldlevel` by one
zM          close all folds
zr            increase `foldlevel` by one
zR           open all folds



 

 