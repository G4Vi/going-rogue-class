# Going Rogue with Metamodern Perl

## Getting Started

Perl v5.40 is required, perlbrew may be the easiest way to install https://perlbrew.pl/

### Linux

Currently, forked Alien-raylib5 is required, with cpanm:

```bash
cpanm https://github.com/perigrin/Alien-raylib5.git
```
Then, the rest of the dependencies can be installed with:

```bash
cpanm --installdeps .
```
### OSX

On OSX you need install with homebrew and App::cpm:

```perl
    brew install raylib
    PKG_CONFIG_PATH="/opt/homebrew/opt/libffi/lib/pkgconfig" cpm install
```
### Other

On other systems the installation dance is left as a lemma for the reader.
Alien::raylib currently will build an older version of Raylib so you need to
use a system library, or a patched version of Alien::raylib.

## Running the game

```bash
perl bin/game.pl
```
A Windows should appear with a green `@`, controllable with the arrow keys.

You may need to comment out `use local::lib qw(local);` in `game.pl` .
