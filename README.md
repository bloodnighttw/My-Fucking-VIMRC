# My Fucking VIMRC 

The repo share my ``.vimrc`` to other and backup it.

I use VIM for c++ (mainly) or python coding,use Jetbrains Intellij IDEA with VIM Plugin for java coding.

NOTE! I am not the master of VIM , ** BUT VIM REALLY HELP ME RISE THE SPEED OF CODING , AND YOU SHOULD TRY IT IF YOU ARE WRITE C++ OR PYTHON **

## Q&A

Q1: Why VIM ?

A1: VIM is Fast,Lightweight,and if you have learned how to use VIM , VIM will speed up your speed of coding!

Q2: Can I Copy it to my ``.vimrc``?

A2: Yes,of course.

Q3: Can I use this ``.vimrc`` to write Python?

A3: Yes. Just Type ``:CocInstall coc-python`` inside the VIM(In Normal mode) , and coc.nvim will install the python plugin and language server.

Q4: Can I use this ``.vimrc`` to write JAVA?

A4: Yes. ** BUT I DON'T RECOMMAND YOU TO USE ``coc-java`` TO WRITE JAVA CODE BECAUSE JDT.LS IS NOT POWERFUL AS OTHER IDE(I THINK) .** Try Jetbrains Intellij IDEA with VIM Plugin!It will also speed up your speed of coding.

Q5: Other Language?

A5: You Should search by yourself. Try Google "coc.nvim XXX" (XXX is your language name),I think there will have a result.

## My enviroment

1. Linux Lite(Ubuntu 18.04 based)
2. Vim 8.2
3. Node.js v12.18.2 (coc.nvim need nodejs , check their repo to see the requirement. )
4. CPU: intel  Celeron  dual-core processor T1600 (Yeah,Very old and slow)
5. Ram: 1GB (Poor My Computer)
6. Terminal: Konsole (with tmux)

## Here is the links.
[coc.nvim](https://github.com/neoclide/coc.nvim).

## Plugin List

### neoclide/coc.nvim
- provide language server function
### vim-airline/vim-airline
- provide statue bar , tab bar and buffer bar
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
- make buffers bar in statue bar
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
- If You use Linux,you can install it with command ``sudo snap install ccls ``
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

