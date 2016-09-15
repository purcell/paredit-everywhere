paredit-everywhere.el
=====================

It turns out that a lot of the `paredit` key bindings work as
expected in non-lisp buffers, since many major modes provide
reasonable sexp-oriented navigation.

This library, then, provides a minor mode which enables a subset
of the `paredit` library's editing commands in non-lisp buffers.

A grander project offering similar functionality is Matus Goljer's
[smartparens package](https://github.com/Fuco1/smartparens).

Installation
=============

If you choose not to use one of the convenient packages in
[MELPA][melpa], you'll need to add the
directory containing `paredit-everywhere.el` to your `load-path`, and then
`(require 'paredit-everywhere)`.

Usage
=====

Enable the minor mode in non-lisp buffers by adding `paredit-everywhere-mode` to
your mode hooks. In Emacs 24 and greater, `prog-mode-hook` is a great choice:

```lisp
(add-hook 'prog-mode-hook 'paredit-everywhere-mode)
```

Use <kbd>C-h m</kbd> to see which paredit commands are available.

[melpa]: http://melpa.org

<hr>

[![](http://api.coderwall.com/purcell/endorsecount.png)](http://coderwall.com/purcell)

[![](http://www.linkedin.com/img/webpromo/btn_liprofile_blue_80x15.png)](http://uk.linkedin.com/in/stevepurcell)

[Steve Purcell's blog](http://www.sanityinc.com/) // [@sanityinc on Twitter](https://twitter.com/sanityinc)

