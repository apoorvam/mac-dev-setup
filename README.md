# Mac OSX Development Setup Guide [![Build Status](https://travis-ci.org/apoorvam/mac-dev-setup.svg?branch=master)](https://travis-ci.org/apoorvam/mac-dev-setup)

This guide is to cover the steps for installing commonly used tools for setting up development environment on a new Mac box. I have tried all of it on Mac Mountain Lion, Mojave and Mavericks.  I plan to add documentation on installation details at one place for common tools and also tips and tricks in usage of these tools which can be very effective during development.

### Contribution

Feel free to contribute by sending a pull request or create new issues on [GitHub](https://github.com/apoorvam/mac-dev-setup/issues). You can support by adding documentation for setting up any other widely used dev tools/libraries/languages.

#### Installation

This is a open source guide and is generated using GitBook. For steps on how to install GitBook, refer this [page](https://apoorvam.github.io/mac-dev-setup/gitbook/).

Like it? [Let me know](https://twitter.com/ItsApoorvaHere).

#### Build from source

* Install `node` and `npm`
* Run `npm install gitbook-cli -g`
* Run `gitbook build` to build project
* Serve the generated webpage. Optionally, you can install `go get github.com/apoorvam/serve` which downloads binary to `$GOPATH/bin` and run `cd _book & serve .`