# Heroku Buildpack: mongo-tools

This is the [Heroku buildpack][buildpack] for mongo-tools.

Sometimes you need mongo-tools on a Heroku dyno, this puts them at your fingertips
in the bin folder

## Usage

Ensure your Heroku app is wired to use this buildpack:

    heroku buildpacks:set https://github.com/zph/heroku-buildpack-mongotools.git#v3.2.11

Mongo Tools are pulled down from deb package and unpacked for this distribution.

The ref at end of buildpack url is for the appropriate branch. Right now it is configured only for 3.2.11.
Pull requests welcome for other versions patterned off of branch: v3.2.11.

## Credits

The source code found here has been remixed from Paxan's [GB buildpack.][gb go buildpack]

That buildpack was remixed from the original [Go buildpack.][hbgo]

The simplicity of the build step in `bin/compile` script can be blamed
entirely on [gb][gbrepo] by [@davecheney](https://github.com/davecheney).

[buildpack]: http://devcenter.heroku.com/articles/buildpacks
