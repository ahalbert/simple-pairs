Simple Pairs.vim
=================

This is a fork of [vim-scripts/simple-pairs](http://github.com/vim-scripts/simple-pairs).

**My changes:**

* Added an option to disable simple-pairs. I find this useful for writing english words in vim.

Original README
--------------------

This is my first attempt at writing a vim script. It needs python support, and it's tested only in >7.1, but it should work in earlier versions as well. Drop me a line if it does and I'll update this description!

It will insert a closing pair when you type a quote (single and double), bracket, parenthesis, brace. It will also move over when you type the closing pair, and it will delete empty pairs when you hit backspace. This broadly mimics TextMate's behaviour for pairs of characters.

Its main difference from all the others is that it is it not aggressive at all! It will try to do so only when it makes sense, that is:

* at the end of the line
* when the next character is one of: <space>,.: 

That, simple as it looks, means that it will do its job when you're writing new code, but it will not mess up when you are editing code. 

It's heavily biased towards Python, so if anybody has other use cases please send me an email!

Options
--------------

`g:Simple_Pair_Enabled `
Defaults to 1. Change to 0 to turn off simple pairs, e.g. `let g:Simple_Pair_Enabled = 0`
