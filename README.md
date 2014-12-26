# neocomplcache-ghc (neco-ghc)

A completion plugin for Haskell, using ghc-mod.

neco-ghc was originally implemented by @eagletmt on July 25, 2010, and then
ujihisa added some new features.

Updated to remove neocomplete/neocomplcache/ycm ~~bullshit~~ er, support,
and uses detailed browse as default on Dec 26, 2014

## Install

* Install ghc-mod package by `cabal install ghc-mod`
* Unarchive neco-ghc and put it into a dir of your &rtp.

## Usage

neco-ghc provides `necoghc#omnifunc` for omni-completion.
I recommend adding the following in your ~/.vim/after/ftplugin/haskell.vim.

```vim
setlocal omnifunc=necoghc#omnifunc
```

See `:help compl-omni` for details on omni-completion.

### Completion engines
This plugin can be used as a source of [VimCompletesMe](github.com/ajh17/VimCompletesMe)
You can enjoy auto-completions without any specific configuration.

## License

[BSD3 License](http://www.opensource.org/licenses/BSD-3-Clause), the same license as ghc-mod.
