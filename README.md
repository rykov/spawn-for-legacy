# Spawn for Legacy

Kernel.spawn in ruby 1.9 solves all issues on asynchronous executions.[1](http://ujihisa.blogspot.com/2010/03/how-to-run-external-command.html)[2](http://ujihisa.blogspot.com/2010/03/all-about-spawn.html)
But ruby 1.8, the legacy version of MRI, is still used on many environments.

This library provides `spawn()` which is almost perfectly compatible with ruby 1.9's.

## Install

    gem install sfl

## How to use

    require 'rubygems'
    require 'sfl'
    
    spawn 'ls'

If your ruby is 1.9, `require 'sfl'` doesn't do anything. If your ruby is 1.8, that defines `spawn`.

## How compatible the spawn is?

(I'll put the coverage here later)

## Misc.

* At first I tried to use the name `spawn` as this gem library name, but the name was already used. The `spawn` gem library does not mean ruby 1.9's `spawn` at all.
* Ruby 1.9's `open3` library, based on `spawn`, is very useful. I would like to port `open3` to ruby 1.8 in my future.
