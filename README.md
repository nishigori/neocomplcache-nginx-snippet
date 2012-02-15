# neocomplcache-nginx-configuration

A neocomplcache snippet complate for the [Nginx](http://wiki.nginx.org/Main).

## install

* install the neocomplcache.vim
* install the neocomplcache-snippets-complete.vim

## How to use

When you configure Nginx's file (nginx.conf, proxy.conf, fastcgi.conf ..),
Specified vim's filetype nginx.

If for some reason this plugin is not being added to neocomplcache-snippets-complete,
check that the filetype in vim contains.

For exam, Please add in your .vimrc:

`augroup FiletypeDetect`
` au! BufRead,BufNewFile /etc/nginx/*,/usr/local/nginx/*,*/nginx/vhosts.d/*,nginx.conf if &ft == '' | setfiletype nginx | endif`
`augroup END`

or {your vim's runtimepath}/ftdetect/nginx.vim:

`au BufRead,BufNewFile /etc/nginx/*,/usr/local/nginx/*,*/nginx/vhosts.d/*,nginx.conf if &ft == '' | setfiletype nginx | endif`

## FUTURE

Not just the snippet, complete the nginx configuration's keyword. Maybe Yes :p

## Info

* [Nginx](http://wiki.nginx.org/Main)
* [neocomplcache (vim.org)](http://www.vim.org/scripts/script.php?script_id=2620)
* [neocomplcache (github)](https://github.com/Shougo/neocomplcache)
* [neocomplcache-snippets-complete (github)](https://github.com/Shougo/neocomplcache-snippets-complete)
* [vim doc: ftdetect](http://vimdoc.sourceforge.net/htmldoc/filetype.html#ftdetect)
* another Vim plugin for nginx
* [nginx.vim (syntax)](http://www.vim.org/scripts/script.php?script_id=1886)
* [@evanmiller forked nginx.vim (syntax, indent)](https://github.com/evanmiller/nginx-vim-syntax)
* [@chase forked nginx.vim (syntax, indent, ftdetect)](https://github.com/chase/nginx.vim)
