Heroku buildpack: Python (wheelhouse)
=====================================

This is a supplementary
[Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks), which
installs any private Python wheels from a `wheelhouse` directory included in
the app.

The standard buildpack configuration looks like this:

    heroku buildpacks:set https://github.com/heroku/heroku-buildpack-python -a app-name
    heroku buildpacks:add https://github.com/orchardmile/heroku-buildpack-wheelhouse -a app-name

It is intended to be
[added](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app)
after [the regular Python buildpack](https://github.com/heroku/heroku-buildpack-python),
as it uses the installed python interpreter to install the wheel files.
