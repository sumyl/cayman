---
layout: default
---

## Command-line course

The aim of this course was to introduce the command-line usage of a UNIX-like system. In 
addition the course also consisted of version control systems and compiling software.
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/Unix_timeline.fi.svg/800px-Unix_timeline.fi.svg.png" alt="Unix" hspace="20"  align="left"/>
 
|Week 1| Introduction to Command-Line Environments|
|Week 2| Navigating UNIX System|
|Week 3| Corpus Processing|
|Week 4| Scripting and UNIX Configuration Files|
|Week 5| Installing and Running Programs|
|Week 6| Version Control|
|Week 7| Building Webpages using GitHub Pages|

### Week 1: Introduction to Command-Line Environments

Introduction to the topic of the course, the basics of command-line. We learned how to use 
command-line and to create and edit files using it.
This command outputs word "hello world".
```bash
echo hello world
```
### Week 2: Navigating a UNIX System

During the second week we learned about UNIX filesystems, their hierarchies and how to create, 
move and destroy directories and files. We learned also to navigate through system using both 
absolute and relative paths.
At the same time we learned also to connect remote UNIX machines using SSH connection, and to 
transfer files securely with SCP.
```bash
cd ~/cmdline_course
```
Using this command one can navigate to the directory named _cmdline_course_ in their home directory
### Week 3: Corpus Processing

The focus of the third week was corpus processing, i.e. how to
modify text files, their content and create new files. During this we learned about pipes and 
regular expressions as well as differences of using ASCII and UNICODE.
```bash
./script.sh
```
This way one can invoke a shell script in the current directory
### Week 4: Scripting and UNIX Configuration Files

On the fourth week we continued with manipulating text files, but instead of manual labour we 
created our first scripts to automate their usage. At the same time we got basic understanding 
about UNIX environmental variables.
```bash
source ~/.bashrc
```
Using _source_-command one can force the current shell (bash) to read again the variables and other
configuration from the file containing them.
### Week 5: Installing and Running Programs

On the fifth week we installed new programs as well as run existing ones. We learned difference 
between installing programs made with different languages, mainly translated language as 
Python and complied ones as C.
We also learned to compile software ourselves from source code, and how to utilize Makefiles 
to automate usage of scripts.
```bash
./configure
make
```
Using these commands one may configure the environment for being able to compile source code 
in current directory (using the _configure_-script that lies there) and then complie the 
program
### Week 6: Version Control

Version control systems were focused on sixth week, and we learned to create a Github account, 
repository and modify it on our own machines. We also learned about meaning and usage of 
branches as well as merging and discarding changes.
Git workflow:
1. Clone repository
```bash
git clone <url>
```
2. Make changes
```bash
nano newfile.txt
```
3. Create files and commit changes
```bash
git add newfile.txt
git commit -am"New file"
```
4. Push changes to remote repository
```bash
git push
```


### Week 7: Building Webpages using GitHub Pages

The last week we introduced ourselves to Github Pages, which included also the basics of Markdown 
and Jekyll, which is a quite handy tool for creating web pages. Unfortunately it was not too 
straightforward to utilize, as we had to solve a few problematic dependency chains to be able 
to install all required components.
```bash
bundle install 
bundle exec jekyll server
```
These commands install the Ruby packages required for using Jekyll, and then start jekyll
server using files in current folder, so that user may visit the created page from their
own computer (the started Jekyll-server runs only on the same computer)
