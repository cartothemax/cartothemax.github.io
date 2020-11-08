---
layout: post
title:  "grep your history"
date:   2020-11-07 13:06:02
categories: cli
---

My favorite trick when using the command line that has saved me likely hours of time is a simple piping of two common cli tools.

## grep

[`grep`](https://man7.org/linux/man-pages/man1/grep.1.html) is very useful command line tool that perhaps have used for searching of a pattern within a file across your system. I have often used `grep` to search for referenced names within a project for example (I actually used [`ripgrep`](https://blog.burntsushi.net/ripgrep/) but it's really the same idea)

## history

[`history`](https://tldp.org/LDP/GNU-Linux-Tools-Summary/html/x1712.htm) is another fun tool for recalling a command that you typed out but just can't quite remember.

I would be remiss to not also mention that `history` has a built in searching by pressing `ctrl+r`.

## pipe |

[`pipe`](https://www.geeksforgeeks.org/piping-in-unix-or-linux/) is a form of redirection from the command line. It allows you to transfer the standard out of one thing into another.

Functional programming languages often use this pattern to chain together functions. The output of one function is the input into another and so on. Commonly you will use this piping technique to have the output of one command be the input to another.

## grep your history

Now that we have these three founding blocks of tooling we can combine them to great effect!

`history | grep jekyll`

Here is an example of "grepping your history". This example, searching for the [`jekyll`](https://jekyllrb.com/docs/usage/) command, was one that I used while I was writing this post actually.

What is happening here is that `history` returns a long list of all the commands you have used from your terminal. That output is "piped" into the `grep` command that then performs a search for the provided pattern. In this case I simply searched for "jekyll". You could try it out with `cd` or `ls` to try it out (`history | grep cd`).

I will often `grep` my history for complex commands that I once in a blue moon, commands that for some reason that day I just can't get _quite_ right, to search through different usages of a command, and more!

This is such a great example of the "linux way" in which small flexible tools can be combined in powerful and undiscovered utility. A powerful lesson for anyone that writes software. Try to create modular code that solves a single problem well and easily able to interfaced with.
