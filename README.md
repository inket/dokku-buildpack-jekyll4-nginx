This is a dokku buildpack for installing Jekyll 3. It uses `Ruby 2.2.1` and `nginx 1.5.7`

Tested with:
- `dokku 0.10.5` and `jekyll-3.6.2` on Ubuntu 14.04.

### Usage

Just add a `.buildpacks` file in the root of your Jekyll project containing:

```
https://github.com/ryandotsmith/nginx-buildpack.git
https://github.com/inket/dokku-buildpack-jekyll3-nginx.git
```

(Delete any previous `.env` file that contain `export BUILDPACK_URL=...`)

### Other

For Jekyll 2.x, use [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

### Credit

Fork tree:

- [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

	- [shsteven/dokku-buildpack-jekyll-nginx](https://github.com/shsteven/dokku-buildpack-jekyll-nginx)

		- [nbudin/heroku-buildpack-jekyll-nginx](https://github.com/nbudin/heroku-buildpack-jekyll-nginx)

			- [mchung/heroku-buildpack-nginx](https://github.com/mchung/heroku-buildpack-nginx)
