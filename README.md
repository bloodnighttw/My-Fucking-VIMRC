
# These files will move to [bloodnighttw/dotfile](https://github.com/bloodnighttw/dotfile)



## My enviroment

~~1. Linux Lite(Ubuntu 18.04 based)~~
~~2. Vim 8.2~~
~~3. Node.js v12.18.2 (coc.nvim need nodejs , check  their [repo](https://github.com/neoclide/coc.nvim)  to see the requirement. )~~
~~4. CPU: intel  Celeron  dual-core processor T1600 (Yeah,Very old and slow)~~
~~5. Ram: 1GB (Poor My Computer)~~
~~6. Terminal: Konsole (with tmux)~~

MY Computer Disk Broken....... QAQ

## Plugin List
### VundleVim/Vundle
- a plugin manager plugin 
### neoclide/coc.nvim
- provide language server function ,it need nodejs to run! pls check their [repo](https://github.com/neoclide/coc.nvim ) to see the requirement.
### vim-airline/vim-airline
- provide statue bar , tab bar and buffer bar(I disable it).
### vim-airline/vim-airline-themes
- airline default theme
### jiangmiao/auto-pairs
- auto complete char like '' [] () {} 
### ayu-theme/ayu-vim
- the theme i use(not use on airline)
### rakr/vim-one
- the theme i use on airline statue bar
### myusuf3/numbers.vim
- line number toggle
### octol/vim-cpp-enhanced-highlight
- cpp syntax highlight (enhanced)
### andymass/vim-matchup
- {} [] () '' highlight when near these char
### bling/vim-bufferline'
- make buffers bar show in statue bar
### ryanoasis/vim-devicons
- icon plugin
### preservim/nerdtree
- show file tree (file manager in vim)
### mhinz/vim-startify
- welcome menu for vim
### christoomey/vim-system-copy
- copy content into system clipboard


## Language Server
### ccls
- A C++/C Language Server
- If You use Linux and have ``snap``,you can install it with command ``sudo snap install ccls `` 
- If not,pls make by yourself.


## Coc.nvim Plugin And Confing 

### coc.snippets
- custom snip complete. Utilsnips supported.

### Config
```json

{
	"languageserver": {
    "ccls": {
      "command": "ccls",
      "filetypes": ["c", "cpp", "c++"],
      "rootPatterns": [".ccls", "compile_commands.json", ".git/", ".hg/"],
      "initializationOptions": {
         "cache": {
           "directory": "/tmp/ccls"
         }
       }
    }
  }
}

```
(This is the config file which let coc.nvim connect to ccls) 
