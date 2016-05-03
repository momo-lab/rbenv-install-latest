# rbenv-install-latest

This [rbenv](https://rbenv.org) plugin to install the latest version of Ruby using [ruby-build](https://github.com/rbenv/ruby-build).

## Usage

     rbenv install-latest [<`rbenv install` options>] [<version-prefix>]

## Installation
This plugin uses [ruby-build](https://github.com/rbenv/ruby-build), so first clone are for them:

    mkdir -p "$(rbenv root)"/plugins
    git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
    git clone https://github.com/momo-lab/rbenv-install-latest.git "$(rbenv root)"/plugins/rbenv-install-latest

## Usage example

Install latest version of Ruby.

    $ rbenv install-latest
    Downloading ruby-2.3.1.tar.bz2...
    -> https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.1.tar.bz2
    Installing ruby-2.3.1...
    Installed ruby-2.3.1 to /home/ubuntu/.rbenv/versions/2.3.1

Install 2.0-based version of Ruby.

    $ rbenv install-latest 2.0
    Downloading ruby-2.0.0-p648.tar.bz2...
    -> https://cache.ruby-lang.org/pub/ruby/2.0/ruby-2.0.0-p648.tar.bz2
    Installing ruby-2.0.0-p648...
    
    WARNING: ruby-2.0.0-p648 is past its end of life and is now unsupported.
    It no longer receives bug fixes or critical security updates.
    
    Installed ruby-2.0.0-p648 to /home/ubuntu/.rbenv/versions/2.0.0-p648

