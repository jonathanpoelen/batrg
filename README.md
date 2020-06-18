# Batrg

Search and highlight files using ripgrep (rg) and bat.


## Usage

    batrg [OPTIONS] PATTERN [PATH ...]
    batrg [OPTIONS] [-e PATTERN ...] [-f PATTERNFILE ...] [PATH ...]
    command | batrg [OPTIONS] PATTERN


## Pattern and PATTERNFILE

See `rg`


## Options

- `--snip` \
  \
  Show the snip decoration (see `bat --style=...`). \
  \
  This is automatically disabled when `--context=0` (see `bat`).

- `--no-snip` \
  \
  Disable `--snip`.

- `--highlight` \
  \
  Highlight matching lines. \
  \
  This is automatically disabled when `--context=0` (see `bat`).

- `--no-highlight` \
  \
  Disable `--highlight`.

- `--file-separator=<separator>` \
  \
  Character used by the separation line between 2 files, or string separator.

- `--file-separator-wrap` \
  \
  If a match is found, appends the separator line above  the  first file and below the last file.

- `--no-file-separator-wrap` \
  \
  Disable `--file-separator-wrap`.

- `--paging=<when>` \
  \
  Specify when to use the pager. To control which pager is used, set the `PAGER` or `BAT_PAGER` environment variables (the latter takes precedence) or use the `--pager` option. To disable  the pager permanently, set `--paging=never`. \
  \
  Possible values: `auto`, `never`, `always`, `one-by-one`.

- `--bat-engine=<command>` \
  \
  Specify command for `bat`. By default use `BATRG_BAT` environment variables or `bat`.

- `--rg-engine=<command>` \
  \
  Specify command for `rg`. By default use `BATRG_RG` environment variables or `rg`.

Another options are passed directly to `ripgrep` or `bat`.


## Dependencies

- `zsh`
- `bat`
- `rg`


## Installation

Just put `batrg` in a `PATH` folder and `completion/_batrg` in a completion folder.
