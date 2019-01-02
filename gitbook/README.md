# Gitbook

[Gitbook](https://www.gitbook.com) is an easy to use solution to write, publish and host books. It is the easiest solution for publishing your content and collaborating on it.

## Installation

The best way to install GitBook is via NPM(If not already installed, refer [this](../npm/README.md) page). At the terminal prompt, simply run the following command to install GitBook:

```
$ npm install gitbook-cli -g
```

## Usage

### Create a book

GitBook can setup a boilerplate book:
```
$ gitbook init
```

If you wish to create the book into a new directory, you can do so by running gitbook init ./directory

### Build and serve book

Preview and serve your book using:
```
$ gitbook serve
```
Or build the static website using:
```
$ gitbook build
```