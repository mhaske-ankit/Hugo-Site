+++
title = "Hello World"
date = "2023-08-01T11:44:19+05:30"
author = ""
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
color = "" #color from the theme settings
+++
### Nodes
- First item
- Second item
- Third item
- Fourth item
  ## How to start

You can download the theme manually by going to [https://github.com/panr/hugo-theme-terminal.git](https://github.com/panr/hugo-theme-terminal.git) and pasting it to `themes/terminal` in your root directory.

You can also choose **one of the 3 possibilities** to install the theme:

1. as Hugo Module
2. as a standalone local directory
3. as a git submodule

⚠️ The theme needs at least Hugo **Extended** v0.90.x.

### Install theme as Hugo Module

```bash
# If this is the first time you're using Hugo Modules
# in your project. You have to initiate your own module before
# you fetch the theme module.
#
# hugo mod init [your website/module name]
hugo mod get github.com/panr/hugo-theme-terminal/v3
```

and in your config file add:

```toml
[module]
  # this is needed when you fetch the theme as a submodule to your repo.
  # replacements = "github.com/panr/hugo-theme-terminal -> themes/terminal"
[[module.imports]]
  path = 'github.com/panr/hugo-theme-terminal/v3'
```

Keep in mind that the theme by default won't show up in the `themes` directory. This means that you are using the theme as it was on the repository at the moment you fetched it. Your local `go.sum` file keeps all the references. Read more about Hugo Modules in the [official documentation](https://gohugo.io/hugo-modules/).

### Install theme locally

```bash
git clone https://github.com/panr/hugo-theme-terminal.git themes/terminal
```

This will clone the repository directly to the `themes/terminal` directory.

### Install theme as a submodule

```bash
git submodule add -f https://github.com/panr/hugo-theme-terminal.git themes/terminal
```

This will install the repository as a sumbodule in the `themes/terminal` directory.

⚠️ If you encounter any issues with:

```bash
Error: module "terminal" not found; either add it as a Hugo Module or store it in "[...your custom path]/themes".: module does not exist
```

then please try to remove `theme = "terminal"` from your config file.

## How to run your site

```bash
hugo server -t terminal
```

and go to `localhost:1313` in your browser. From now on all the changes you make will go live, so you don't need to refresh your browser every single time.
