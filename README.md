BBCode Mode
===========

This major mode lets you write [phpBB][phpbb] forum posts in
[Emacs][emacs]. It implements syntax highlighting and keyboard
commands for [BBCode][bbc] (Bulletin Board Code), the markup language
used by phpBB.

Do `M-x bbcode-scratch` to instantly get a temp buffer to write
posts. Use `M-x bbcode-mode` to switch an existing buffer to BBCode
mode. The file name extension `.bbcode` is also recognized.

Other BBCode Modes
------------------

The [BBCode article on EmacsWiki][ew-bbcode] lists two other BBCode
modes:

* [xbbcode-mode.el][xbbcode-mode] by Xah Lee. He requires a payment of
  $3 via PayPal to download it.
* [bcode-mode.el][bcode-mode] by Jason McBrayer. Beginnings of a mode
  like this one from 2008.


How To Install
--------------

We recommend installing from [MELPA][melpa].

Otherwise, to install manually, all you need to do is place
`bbcode-mode.el` in your `load-path`, then add `(require
'bbcode-mode)` to your Emacs init file and restart Emacs.


How To Report Bugs
------------------

GitHub issues are preferred. Email is also ok.

Please include the package version number. It can be found in `M-x
list-packages` output or at the top of `bbcode-mode.el`. If you have
cloned the official Git repository, please state the commit hash of
the version you are using.


Supported Tags
--------------

Below is a list of all the tags BBCode Mode supports.  It also lists
the key-bindings to insert those tags.  If you have a selected region
then BBCode Mode will wrap the tag around the region.

Each key-binding has three parts.  They all begin with `C-c`.  The
second part indicates the ‘group’ to which the binding belongs.  And
the third part is a single letter named after the actual tag.  Each
section below provides a mnemonic to help remember the second part.

### Common Tags ###

Key-bindings for common tags begin with `C-c C-t`.

Mnemonic: <strong>T</strong>ag

* `[b]`: `C-c C-t b`
* `[center]`: `C-c C-t n`
* `[code]`: `C-c C-t c`
* `[del]`: `C-c C-t d`
* `[email]`: `C-c C-t e`
* `[i]`: `C-c C-t i`
* `[img]`: `C-c C-t m`
* `[quote]`: `C-c C-t q`
* `[s]`: `C-c C-t s`
* `[u]`: `C-c C-t u`
* `[url]`: `C-c C-t l`

### Font Tags ###

Key-bindings related to font tags begin with `C-c C-f`.

Mnemonic: <strong>F</strong>ont

* `[color]`: `C-c C-f c`
* `[font]`: `C-c C-f f`
* `[size]`: `C-c C-f s`
* `[style]`: `C-C C-f y`

### List Tags ###

Key-bindings for list tags begin with `C-c C-l`.

Mnemonic: <strong>L</strong>ist

* `[li]`: `C-c C-l i`
* `[list]`: `C-c C-l l`
* `[ol]`: `C-c C-l o`
* `[ul]`: `C-c C-l u`
* `[*]`: `C-c C-l *`

### Table Tags ###

Mnemonic: Ta<strong>b</strong>le

Key-bindings for table tags begin with `C-c C-b`.

* `[table]`: `C-c C-b t`
* `[td]`: `C-c C-b d`
* `[th]`: `C-c C-b h`
* `[tr]`: `C-c C-b r`

### Special Tags ###

These are tags which are uncommon in BBCode and may even be unique to
specific websites.  These key-bindings all begin with `C-c C-s`.

Mnemonic: <strong>S</strong>pecial

* `[attachment]`: `C-c C-s a`
* `[gvideo]`: `C-c C-s g`
* `[manual]`: `C-c C-s m`
* `[wiki]`: `C-c C-s w`
* `[youtube]`: `C-c C-s y`


Contributors
------------

* [Eric James Michael Ritz](https://github.com/ejmr/) &mdash; author
* [Sebastian Wiesner](https://github.com/lunaryorn)
* [L.C. Karssen](https://github.com/lckarssen)
* [Lassi Kortela](https://github.com/lassik)


License
-------

[GNU General Public License][gpl] version 3 or later



[phpbb]: https://www.phpbb.com/
[bbc]: http://bbcode.org/
[bcode-mode]: https://bitbucket.org/jfm/emacs-bbcode/
[emacs]: http://www.gnu.org/software/emacs/
[ew-bbcode]: http://www.emacswiki.org/emacs/BbCode
[gpl]: http://www.gnu.org/copyleft/gpl.html
[melpa]: https://melpa.org/#/?q=bbcode-mode
[xbbcode-mode]: http://xahlee.org/emacs/xbbcode-mode.html
