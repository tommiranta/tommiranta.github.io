---
layout: post
title: "Work ergonomy from a coder's perspective"
date: 2022-11-07
tags: coding
---

foo. We all know the importance of a good bed — we spend one third of our time in
one. As a worker in the software industry I spend an equal amount of time in
front of a computer. That got me thinking about what I can do to improve work
ergonomy and what tools to use to make my time coding as pleasant as possible.
In this article I will go beyond the good chairs and height-adjustable
tables and show you what I've done so far.

![My desk](/assets/images/2022-11-07-coders-work-ergonomy/setup.jpg)

## Typing comfort

One year ago a friend suggested that I try a mechanical keyboard. I knew
they existed, but I had never given them much more thought thinking it's something
gamers use. Little did I know that it's possible to go deep down
the rabbit hole and spend unreasonable amount of resources in the search for
the perfect [THOCK](https://www.youtube.com/watch?v=_pA7WDsoBzk) sound. :sweat_smile:

What I learned was that there is a myriad options to configure your keyboard
to your liking. The options are not restricted to switches and keycaps. You can
also build your own keyboard from a kit. This is where you can take writing
comfort to the next level. [Split keyboards](https://golem.hu/boards)
allow you to keep your arms in a more natural position while typing. You can
choose from tens of different models, each with its distinctive form factor and
amount of keys. A more compact model requires less movement of your hands
while typing.

You might wonder how to use a keyboard with 40 keys. The answer
lies in thinking about your keyboard as having layers and toggling between
these to get access to all the necessary characters. It's essentially the same
thing you do when using your modifier keys (shift, ctrl/command, alt/option) on
your normal keyboard. You can configure the keyboard layout by modifying
the keyboard firmware. Popular alternatives are [QMK](https://qmk.fm/) and
[VIA](https://www.caniusevia.com/). QMK offers more options, but with a slightly
higher learning curve. This is not a problem for a programmer. VIA
offers easy configuration using their website, but you have fewer options to
access advanced keyboard firmware features.

![Lumberjack](/assets/images/2022-11-07-coders-work-ergonomy/lumberjack-1.jpg)

I built my first keyboard this autumn, a [Lumberjack](https://github.com/peej/lumberjack-keyboard).
It uses an orthogonal key layout and separates the hands from each other so
that I don't need to keep them as close as on a regular keyboard. This is my
transition towards building a split keyboard, which will be either a
[Corne](https://github.com/foostan/crkbd) or a [Skeletyl](https://github.com/Bastardkb/Skeletyl).

## Coding comfort

Let's look at what you can do to improve ergonomy with the help of software,
now that we have covered the hardware. The goal is to not have to switch
between using your keyboard and mouse. In other words, we need to maximise the
use of the keyboard. I use the [Neovim](https://neovim.io/) editor and the
[tmux](https://github.com/tmux/tmux/wiki) terminal multiplexer. This way I can
work on different project workspaces/repositories at the same time and
seamlessly switch between them. The figure below illustrates my approach.

![Tmux](/assets/images/2022-11-07-coders-work-ergonomy/tmux.jpg)

Tmux lets me create separate terminal windows. You can split a window into one
or more panes. The windows listed at the bottom of my screen represent the repositories
I'm working on. The pane on the left side is my main pane where I have my code
editor. On the right side I have two panes for terminal use. I move
between the windows and panes using keyboard shortcuts.

What makes Vim/Neovim different from other editors is that they have
different modes. In _normal_ mode you can use keyboard commands to navigate within
your file. In _visual_ mode you can select fractions of code before taking
actions on it, such as copy/change/delete. In _insert_ mode you can write text
as you would in any editor. There's also a _command_ mode that allows you to
run editor commands. The existence of normal and visual mode is what replaces
the need for a mouse in regular editors, such as VS Code. There is a learning curve
when transitioning to Neovim, but I'm happy to have made the effort to learn it.

Neovim is highly configurable and you can extend it using plugins. What distinguishes
these plugins from e.g. VS Code extensions is the variety of plugins available.
They range from small utility-like plugins that improve your editor's usability
and efficiency all the way to integrations to language servers that offer
linting, code formatting, auto-complete etc. Everything you'd expect from a
full fledged IDE. Setting up and personalising your configuration files, or
[dotfiles](https://driesvints.com/blog/getting-started-with-dotfiles/) to be
specific, is an involved process. The benefit is that you can store them in
version control and even use a [dedicated tool](https://www.chezmoi.io/) to manage
your dotfiles. You'll be able to check out the dotfiles on another computer and
within minutes have the familiar setup in front of you, ready for work!

## Closing words

I hope to have sparked some interest into improving your work ergonomy using
the tools and tips mentioned. It requires a bit of time and willpower to get
started, but it's well worth the effort. Even an old dog can learn new tricks!

![Building in progress](/assets/images/2022-11-07-coders-work-ergonomy/building-1.jpg)
