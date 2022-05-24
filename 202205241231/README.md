# Vim Tutor Notes

## Level 1

h Move cursor left l Move cursor right 

j Move cursor down k Move cursor up 

:q Close file :q! Close file, don't save changes

:w Save changes to file :wq or :x or ZZSave changes and close file

x Delete character at cursor i Insert at cursor 

I Insert at beginning of line

a Append at cursor A Append at end of line

escape or ctrl+\[  Exit insert mode

## Level 2 

dw Delete word d$ or D Delete to end of line

w Next word $ Go to end of text on current line

^ Go to beginning of text on current line 0 Go to beginning of current line

2w Go two words forward 3e Go to end of third word ahead d2w Delete two words

dd Delete entire line 2dd Delete two lines 

u Undo last change U Undo changes on entire line

ctrl+r Redo change

d = operator

w = motion

[number] = amt. of times to repeat motion/operation 

## Level 3 

p Paste after cursor P Paste before cursor 

r Replace character under cursor cw Change wordc $ or C Change to end of line 

c2w Change two words

c = change  can use same motions as d  

## Level 4

50gg/50G or :50 Go to line 50 G Go to last line in file

gg Go to first line in file /waldo Search for "waldo" 

n Go to next search result N Go to previous search result 

?carmen Search backwards for "carmen" ctrl+o Jump to previous location (jump back) 

ctrl+i Jump to next location (jump forward) % Go to matching parentheses or brackets 

:%s/bad/good Replace bad with good in current line :%s/hi/bye/g Replace hi with bye in entire file

:%s/x/y/gc Replace x with y in entire file, prompt for changes

:#.#s/old/new/g  Substitute phrases between two line #'s type 

## Level 5 
:!ls Run shell command ls v Open visual mode

 vw Visual select word vwd or vwx Visual select word, then delete word
 
 :w play.rb Save current file as "play.rb" :r hat.rb Read in file "hat.rb"
 
 
 :r = Pulls file in from outside workspace
 
visual = is like highlight mode to copy paste or whatever operator you want to use



## Level 6

o Open new line below O Open new line above

 e Go to end of word 2e Go to end of next word 
 
 a Append after cursor R Enter replace mode
 
 yw *Yank* word vwy Visual select word, then yank y$ Yank to end of current line 
 
 set ignorecase or set ic Change search settings to ignore case 
 
 set noignorecase or set noic Change search settings to use case
 
 :set hls  Highlights search :set nohls to turn off
 
 
 # Level 7
 
  Type  :help  or press <F1> or <HELP>  to open a help window.

  Type  :help cmd  to find help on  cmd .

  Type  CTRL-W CTRL-W  to jump to another window.
  
  Type  :q  to close the help window.

  Create a vimrc startup script to keep your preferred settings. .vimrc

  When typing a  :  command, press CTRL-D to see possible completions.
  Press <TAB> to use one completion.
