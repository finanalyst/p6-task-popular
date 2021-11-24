# Task::Popular
[Introduction](#introduction)    
[Module Listing](#modules-in-this-distribution)  
[Date of Compilation](#date-of-compilation)  
[Problems](#problems)  
[Updates and Algorithm](#updates-and-algorithm)

## Introduction

The developers of Perl6 decided that the implementation
of the language (eg. Rakudo) would be available with a bare minimum of "core" modules.
Some modules are essential, such as Test, or the module manager (previously `panda`, currently `zef`).

The intention is for users / user groups to contribute distributions that meet a specific topic area.
Rakudo itself is available in a package called `Rakudo Star` with a minimal number of modules.

This distribution list takes another, data driven, approach.

Modules are intended to provide common functionality, and so are `use`d or **cited** by other modules in the Ecosystem. A set of modules that are
frequently used can be fairly safely assumed will be regularly maintained. Failures in these modules will affect many other modules, and there will be pressure to get them fixed. 

This list uses [Citation Indices](http://finanalyst.github.io/ModuleCitation/) to identify the 30 modules most recursively popular modules in the Ecosystem.

## Modules in this distribution

| Module Name | Recursive Citation Index | Module Description |
|---| :---: | :--- |
| JSON::Fast | 42.37 | OOps description not found, please file issue at github repository of p6-task-popular |
| MIME::Base64 | 31.45 | Encoding and decoding Base64 ASCII strings |
| File::Directory::Tree | 30.89 | Port of File::Path::Tiny - create and delete directory trees |
| URI | 28.44 | A URI implementation using Raku grammars to implement RFC 3986 BNF |
| OpenSSL | 24.11 | OpenSSL bindings |
| File::Temp | 23.35 | OOps description not found, please file issue at github repository of p6-task-popular |
| File::Find | 19.02 | File::Find for Raku |
| File::Which | 18.27 | Cross platform Perl 6 executable path finder (aka which on UNIX) |
| HTTP::Status | 16.76 | Get the text message associated with an HTTP status code |
| DateTime::Parse | 16.57 | DateTime parser |
| Terminal::ANSIColor | 16.57 | Colorize terminal output |
| JSON::OptIn | 16.38 | OOps description not found, please file issue at github repository of p6-task-popular |
| JSON::Name | 16.2 | OOps description not found, please file issue at github repository of p6-task-popular |
| JSON::Unmarshal | 15.63 | Turn JSON into objects |
| JSON::Marshal | 15.44 | OOps description not found, please file issue at github repository of p6-task-popular |
| JSON::Tiny | 15.25 | OOps description not found, please file issue at github repository of p6-task-popular |
| JSON::Class | 15.07 | OOps description not found, please file issue at github repository of p6-task-popular |
| Shell::Command | 14.12 | Common shell command replacements |
| IO::Socket::SSL | 13.94 | IO::Socket::SSL for Perl 6 using OpenSSL |
| META6 | 12.62 | OOps description not found, please file issue at github repository of p6-task-popular |
| Digest | 12.43 | Pure perl6 implementation of digest algorigthms. |
| Encode | 12.24 | Character encodings in Perl 6 |
| LibraryMake | 12.24 | An attempt to simplify native compilation |
| HTTP::UserAgent | 11.86 | Web user agent |
| License::SPDX | 11.68 | OOps description not found, please file issue at github repository of p6-task-popular |
| Test::META | 11.49 | OOps description not found, please file issue at github repository of p6-task-popular |
| YAMLish | 10.92 | a YAML parser/emitter written in pure raku |
| OO::Monitors | 10.73 | OOps description not found, please file issue at github repository of p6-task-popular |
| Digest::HMAC | 10.55 | Generic HMAC implementation |
| Hash::Merge | 9.6 | OOps description not found, please file issue at github repository of p6-task-popular |
## Date of Compilation

This list was compiled on 2021-11-24.

## Problems

Inevitably for commonly needed functionality, there may be multiple modules that provide the same functionality.
An example is JSON::Tiny and JSON::Fast. J/Fast was designed to be a drop-in replacement for J/Tiny, which
was first written to demonstrate how to use Perl6 and not as a workhorse module. However, for some reason J/Tiny
has a lot of support, although J/Fast is taking over (see the  ModuleCitation page to trace the historical change).

So the Task::Popular list may have alternate modules for the same functionality. But for a newcomer to the Ecosystem
that might in fact be interesting as it provides a choice, and the opportunity to compare coding styles.

## Updates and Algorithm

The aim is to update the list regularly (eg. monthly).

The algorithm for generating the distribution list is implemented as a method in the [ModuleCitation class](https://github.com/finanalyst/ModuleCitation).
