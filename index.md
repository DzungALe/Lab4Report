# Lab 4 Report

## Part 1. Change all "start" parameters to base

There are different instances of start in the code, and we need to replace all of them and change it to base. To do this, we will we use the commands below:

    :set<space>number<enter>12,26s/start/base/g<enter>:wq

This will require the shortest number of strokes possible to replace every instance of start into base
___
## Part 2. Styles of editing
### First style: Editing on local
1. Use Ctrl + f or select find/replace to find all instances of start
2. Replace start with base
3. Ctrl + s to save file
4. Move on to local terminal. Use scp to copy file onto a remote server
5. Connect to remote server using ssh
6. Run bash test.sh

This process was slower than remote for sure, simply because I knew what commands to put when working with vim.

### Second style: Using vim on a remote server
1. Connect to remote server using ssh
2. Use cd to find docSearch
3. Enter commands:

    :set<space>number<enter>12,26s/start/base/g<enter>:wq
4. Test with test.sh

This was faster, but only just. The time it took for me to edit in vim and type the commands to edit in vim made it shorter but still tedious in some ways.

### Questions

Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?

I prefer to work on the local machine right now simply because I am still accustomed to a local environment. While working locally did take longer than remote, this was due to me only using commands from the command line. Plus, there are tools like WinSCP or MobaXTerm that I've been using to help me secure copy files onto a remote machine, which is just as fast as working remotely. 

What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)

Well, some programs run on Linux better than on Windows. For example, while bash does not run on Windows, it runs on Linux just fine, so it might be better if I work with some things like bash on a completely remote environment as opposed to my local Windows machine. However, with most programs, I think using a local machine will work just fine.

