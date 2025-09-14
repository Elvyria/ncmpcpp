# NCurses Music Player Client (Plus Plus)

<img width="1086" height="643" alt="image" src="https://github.com/user-attachments/assets/e48322b8-e2b1-444a-8699-f493ff2eab8c" />


## Changes 

* `sderr` is no longer redirected to the hardcoded path in a `${XDG_DATA_HOME}` location
* removed `search` and `reset` buttons from the search screen, search is now instant
* legacy colors inside of format strings in the config `$1` - `$8` are now effective only inside of their own bracket group
* fixed regexp for `https://genius.com` lyric fetcher
* configurable nerd font icons for the state flags `state_flags_consume_look`, `state_flags_crossfade_look`, `state_flags_db_update_look`, `state_flags_random_look`, `state_flags_repeat_look`, `state_flags_repeat_single_look`, `state_flags_single_look`
* configurable player state message `state_player_playing_look`, `state_player_paused_look`, `state_player_stopped_look`, `state_player_unknown_look`
* `--ignore-config-errors` flag is removed, config errors are ignored by default

## ncmpcpp – featureful ncurses based MPD client inspired by ncmpc

### Main features:
* tag editor
* playlist editor
* easy to use search engine
* media library
* music visualizer
* ability to fetch artist info from last.fm
* new display mode
* alternative user interface
* ability to browse and add files from outside of MPD music directory
…and a lot more minor functions.

### Dependencies:
* [boost](https://www.boost.org/)
* [ncurses](https://invisible-island.net/ncurses/announce.html)
* [readline](https://tiswww.case.edu/php/chet/readline/rltop.html)
* [curl](https://curl.se), for fetching lyrics and last.fm data
#### Optional
* [nerd font](https://www.nerdfonts.com), to properly display new icons
* [fftw](http://www.fftw.org), for frequency spectrum music visualization mode
* [taglib](https://taglib.org/), for tag editing

### Known issues:
* No full support for handling encodings other than UTF-8.

### Installation:
The simplest way to compile this package is:

  1. `cd` to the directory containing the package's source code.

  For the next two commands, `csh` users will need to prefix them with
  `sh `.

  2. Run `autoreconf -fiv` to generate the `configure` script.

  3. Run `./configure` to configure the package for your system.  This
     will take a while.  While running, it prints some messages
     telling which features it is checking for.

  4. Run `make` to compile the package.

  5. Type `make install` to install the programs and any data files
     and documentation.

  6. You can remove the program binaries and object files from the
     source code directory by typing `make clean`.

Detailed intallation instructions can be found in the `INSTALL` file. 

### Optional features:
Optional features can be enable by specifying them during configure. For
example, to enable visualizer run `./configure --enable-visualizer`. 

Additional details can be found in the INSTALL file. 
