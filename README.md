# Task::Popular
## Introduction

The developers of Perl6 decided early on that the implementation
of the language (eg. Rakudo) would be available with a bare minimum of "core" modules.
Some modules are essential, such as Test, or the module manager (previously `panda`, currently `zef`).

Rakudo is available with some modules in a distribution called `Rakudo Star`.

However, for someone coming to Perl6 for the first time, there is a natural question as to which
modules 'should' be installed first. Since 'should' is subjective, there is no real solution.

Another problem (at the time of writing) is that Perl6 has a rapidly expanding user base, and the language
continues to evolve. This means that modules which were well-tested and useful at one moment in time are being
replaced by other modules. Consequently, any list of 'necessary' modules that is chosen by someone has to
be monitored on a regular basis, as some of the modules in the list become dated.

This distribution list takes another approach.

Some modules are used far more than others in the Ecosystem. Consequently, by chosing a set of modules that are
frequently used, it can be fairly safely assumed they will be regularly maintained.

This list uses [Citation Indices](http://finanalyst.github.io/ModuleCitation/) to identify the 30 modules most recursively popular modules in the Ecosystem.

## Problems

Inevitably for commonly needed functionality, there may be multiple modules that provide the same functionality.
An example is JSON::Tiny and JSON::Fast. J/Fast was designed to be a drop-in replacement for J/Tiny, which
was first written to demonstrate how to use Perl6 and not as a workhorse module. However, for some reason J/Tiny
has a lot of support, although J/Fast is taking over (see the  ModuleCitation page to trace the historical change).

So the Task::Popular list may have alternate modules for the same functionality. But for a newcomer to the Ecosystem
that might in fact be interesting.

## Updates

The aim is to update the list regularly (eg. monthly).

## Software

The algorithm for generating the distribution list is implemented as a method in the [ModuleCitation class](https://github.com/finanalyst/ModuleCitation).

## Modules in this distribution

| Module Name | Recursive Citation Index |
|---| :---: |
| JSON::Fast | 32.69 |
| MIME::Base64 | 25 |
| File::Directory::Tree | 23.46 |
| File::Temp | 23.08 |
| URI | 21.54 |
| HTTP::Status | 20.38 |
| JSON::Tiny | 18.08 |
| JSON::Name | 13.85 |
| Encode | 13.46 |
| DateTime::Parse | 13.08 |
| HTTP::UserAgent | 12.69 |
| JSON::Unmarshal | 12.69 |
| JSON::Marshal | 12.31 |
| JSON::Class | 11.54 |
| XML | 11.54 |
| OpenSSL | 11.15 |
| Terminal::ANSIColor | 11.15 |
| Digest | 9.62 |
| META6 | 8.85 |
| PSGI | 8.85 |
| Test::META | 8.08 |
| File::Find | 7.69 |
| IO::Socket::SSL | 7.69 |
| DateTime::Format | 7.31 |
| File::Which | 7.31 |
| LibraryMake | 7.31 |
| HTTP::Easy | 6.54 |
| Digest::HMAC | 6.15 |
| JSON::Pretty | 6.15 |
| LWP::Simple | 6.15 |