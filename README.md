This is a dokku buildpack for installing Jekyll 4. It uses `Ruby 2.7.2` and `nginx 1.9.5`

Tested with:

- `dokku 0.13.4` and `jekyll-4.2.0` on Ubuntu 16.04.

### Usage

Just add a `.buildpacks` file in the root of your Jekyll project containing:

```
https://github.com/heroku/heroku-buildpack-nginx.git
https://github.com/inket/dokku-buildpack-jekyll4-nginx.git
```

(Delete any previous `.env` file that contain `export BUILDPACK_URL=...`)

### Other

For Jekyll 3.x use

```
https://github.com/heroku/heroku-buildpack-nginx.git
https://github.com/inket/dokku-buildpack-jekyll4-nginx.git#b99e300b0315a2bfa39faeaeefc580f9c1f65535
```

For Jekyll 2.x, use [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

### Credit

Fork tree:

- [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

	- [shsteven/dokku-buildpack-jekyll-nginx](https://github.com/shsteven/dokku-buildpack-jekyll-nginx)

		- [nbudin/heroku-buildpack-jekyll-nginx](https://github.com/nbudin/heroku-buildpack-jekyll-nginx)

			- [mchung/heroku-buildpack-nginx](https://github.com/mchung/heroku-buildpack-nginx)
