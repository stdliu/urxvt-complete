# URxvt Completion

A completion extension for URxvt.

## INSTALL

Download (git clone) the [urxvt-complete](https://github.com/stdliu/urxvt-complete/blob/master/urxvt-complete) into your floder.
Then add the following code to your .Xdefaults/.Xresources :

	URxvt.perl-lib: /your/folder/
	URxvt.perl-ext-common: urxvt-complete
	URxvt.keysym.M-Tab: perl:urxvt-complete:activate
	! M-/
	URxvt.keysym.M-0x2f: perl:urxvt-complete:activate

## USAGE

Use Alt-Tab or Alt-/ to activate completion mode, then use the following keys:

	Ctrl-n/Alt-n/Down : next.
	Ctrl-p/Alt-p/Up : previous.
	Ctrl-f/Ctrl-v/PageDown : next page.
	Ctrl-b/Alt-v/PageUp: previous page.
	Tab : forward common prefix, or next.
	Enter/Space : commit.
	Escape: deactivate complete mode.

## SNAPSHOT

![URL complete](https://raw.github.com/stdliu/urxvt-complete/master/images/url_complete.png "URL complete")

![nano complete](https://raw.github.com/stdliu/urxvt-complete/master/images/nano_complete.png "nano complete")

## TODO

- Add Left, Right key for long string.
- Add cursor move support.
- Display match string in appear order instead of dictionary order.
