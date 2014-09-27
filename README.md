# WKHTMLTOPDF Buildpack

This is a [Heroku buildpack][0] for bundling a compatible [wkhtmltopdf][1] and [wkhtmltoimage][1] binary with your environment.

## Versions

* Buildpack:   0.2
* WKHTMLTOPDF: 0.12.1
* WKHTMLTOIMAGE: 0.12.1

## Usage

```bash
$ heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git
$ echo 'https://github.com/versacommerce/wkhtmltox-buildpack.git' >> .buildpacks
$ echo 'https://codon-buildpacks.s3.amazonaws.com/buildpacks/heroku/ruby.tgz' >> .buildpacks
$ git add .buildpacks
$ git commit -m 'Add multi-buildpack'
```

Please note that this buildpack is only compatible with the cedar-14
stack. You can use `heroku stack:set cedar-14` to set the correct stack.

[0]: http://devcenter.heroku.com/articles/buildpacks
[1]: http://wkhtmltopdf.org
