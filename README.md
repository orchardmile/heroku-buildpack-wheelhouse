Heroku buildpack: Python/wheelhouse
===================================

This is a supplementary
[Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks), which
installs any private Python wheels from an included `wheelhouse` directory.

It is intended to be
[added after the regular Python buildpack](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app),
as it uses the installed python interpreter to install the wheel files.
