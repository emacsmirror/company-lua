# company-lua #

Company-lua is a [company-mode](http://company-mode.github.io/)
completion backend for `Lua`.

## Installation ##

### Manual ###

Add `company-lua` to the `load-path`:

```lisp
(add-to-list 'load-path "path/to/company-lua")
```

Add the following to your `init.el`:

```lisp
(require 'company)
(require 'company-lua)
(add-to-list 'company-backends 'company-lua)
```

or if you only want to use `company-lua` as backend:

```lisp
(add-hook 'lua-mode-hook
          (lambda () (setq-local company-backends '(company-lua))))
```
