# Welcome To My Page! 👜
I am Robin and you can access my profile from this link - https://github.com/Rapparicio

I have always considered myself a lifelong learner.  I have been willing to take on big things and to learn from my mistakes.  So when first introduced to the concept of the growth mindset, I thought that this concept was perfectly aligned with what I believed myself to be.  However, when I examined it more closely, I saw that it went beyond my thinking.  It includes actions beyond just learning.  For example, I did not think of celebrating someone else's win as a chance for me to be inspired by it to move me forward.  I would just be willing to celebrate them.  The growth mindset is a set of principles that drive positive action and personal and professional action.  The things that can hold me back are how I react to challenges, obstacles, or criticism.  The opposite is true; the things that will spire me forward are my reactions to these things aforementioned.  **Can I take criticism and learn from it?  Am I willing to continue with something to its completions?** 

##### To Keep A Growth Mindset:
  - Do not fight against a challenging concept; take it head-on and don't complain about it.
  - The adage is true -  *Hard work is its own reward.*
  - Lifelong learners take a risk.
  
# Learning Blog

The first few assignments have been about understanding the need for a growth mindset when it comes to learning something new.  In this case I am learning the basics about 
software development.  It is important to concentrate on the various elements of basic coding in order to set up your web page successfully.  This learning blog is designed highlight some key things. Important elements that go beyond what can be googled. 

## Setting up my pages - Markdowns
According to guides.github.com, > Markdowns are ways to style on the web.> This is an opportunity to use your creative expression.  You decide how your pages will look, 
using bold, italic, lists, bullets, or uploading images.
- [Using the non-alphabetic characters like # or *](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

This is the second page that I have set up in the repository in order to learn by doing.  I am learning how to set up a functioning page with provides the information in a systematic way.   I can optimize the look of my pages by using GitHub pages.

Get comfortable with GitHub
- Typing the @ symbol followed by someone's name will alert them to your project this is useful for teams and for other people you want to view your site. 
- To create a paragraph, live a blank line between the text.

## Chose Text Editors 
Software that is available for download to help write and manage text.  This is incredibly useful according to the article by The Older Coder. 

***What features should you look for in a text editor? I would say some of the most important features are:***

- code completion; 
- syntax highlighting; 
- a nice variety of themes (to reduce eye strain and fatigue); and 
- the ability to choose from a healthy selection of extensions available when you need them. 
You might find some other features that are must-have’s, but I think these features are a good start.


The way one codes is very individualised like a signature.  And the selection of a text editor should be based on needs and ways in which the coder feel most comfortable.  Computers like mine have a built in editor but there are lot of different editors to choose from - Notepad, TextWrangler, BB Edits, Visual Studio Code, Atom, Brackets, as well as Sublime Text.

***IDE- Integrated Development Environment*** 
  1. This is a string of software pulled together, it is an all in one.  
  1. Pulling together features one may like from different text editing softwares. 

**Optimal Use of the Terminal - [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/vi.php)**

**Command line**
A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.
  * Line 1 presents us with a prompt ( robinapparicio@Robins-iMac ). After that we entered a command ( ls ). Typically a command is always the first thing you type. 
  * Important to note, these are separated by spaces (there must be a space between the command and the first command line argument also). 
  * The first command line argument ( -l ) is also referred to as an option. Options are typically used to modify the behaviour of the command. 
    * Options are usually listed before other arguments and typically start with a dash ( - ).
  * Lines 2 - 5 are output from running the command. Most commands produce output and it will be listed straight under the issuing of the command. Other commands just perform their task and don't display any information unless there was an error.
  * Line 6 presents us with a prompt again. After the command has run and the terminal is ready for you to enter another command the prompt will be displayed. 
Opening a Terminal 
  * If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. 
  * An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up

**The Shell,Bash**
  * Within a terminal you have what is known as a shell. 
	This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you.
	If you would like to know which shell you are using you may use a command called echo to display a system variable stating your current shell. echo is a command   which is used to display messages.
1. Shortcuts
  * Here's your first shortcut. When you enter commands, they are actually stored in a history. 
  * You can traverse this history using the up and down arrow keys. 
  * You can also edit these commands using the left and right arrow keys to move the cursor where you want.
1. Print Working Directory - pwd this tells my current or present working directory.
1. List - Is [options] [location ] you can run the command with or without them. 
1. Path- the means to get to a certain file or directory on the system
1. Two types absolute and relative 
1. Root directory ( / ) has subdirectories and files can be in any of the directories
	Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
	Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
1. Paths - 
* ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
* . (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
* .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.
Change directory or cd
If you run the command cd without any arguments then it will always take you back to your home directory.

**Summary** 
file
obtain information about what type of file a file or directory is.
ls -a
List the contents of a directory, including hidden files.
Everything is a file under Linux
Even directories.
Linux is an extensionless system
Files can have any extension they like or none at all.
Linux is case sensitive
Beware of silly typos.
1. Linux Commands
man <command>
Look up the manual page for a particular command.
man -k <search term>
Do a keyword search for all manual pages containing the given search term.
/<term>
Within a manual page, perform a search for 'term'
n
After performing a search within a manual page, select the next found item.
The man pages are your friend.
Instead of trying to remember everything, instead remember you can easily look stuff up in the man pages.

Making a Directory
mkdir - is the way to create a directory 
rmdir - remove a directory
touch - creates a blank file
cp- copy a file or directory 
mv- move a file or directory 

**Summary** 
No undo
The Linux command line does not have an undo feature. Perform destructive actions carefully.
Command line options
Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

**Vi Text Editor**
Saving and exiting
* ZZ (Note: capitals) - Save and exit
* :q! - discard all changes, since the last save, and exit
* :w - save file but don't exit
* :wq - again, save and exit
1. Files in Vi
Below are some of the many commands you may enter to move around the file. Have a play with them and see how they work.
* Arrow keys - move the cursor around
* j, k, h, l - move the cursor down, up, left and right (similar to the arrow keys)
* ^ (caret) - move cursor to beginning of current line
* $ - move cursor to end of the current line
* nG - move to the nth line (eg 5G moves to 5th line)
* G - move to the last line
* w - move to the beginning of the next word
* nw - move forward n word (eg 2w moves two words forwards)
* b - move to the beginning of the previous word
* nb - move back n word
* { - move backward one paragraph
* } - move forward one paragraph

  Deleting Content
* x - delete a single character
* nx - delete n characters (eg 5x deletes five characters)
* dd - delete the current line
* dn - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)

  Undo
Undoing changes in vi is fairly easy. It is the character u.
* u - Undo the last action (you may keep pressing u to keep undoing)
* U (Note: capital) - Undo all changes to the current line
 
**Summary**
No mouse
	
vi is a text editor where everything is done on the keyboard. If you can touch type then this is great. If not then maybe you should think about learning.
Edit commands
There are many of them. Practice is the key to remember the most commonly used and useful ones.

[link to test file](./Test.md)

[Learning Blog](https://github.com/Rapparicio/Robi.Reading-Note-/blob/main/Learning%20Blog.md)	
