# ME 701 -- Homework 1 -- Your Name Here

## Instructions

Your solution should be an update to this `README.md` file that will be
committed back to your repository created when you clicked the HW 1 link.

## Problem 1 -- Open-Source Software

### Statement

Think of the things you do routinely on a computer that require
specific software packages.  Find an
open-source solution from the software repository
for one of these activities and tell me about it in 100 words or less.
For example, I used to do lots of audio recording when I was in
high school (not *that* long ago) and used special (and
pretty expensive) tools like
Cakewalk Sonar.  Since then, I've found an
open-source package for doing multitrack
recording called Ardour that doesn't have all the bells and
whistles but, because I can program in C++ and the
source code is available, I could, in theory,
create any such whistles I need.  **Note**: You may not
describe anything already discussed in class (e.g., the LibreOffice suite
or Octave).

### Solution

Something I have used in the past is Gimp. It's a free, open source alternative to photoshop, aka, a photo editor. I downloaded it a couple years ago to photoshop a few pictures, and it did the job. I wasn't very familiar with the software at the time, but apparently it's the most popular photo editor on Linux. I also just learned that GIMP stands for GNU Image Manipulation Program, which is crazy to me because I had no idea when i downloaded it with windows a couple years ago, before I knew anything about Linux.

[Write your solution here.  Note, in the past, we've used a full, graphical
version of Linux.  With WSL, you probably don't have as direct a path for
exploring software in the Software Manager.  However, use the power of
Google (or AskJeeves) to explore what sorts of open-source software is out
there for technical or other applications.]


## Problem 3 -- Your CPU

### Statement

Figure out how to display information about your CPU via the
command line.  This should include at least the **processor
speed** and the **number of cores**.  Describe your command(s) below.
(Hint: redirection is helpful; remember, that's like
using `ls > directory_contents.txt` to dump the contents of a directory to a file.

### Solution

To display CPU information, I used the following command:
'''bash
lscpu
'''
but that only told me that I have 8 cores. so instead I used this to find the speed for each core:

'''bash
cat /proc/cpuinffo
'''
which told me the speed for each of my 8 cores, and told me that I do, indeed, have 8 of them. My speed for each was about ~2994 MHz.

[
```bash
ls -al # <--- that's not right, but it shows you how to include
       #      code in Markdown!
```
]

## Problem 4 -- Resource Hogs

### Statement

Figure out how to list the programs that use the most
amount of (1) processing and (2) memory.  Describe your command(s)
in your writeup.

### Solution

thinking htop or top or ps aux but I know they're not showing every process.


## Problem 5 -- `bash`

### Statement

Where is `bash` located on your Linux system?  And what version of
`bash` are you using?  Make sure to provide any commands you use to
determine this information.

### Solution
Using the command 

echo "${BASH_VERSION}"

I saw that my bash version is 5.1.16(1)-release.
