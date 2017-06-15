# Welcome to worker! [![Build Status](https://travis-ci.org/thibmaek/worker.svg?branch=master)](https://travis-ci.org/thibmaek/worker)
> Getting your macOS machine up and running!

Worker is a personal project to quickly get new or clean installed macOS machines
up and running with everything I need for my development workflow.

It currently presets all of the following:
* [macOS sensible defaults](https://github.com/mathiasbynens/dotfiles/blob/master/.macos)
* [Brew](https://github.com/Homebrew/homebrew) (with casks)
* Node (trough [nvm](https://github.com/creationix/nvm)) (with global packages trough npm)
* Ruby (trough [rbenv](https://github.com/rbenv/rbenv))
* Python (trough [pyenv](https://github.com/yyuu/pyenv))
* [Atom](https://github.com/atom/atom) (with apm packages & themes)

This is great for setting up the tools you need. If you need to tweak the shell you might want to look into [my dotfiles](https://github.com/thibmaek/dotfiles).

### Installing
Just running it from the top is easy:

```shell
git clone https://github.com/thibmaek/worker.git .worker && cd .worker
./make.sh
```

`make` is the file that points your shell to each specific module.
If you want to turn certain modules of, just comment them out from `make`

If you want to you can also install this on a file-per-file base, just run the .sh files inside of the modules directory. The extensions directory installs additional content to the modules.

### Modifying
No problem forking this over to your own account, but don't bother sending a PR because I won't merge it unless it's a bug fix (though I prefer to use the issues on this repo for that.)

#### Testing
There is a `test.local` script for locally running the tests.
Tests are just shell scripts so you can add your own in.

Run the local tests with `./test.local`
