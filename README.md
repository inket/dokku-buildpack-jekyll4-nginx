Heroku buildpack: Jekyll + Nginx
================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for Jekyll sites.  In contrast to 
[Mark Pundsack's Jekyll buildpack](https://github.com/markpundsack/heroku-buildpack-jekyll), this buildpack
embeds a copy of [nginx](http://nginx.org) in your app slug.  This approach has several benefits:

* nginx is a smaller, more lightweight web server
* No need to start the Ruby interpreter, so your app boots faster
* nginx is evented, so can handle multiple HTTP requests at a time

Credit where credit's due
=========================

Honestly my contribution to this buildpack consisted mainly of judicious use of copy and paste.
This is basically a mashup of [heroku-buildpack-nginx](https://github.com/essh/heroku-buildpack-nginx) and
[heroku-buildpack-jekyll](https://github.com/nbudin/heroku-buildpack-jekyll-nginx).  Thanks very much to Stephen
Haynes and Mark Pundsack for those buildpacks.  Thanks also to Marc Chung, who wrote another nginx buildpack I
also used while developing this one.
