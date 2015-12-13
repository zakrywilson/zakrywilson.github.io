---
layout:		  post
title:			Remove the training wheels and use VIM
date:			  2015-11-29 14:57
summary:		Why I use VIM, why you should use it, and how to become faster with it
categories:	VIM
---

## First: my personal experience with VIM
When I first started programming years ago, I began, like most people, with finding a basic text editor---quickly developing a predilection towards neat syntax highlighting and visually pleasing color schemes. After learning C, I moved onto learning Java and discovered the IDE: *the most powerfully amazing tool ever to exist*---tool that told me what methods existed on an object, automatically imported all the libraries I needed, and caught all my silly syntax errors. I loved using Eclipse and products created by JetBrains (in fact, I still like using JetBrains' products for larger projects). The problem was, I wasn't bettering myself as a programmer: I wasn't *really* learning the syntax as well as I should; I wasn't being mindful of what classes existed in what libraries. The IDE lessened the learning curve while lessening my learning in general. 

I eventually took a class in UNIX which forced me to use VI for my assignments. It was terrible: I could barely do anything. I only knew `:wq` and how to switch between *command* and *edit* mode. `Backspace` was my only friend in those dark days. When people would tell me that they used VIM, I was always shocked. *Why do they choose to live in the Stone Age?* 

I then did my research and found that VIM, like a classic work of art, has stood the test of time for a reason.

## So why use VIM?
In my experience, each developer seems to have their own reason for choosing VIM. Here are some of the reasons I think VIM is something every programmer should at least give a whole-hearted try. Note that VIM is *VI "improved"* but whether it's actually an improvement is subjective. Regardless, it has added functionality that many find useful.

#### Increase in efficiency
VI was developed with the intent of speed: programmers who write code using a mouse or a track-pad and arrow keys are wasting small amounts of time every time they switch between the two. The reason for this is simple: it takes time for your hand to move from the keyboard to the mouse and vice versa. Multiply that time by the amount of times your hands make that adjustment in your lifetime... I've never done the calculation, but the assumption is that it's a lot of wasted time. The alternative is to keep your hands in the same position, thus reducing wasted time. VI was designed to allow its users to keep their hands in the same area to elicit an increase in productivity. And who doesn't enjoy speed?

#### It's a convention
VI exists on almost every Linux system. If you need to write/edit code on a Linux system, you don't have to take the time to go download your favorite text editor or endure using whatever is provided; you can go right to work in an editor in which you're already comfortable.

#### Bettering yourself as a programmer
I think that for any programmer who wants to become more well-versed in any language would do well to drop the text editor or IDE and switch to VIM or Emacs. The other reason I have found VIM to be useful in forcing me to do things without the aid of an intelligent program is that it's very useful for interviews. At some companies, especially the top 4, you'll most likely be asked to write code on a whiteboard. If you're completely reliant upon an IDE to do things like create `main` for you, catch your small syntax errors, and manage your imports, you might find yourself in an awkward position during an intense interview.


## My VIM settings
Now I'm no hardcore VI guy: I use VIM and I have a decent amount of customization that makes things a little less old-school. If you want to try out my settings, you can find them [here](https://github.com/zakrywilson/vim-customization).

![My VIM](http://i.imgur.com/qQIez5a.png)

#### A very small intro to the .vimrc file
For those of you who don't know this, inside your home directory, you can customize your VIM settings by editing/adding the `.vimrc` file. In this file, you can specify tab sizing, whether or not you want line numbers or syntax highlighting, etc.

#### My preferred color scheme
I have tried many color schemes, but I have found [molokai](https://github.com/tomasr/molokai) to be my favorite.

#### Really taking it to the next level
If you want to really take your VIM skills to the next level and---in the end---increase your VIM speed even more, you can add these to your `.vimrc` file: 

* Remove arrow keys functionality
* Remove mouse/track-pad scrolling ability
* Remove ability to hold down navigation keys

You don't need arrow keys: use the navigation keys that are already under your fingers: `h`, `j`, `k`, and `l`. The navigation keys are great for jumping over characters, but they were not intended to be the *only* method for navigating your file. There are much better alternatives such as `w` to jump forward one word and `b` to jump backwards one word. There are also commands such as `$` to jump to the end of the line and `^` to jump to the beginning. There are many different commands to move around in VIM. If you want to learn more, [this](http://vim.rtorr.com/) might be a good starting point. There exists a plugin for VIM called [hard mode](https://github.com/wikitopian/hardmode) that disables the ability to use things like arrow keys and h, j, k, and l. The reason for this is that there are far better ways of navigating when you're writing code than using the arrow keys or your mouse. The problem is, you need to kick the habit so you can fully embrace the power of VIM.

I think another feature people who are new to VIM are not aware of is that VIM does almost everything you would want out of an editor. For example, `:4,22 >` will indent lines 4 through 22 by one tab. There are more goodies like this, you just need to look, and you'll find them. 

## Conclusion
Starting off with VIM is a steep learning curve---steep enough that most people give up, but it's worth it. In time, you'll become more efficient in your programming. It's worth a shot... so try it.
