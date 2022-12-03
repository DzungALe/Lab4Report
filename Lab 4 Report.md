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

### Second style: Using vim on a remote server
1. Connect to remote server using ssh
2. Use cd to find docSearch
3. Enter commands:

    :set<space>number<enter>12,26s/start/base/g<enter>:wq
4. Test with test.sh

