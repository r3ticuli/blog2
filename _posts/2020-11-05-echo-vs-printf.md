---
layout: post
title: echo vs printf
date: 2020-11-05 00:14 -0500
---

today I learned that `echo` appends a `\n` to its input.

If you're doing something like this :

```bash
echo "y" | <some command that prompts [y/N]>
```

You're probably fine with echo. However, if you're doing something like this :

```bash
echo "${some_var}" | <command expecting var from stdin>
```

Here is where the issues begin. Not even `echo -n` could remove the trailing newline (If you know why, please let me know).

I fixed this by swapping `echo` with`printf`. This cost me a couple of hours. From now on I will be using `printf` over `echo` by default.
