# VIM - Jasmine

This is a syntax highlighting plugin for the [Jasmine](http://) JavaScript testing framework. I extracted most of this from [thomd's VIM-Jasmine plugin](https://github.com/thomd/vim-jasmine) which is wonderful, but overkill for what I was looking for. I made a few modifications to suit my preferences.

## Installation

### With [Vundle](https://github.com/gmarik/vundle)

Add:

```
Bundle 'glanotte/vim-jasmine'
```

To your `.vimrc` and run `BundleInstall` from within vim or `vim +BundleInstall +qall` from the command line

### With [Pathogen](https://github.com/tpope/vim-pathogen)

```
cd ~/.vim/bundle
git clone https://github.com/glanotte/vim-jasmine.git
```

## Usage

By default this syntax is used with all `*_spec.js` and `*Spec.js` files. If you don't follow this norm use something like:

```
autocmd BufReadPost,BufNewFile *_foo.js set filetype=jasmine.javascript syntax=jasmine
```

In your `~/.vimrc`

## Dependencies

This assumes that you are using some other javascript plugin for syntax highlighting and it attaches itself onto the JavaScriptAll cluster.
