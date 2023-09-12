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



## How to run a macro on all selected lines
:'<,'>normal @q


## How to Install VIM Plugins
- http://howchoo.com/g/ztmyntqzntm/how-to-install-vim-plugins-without-a-plugin-manager


## Sort and Remove Duplicates
:sort u
 

## Fix cursor position while scrolling
:set scrolloff=5
 
to restore normal scrolling:
:set scrolloff=0

- scrolloffset (scrolloff for short) adds the configured number of lines as padding above or below the cursor when moving
  the cursor up or down the file.  
- simplest way to understand this is to open a file that is large enough to require scrolling, set a value, then press
  j or k to move the cursor up or down.  When you get near the top or bottom of the page you'll see that the page will
  scroll to keep the configured number of lines visible when scrolling
 

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

## Enable/Disable Line Numbers
to enable line numbers
  :set number

to disable line numbers
  :set nonumber


## Capitalize Letter Under The Cursor
Can capitalize the letter under the cursor by typing ~



## Movement
NOTE most movement commands can be preceded by a number to repeat the command that many times.
  e.g. 
    w moves to the beginning of the next word, 3w moves forward 3 words.
    j moves one line down, 3j moves 3 lines down.


h - move one character left
j - move one line down
k - move one line up
l - move one character right

e - move to end of a word
    - 3e - move to the end of the third word
E - same as e but treats non-whitespace chars as part of the word
w - move to the beginning of a word
    - 3w - move forward three words
W - same as w but treats non-whitespace chars as part of the word
b - move backward to the beginning of a word
B - same as b but treats non-whitespace chars as part of the word

$ - move to the end of the line
^ - move to the first non-blank character of the line
0 - move to the beginning of the line
) - jump forward one sentence
( - jump backward one sentence
} - jump forward one paragraph
{ - jump backward one paragraph

H - jump to top of visible page
M - jump to the middle of the visible page
L - jump to the bottom of the visible page

gg - jump to top of file
G - jump to bottom of file
nG - jumps to line n
    example: 10G - jumps to line 10

BABIF - explore all movement commands: see https://vim.fandom.com/wiki/Moving_around



## WHEN I REACH THE BOTTOM FIND A NEW TIP TO ADD TO THIS LIST 
- add a movement section that groups all of the movement commands together
 

 fiddle.dee.foo doodle.dee&dooB

