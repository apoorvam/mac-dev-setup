# Ruby

Mac comes preinstalled with Ruby, but it can get difficult to manage multiple versions of it depending on project. So it is better to use tools like `rbenv` or `rvm` to manage and install multiple versions of it, locally or globally. 

## Installation

Install ruby via homebrew as:

```
$ brew install ruby
$ echo 'eval "$(rbenv init -)"' >> ~/.zshrc # To use above installed ruby, rather than system pre-installed
$ source ~/.zshrc
$ brew install rbenv
```

You can install particular version of Ruby as `rbenv install 2.3.4`. To set a existing ruby version to repository locally, you can run `rbenv local 2.3.4`

## Bundler

Bundler is used to install particular version of gems that is required for your project.

```
$ gem install bundler
```

Now you can run `bundle install` to install all the dependencies from your project root directory.