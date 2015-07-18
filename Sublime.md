# Sublime Text

Sublime text is my favorite text editor.  It's already awesome but customization makes it extremely powerful. 

## Packages

First, [Package Control](https://packagecontrol.io/) makes installing things extremely easy.  
See installation instruction on [the website](https://packagecontrol.io/) to install it. 

Now you should be all set to install useful packages by hitting `cmd + Shift + P`
and choose `Package Control: Install Package`.

### Theme

[SpaceGray](http://kkga.github.io/spacegray/) makes the side bar much nicer than the default theme. 

![SpaceGray](http://kkga.github.io/spacegray/assets/spacegray.png)

### Misc (Language Independent)

- *AdvancedNewFile* — create new file anywhere with `cmd+opt+n`
- *Alignment*
- *AllAutoComplete* – extend sublime autocomplete to check all opened files.
- *EasyMotion* - super fast navigation with `cmd+;+<*character-to-jump-to*>` a super plugin inspired from a famous Vim plugin.
- *Sidebar Enhancement* – many cool add-ons to the sidebar

### Misc (Work for many languages)

- *Sublimelinter* is great for checking syntax errors and warning for most languages.
You will need to install its subpackage e.g.,  **TODO**

- *DocBlockr* is great for creating comments for Javascript/C.

### Git 
- *[GitGutter](http://www.jisaacks.com/gitgutter)* – view changes in git instantly in your editor

### HTML Editing

- *Emmet* — quick html/csscoding

### Markdown
- *[MarkdownEditing](https://packagecontrol.io/packages/MarkdownEditing)* - provide a number of commands for editing markdown.  For instance:
  - `cmd+r` will show all markdown headers in the symbol list.
  - `cmd+alt+k` - insert a link.  Even better `cmd+alt+v` will insert a link from your clipboard. 
- *[MarkdownExtended](https://packagecontrol.io/packages/Markdown%20Extended)* - extend to support yaml header and etc. 

## Keyboard Shortcuts

- `alt+enter` in the find screen will select all of the occurence (in the multiple selection mode)

**TODO**

## Trick

- To select all text inside quotes, use `([""'])(?:(?=(\\?))\2.)*?\1` as your find RegEx.  (I put this as `quote#` in [Dash](Dash.md)

## Accessing Sublime from command line

From https://www.sublimetext.com/docs/3/osx_command_line.html, add symlink to the `subl` binary in your preferred bin directory.  The example here assumes you have `~/bin/` created. 

```
ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" ~/bin/subl
```

If you don't have `~/bin/` created and prefer to use it, run `mkdir ~/bin` to create one.
Then add the following line to your shell profile file (`~/.zprofile` for zsh, `~/bash_profile` for bash).

```zsh
export PATH=/usr/local/git/bin:$PATH
```
