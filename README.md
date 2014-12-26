# neco-ghc

A completion plugin for Haskell, using ghc-mod.

neco-ghc was originally implemented by @eagletmt on July 25, 2010, and then
ujihisa added some new features.

Note: Updated to remove neocomplete/neocomplcache/ycm ~~bullshit~~ er, support,
and uses detailed browse as default on Dec 26, 2014

## Install

* Install ghc-mod package by `cabal install ghc-mod`

AND

If you don't have a preferred installation method, I recommend installing
pathogen.vim, and then simply copy and paste:

`cd ~/.vim/bundle && git clone git://github.com/ajh17/neco-ghc.git`

## Usage
Simply set the following variables to `completefunc` or `omnifunc`:

```vim
setlocal omnifunc=necoghc#omnifunc
```
This plugin can also be used with [VimCompletesMe](https://github.com/ajh17/VimCompletesMe).
Simply set the `b:vcm_tab_complete` variable to "omni":

```vim
let b:vcm_tab_complete = "omni"
```

## License

[BSD3 License](http://www.opensource.org/licenses/BSD-3-Clause), the same license as ghc-mod.
