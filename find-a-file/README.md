> :construction: TK-TODO: Add screenshots.

## Objective

In this exercise, participants are asked to locate a particular file within a large directory tree.

## Tools Introduced

* `ls`
* `cd`
* `grep`

### Additional Optional Tools

* `tree`
* `less`

## Description

When the [Find-A-File](https://github.com/aubrel/iointrotocmdline/tree/master/find-a-file) repository is downloaded (we assume that because these tools are being used to introduce basic command line concepts, the user has not yet learned how to use `git clone` from a command line), the user acquires several directories, nested within the `find-a-file` directory. Within the `find-a-file` directory, there are many directories containing many files. In one of these files in one of these directories, there is the file we want. The keyword to use to find this file is located _within_ the file; it is not the file name.

**Solution:**
* Use `grep -r` to locate a file within a large directory tree:

`grep -r VICTORY`

## Suggested Walkthrough

While these materials can be used to introduce basic concepts in any way, here is a walkthrough you can use if you'd like some guidance.

1. Introduce the point of this exercise:
    * We are going to be trying to locate a particular file in a large directory tree, which is very much like finding a needle in a haystack.
    * The other condition of this exercise is that we don't know what the _name_ of the file we are trying to locate, and there are many files within the tree that have the same names. Thus, we are trying to locate content _within_ a file, as opposed to the _name_ of a file.
    * Luckily, we do have a clue: we have a "keyword" to search for: `VICTORY`.
1. Participants [download the Find A File repo](https://github.com/aubrel/iointrotocmdline/tree/master/find-a-file) somewhere easily accessible on their machines.
1. Participants launch their command line application.
1. Introduce `ls`, so that participants can see the directory in the command line. Compare the GUI view with the CLI view, to demonstrate the sameness between the two.
1. Introduce `cd`, and have participants change directories into the `find-a-file` directory.
1. `ls` to see what the directory contains. Explain the concept of a directory tree. **Optional:** Introduce `tree`, so participants can view the directory tree and all contents of the directories visually.
1. Introduce `grep`, and its relevant `man` page.
1. Explain that the `-r` option is required due to the recursive search across many directories and files; introduce the concept of recursion.

> TK-TODO: Finish this README!
