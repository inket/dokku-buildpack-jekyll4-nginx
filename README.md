Heroku buildpack: Jekyll + Nginx
================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for Jekyll sites.  In contrast to 
[Mark Pundsack's Jekyll buildpack](https://github.com/markpundsack/heroku-buildpack-jekyll), this buildpack
embeds a copy of [nginx](http://nginx.org) in your app slug.  This approach has several benefits:

* nginx is a smaller, more lightweight web server
* No need to start the Ruby interpreter, so your app boots faster
* nginx is evented, so can handle multiple HTTP requests at a time

