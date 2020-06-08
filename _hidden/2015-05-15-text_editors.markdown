---
layout: post
title:  The search for a perfect text editor
date: 2020-05-15
description: My search for a perfect text editor
---

# DRAFT


### Word
My quest with text editors began before I really got into coding. I was tired with microsoft word. I have never liked software that had loads of functionality that I never used. Especially if that functionality translated into long load times. 5 second load times are pointless if all you want to do is edit text. Besides, all the functionality gets in the way and takes up screen real-estate.

### Evernote
While I was writing and taking notes, I had many documents that were very short. Opening them up in word was too slow. So I tried services like Evernote. I did enjoy using them, and they helped me manage many small notes well, yet I was still frustrated by its speed. I sometimes wanted to edit a single note, without having to open the whole interface and see all of my other notes from all time.

### Notepad
I started using notepad. Which was great. Simple, fast, easy. My notes were light and I could just use a folder structure to organize things. Yet I did miss some functionality. I also wanted to customise the look of notepad and so I moved to notepad++.

### Notepad++
I stuck with notepad++ for a long time. I defined custom syntax that was similar to markdown, though I had never heard of markdown. To do things like enable folding, make text **bold** and other things like that. I used the project functionality and experimented with plugins. That said I was never really happy with the way projects worked (I still haven't found one that I don't have any problems with).

### Sublime Text
Then came Sublime Text. I had installed it once before but I uninstalled it quite quickly. Partly because it seemed far too big for what I wanted, and then I found out that the preferences were adjusted by modifying a huge `json` file and I ran. I didn't know what `json` was and I didn't understand it.

I came back to it when the Python coding course I had signed up to recommended it. It was then I came to appreciate how simple it really was. It did have more functionality than notepad++ but most of it came from plugins which were very easy to install and manage thanks to the Package Control plugin.

I never gave up on notepad++ completely though, it is still my editor of choice when I have to edit single files. It opens fast and has enough syntax highlighting to get by. I uninstalled most of the plugins and have it as my 'quick and dirty' editor.

### VB Editor and "heavyweights"
When I got into Excel VBA I inevitably started using Microsoft's GUI. Its minimal syntax highlighting was hard to bear. The lack of multi-highlights, multi-cursors and many quality of life features were sorely missed. That said, its search and debugging features were great. This led me to adopt Pycharm, just for its step debugging. I am sure that there is probably a lighter CLI version but I haven't found it yet.

Pycharm so far I use exclusively for its step debugging. The rest of it annoys me. The way it creates a .idea folder I am sure has its reasons, I just hate to see extra files in my file manager. Plus I have to remember to `.gitignore` it.

Recently I came to appreciate Visual Studio Code. Its a heavyweight, which I dislike. Yet it has that magic property of "just working". Its terminal seems to work better than anything else on Windows. Git integration is easy. Syntax is up to date. Plugins are easy to install. It also extremely popular. I see myself using it more and more. Possibly to replace Pycharm. Yet for now I use it for its terminal and git when ConEmu is not playing nice. Or to modify Linux files.

### Abricotine
I used sublime in general as my markdown editor, along with some plugins but needed something that gave me an immediate preview. I tried many other editors like Markdown Pad, but the double pane preview I was never really convinced with. Getting the combination right of supporting highlighted code blocks, reliable export, custom CSS, lightweight, fast with real-time "transparent" preview was hard to find. Until I came across Abricotine which does all this.

### My setup

Notepad++ is my lightweight tool for quick edits and fast notes.
Sublime Text is my preferred element for projects and general coding.
Abricotine deals with all my markdown.
The "heavyweights" VB Editor, Pycharm and VS code - for specific tasks that I am sure there is some lightweight modular alternative to do the tasks I need, but when I am frustrated and need a solution, they usually have what I need. Still takes a few minutes to fire them up though.


