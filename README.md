# neocomplcache-ghc (neco-ghc)

A completion plugin for Haskell, using ghc-mod.

## What is neco-ghc

This plugin supports the following completion.

* pragma
    ![](http://cache.gyazo.com/c922e323be7dbed9aa70b2bac62be45e.png)
* language
    ![](http://cache.gyazo.com/9df4aa3cf06fc07495d6dd67a4d07cc4.png)
* importing a module
    ![](http://cache.gyazo.com/17a8bf08f3a6d5e123346f5f1c74c5f9.png)
* importing a function of a module
    ![](http://cache.gyazo.com/d3698892a40ffb8e4bef970a02198715.png)
* function based on importing modules
    ![](http://cache.gyazo.com/bc168a8aad5f38c6a83b8aa1b0fb14f6.png)

neco-ghc was originally implemented by @eagletmt on July 25, 2010, and then
ujihisa added some new features.

Updated to remove neocomplete/neocomplcache/ycm ~~bullshit~~er, support,
and uses detailed browse as default.

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
