#[vim](https://my.mindnode.com/dsyhczzfLsBAG4EpFt5TZnBYWAD9mfc9ms7nPMCz) 👾

![](http://i.imgur.com/3g9bJWV.jpg) 

#mindmap index 🗄️

# neat


## in normal mode

# neat


## in normal mode

### vi(

- inside brackets, go to visual mode and select text inside the brackets

- where ( can be any other symbol

### va(

- inside brackets, go to visual mode and select text AND the brackets

## search and replace

### :%s/foo/bar/g

- in all lines

- find each occurrence of ‘foo’

- replace with bar

## gg=G

### will indent code


# [vim plug](https://github.com/junegunn/vim-plug)


# todo


## look into macros

## make mapping to source vim settings for current file

## learn text objects

### read

- [definitive guide](http://blog.carbonfive.com/2011/10/17/vim-text-objects-the-definitive-guide/)

## json comments are red

### really annoying


# terms


## text objects

### are blocks of text with a starting and ending point

### when you use a motion, conceive of that as an operation that is creating a dynamic text object that is delimited by the starting and ending cursor position

## [buffers](http://joshldavis.com/2014/04/05/vim-tab-madness-buffers-vs-tabs/)

### is text that you are editing

### i.e. when you open a file, the content of the file is loaded into a buffer


# macros


# tricks


# normal mode


## (⇧) shift mappings

### ⇧ + v

- visually select current line

	- then can move up and down with j k

	- ⇧ + v n j

		- visually select next n lines

	- ⇧ + v n k

		- visually select previous n lines

## commands

### d

- delete

- df<x>

	- delete until next x

- dF<x>

	- delete until previous x

- dt<x>

	- delete until x

### f

- f<char>

	- will go to next character

- F<char>

	- will go to previous character

## useful

### go to beginning of line

- 0

	- always moves the cursor to the "first column"

- can also use ⇧ + I

	- to move and switch to insert mode

## ^

### jump to start of line

## $

### jump to end of line

## G

### jump to end of file

### 2G

- jump to line 2

- where 2 is number of lines

## w

### go forward one word

## b

### go back one word

## x

### delete sign under cursor

## dd

### delete line

## d

### works like cut

## y

### yank = copy

## p

### paste

## Y

### copy line

## i

### insert mode at cursor position

## a

### insert mode at next cursor position

## A

### insert at the end of line

## o

### insert in next line

## O

### insert in before line

## H

### brings me to top of current window

## M

### brings me to the middle

## v

### go to visual mode

## 0

### goes to beginning of the line

## D

### delete line after cursor

## GA

### go to bottom of file

## da

### delete until start of next word

## rx

### replace currently selected characters with x

## ce

### replace until the end of word

## dgg

### delete text to top of file from cursor

## zz

### put current line to middle of screen

## zt

### put current line to top of screen

## zb

### put current line to bottom of screen

## .

### will duplicate the above line

## nk

### where n is the line number you choose to go up to certain amount of lines

## gg

### go to beginning of file

## Vu

### lowercase whole line

- V - selects the entire line in visual mode

- u - lowercases the selected area

## ggVGu

### lowercase the entire file

- gg - goes to first line of text

- G - goes to end of file


# ⌃ in normal mode


## ⌃v

### visually select current line

## ⌃e

### go down a page while keeping the cursor in place

## ⌃y

### go up a page while keeping the cursor in place


# insert


# ⌃ in insert mode


## ⌃p

### text completion, browse down

## ⌃n

### text completion, browse up

## ⌃x

### enter special insert mode

- RESEARCH: 

## ⌃f

### filename completion

## ⌃l

### context aware line completion


# command mode


## :x

### saves and quits from the file

## :map

### see all currently defined mappings

## :verbose map

### know where each mapping was defined


# ⇧ in normal mode


## ⇧4

### goes to the end of the line

## ⇧H

### go top of screen

## ⇧M

### go middle of screen

## ⇧L

### go bottom of screen

## ⇧V

### highlights current line


# resources


## text objects

### [definitive guide](http://blog.carbonfive.com/2011/10/17/vim-text-objects-the-definitive-guide/)

## [you don’t grok vi](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/1220118#1220118)

### great answer

## [coming home to vim](http://stevelosh.com/blog/2010/09/coming-home-to-vim/)

## [from novice to professional](http://derekwyatt.org/vim/tutorials/novice/)

### TODO: go through

## [vim casts screencasts](http://vimcasts.org/episodes/archive/)

### TODO: watch


# motions


## Motions are in most cases the second part of an entire command you want to execute when working with Vim.

## You apply them during the so called **Operator-Pending Mode**, which is the little time frame where you apply a "target" to built-in commands such as d, y or c.

## Let's say you want to delete from the current cursor position until the next occurrence of the letter r. You do that with the t command which brings your cursor in front of the next occurrence of the given characer. So typing dtr in Normal Mode could be read as Delete until next 'r'. The basic pattern of the d command is d{motion} and you can use any kind of motion there.


# visual mode


## v/foo

### will select from my current position to the next instance of “foo”

## V

### go to visual line mode (one line at a time)


# text objects


## Text-objects can be used in context of motions.

## They are a bit more clever than normal motions because they can act in both "directions."

## For example, whereas the w command in Normal Mode is a motion to jump to the next word, iw is a text-object that operates inside the current word.

## Where "inside" means "this word excluding the surrounding spaces".

## So, to delete a word you can compose commands like diw or daw for around a word. 

## There are text-objects for paragraphs (ip, ap), sentences (is, as), HTML tags (it, at) and Vim is even smart enough to act on the current function block (i{, a{).

