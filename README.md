This is a dokku buildpack for installing Jekyll 3 with Nginx.

Tested with `dokku v0.4.2-45-ge471214` and `jekyll-3.0.0`

### Usage

Just add a `.env` file in the root of your jekyll project containing:

```
export BUILDPACK_URL=https://github.com/inket/dokku-buildpack-jekyll3-nginx.git
```

### Other

For Jekyll 2.x, use [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

### Credit

Fork tree:

- [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

	- [shsteven/dokku-buildpack-jekyll-nginx](https://github.com/shsteven/dokku-buildpack-jekyll-nginx)

		- [nbudin/heroku-buildpack-jekyll-nginx](https://github.com/nbudin/heroku-buildpack-jekyll-nginx)

			- [mchung/heroku-buildpack-nginx](https://github.com/mchung/heroku-buildpack-nginx)