# WKHTMLTOPDF Buildpack

This is a [Heroku buildpack][0] for bundling a compatible [wkhtmltopdf][1] and [wkhtmltoimage][1] binary with your environment.

## Versions

* Buildpack:   0.2
* WKHTMLTOPDF: 0.12.2.1
* WKHTMLTOIMAGE: 0.12.2.1

## Usage
Add the following line to your ```.buildpacks``` file
```ruby
'https://github.com/homelight/wkhtmltox-buildpack.git'
```

Please note that this buildpack is only compatible with the cedar-14
stack. You can use `heroku stack:set cedar-14` to set the correct stack.

[0]: http://devcenter.heroku.com/articles/buildpacks
[1]: http://wkhtmltopdf.org
