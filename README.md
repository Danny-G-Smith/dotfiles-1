# My dotfiles

The majority of this repo is shamelessly stolen from Mathias Bynens famous [dotfiles repo](https://github.com/mathiasbynens/dotfiles). He has a ton of stuff going on in his dotfiles project that I didn't want, so I copied most of the setup files from there as a starting point for my configs.

## Installation

Clone the repository to `~/Projects/dotfiles` (with `~/dotfiles` as a symlink). The bootstrapper script will pull in the latest version and copy the files to the home folder.

```bash
git clone https://github.com/richardkalehoff/dotfiles.git && cd dotfiles && source bootstrap.sh
```

## To update

`cd` into the `dotfiles` repository and then:

```bash
source bootstrap.sh
```

Alternatively, to update while avoiding the confirmation prompt:

```bash
set -- -f; source bootstrap.sh
```

## Tmux

I use the fantastic [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm) with the following plugins:

* [tmux-sensible](https://github.com/tmux-plugins/tmux-sensible)
* [tmux-pain-control](https://github.com/tmux-plugins/tmux-pain-control)
* [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)
* [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum)

To install the plugins, run `prefix + I`.

To resurrect an environment, run `prefix + Ctrl-r`.
