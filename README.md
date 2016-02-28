# Buildpack for Python NLTK

This build pack will build upon Heroku's default python buildpack.
Therefore this should be deployed in a
[multi-buildpack arrangement](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app).

## Configuration

Create a file named `nltk` within your root directory. This should
contain a list of packages you wish to be downloaded. For example:

```
punkt
brown
```

Note that you can easily take your project over Heroku's maximum
slug size using this method.

Tested with [flynn](http://flynn.io).
