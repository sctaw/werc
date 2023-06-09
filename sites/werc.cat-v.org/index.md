werc - A sane web anti-framework
================================

Werc is a minimalist web anti-framework built following the [Unix](http://doc.cat-v.org/unix/) and [Plan 9](http://plan9.cat-v.org)
*tool philosophy* of software design.

Werc avoids the pain of managing collections of websites and developing web
applications.

* Database free, uses files and directories instead.
* Written using [the rc shell](http://rc.cat-v.org), leveraging the standard Unix/Plan 9 command toolkit.
* Minimize tedious work: eg., no need to ever write HTML, use markdown (or any other format) instead.
* Very minimalist yet extensible codebase: highly functional core is 150 lines, with extra functionality in modular [apps](/apps/).


Features
--------

Here are some of the features provided by werc:

* Good integration with pre-existing content, you can add HTML or plain text files and they will be seamlessly integrated with the rest of the site.
* You can use your favorite tools (text editor, shell, file manager, etc) to edit, manipulate and manage data stored in werc.
* Designed to manage any number of 'virtual' domains that share a common style and layout from a single werc installation.
* Configuration and customization can be at at any level: global, per-domain-group, domain-wide, directory sub-tree, and single file.
* Can trivially run multiple (customized) versions of werc side by side.
* Very simple and flexible user management and permissions system.
* Applications can be easily combined: eg., add comments to your blog or wiki by enabling the 'bridge' app; or by enabling the 'diridir' wiki convert any document tree into a wiki.
* Can easily write werc 'apps' and extensions in *any* language! (But of course, rc is recommended).


Install Requirements
--------------------

All you need is some Plan 9 commands (cat, grep, sed, rc, etc.), and an HTTP
server with CGI support.

Werc runs on any Unix-like system where [Plan 9 from User Space](https://9fans.github.io/plan9port/),
[9base](https://tools.suckless.org/9base/),
or [frontport](https://code.9front.org/hg/frontbase)
are available (this includes Linux, \*BSD, OS X and Solaris), and on Plan 9.

Werc can use any HTTP server that can handle CGI, and has been tested with at
least Apache, Lighttpd, Cherokee, nhttpd, Hiawatha, rc-httpd, cgd, and others.

Werc uses markdown by default (and the standard Perl markdown is included with
the distribution), to format documents, but any other formatting system can be
used.


Source
------

To get a copy of the latest development code using mercurial, do:

	hg clone https://code.9front.org/hg/werc/

You can also [browse the online repository](https://code.9front.org/hg/werc/).


Contact
-------

For questions, suggestions, bug reports and contributing patches you can join
the werc mailing list. To join, send a message with a body consisting only of the word _subscribe_ to werc-owner@cat-v.org. After you get the confirmation notice, you can post by sending messages to werc@cat-v.org.

To track commit messages, you can join the werc-commits mailing list. To join, send a message with a body consisting only of the word _subscribe_ to werc-commits-owner@cat-v.org.

On irc, join [#cat-v](irc://irc.oftc.org/cat-v) on irc.oftc.org


License
-------

Public domain, [because so called 'intellectual property' is an
oxymoron](http://harmful.cat-v.org/economics/intellectual_property/).

Alternatively if your prefer it or your country's brain dead copyright law
doesn't recognize the public domain werc is made available under the terms of
the MIT and ISC licenses.


Credits
-------

Thanks to [Uriel](http://uriel.cat-v.org/) for creating werc.

Thanks to Kris Maglione (aka JG) for implementing rss feeds, for writing the
awk rc-templating system, and other help and inspiration (some parts of the
code were based on JG's diri wiki).

Thanks to Mechiel (aka oksel) for the md_cache script.

Thanks Garbeam (aka arg) for writing the original diri code and showing that
writing complex web apps in rc was feasible.

Thanks to Ethan Gardner for writing rc-httpd.

And thanks to everyone else whom we may have forgotten and that has provided fixes
and feedback.
