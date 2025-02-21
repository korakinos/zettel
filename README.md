# Zettel CLI -- **private fork**
My version of a dead simple zettel CLI.

WARNING: Requires [the silver searcher](https://github.com/ggreer/the_silver_searcher)

Works better when combined `vim` and [zettel-vim](https://github.com/grantmiiller/zettel.vim)

## What is Zettel?
Stands for [Zettelkasten](https://zettelkasten.de/)

## The ID system
This version uses the bash `date` command with `%Y%m%dT%H%M%S` as the format string. [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations)

## How to use
Make sure the `zettel` bash script is in your execution path

Make sure you have the `ZETTEL_DIR` environment variable set to where you want your notes, else this program will default to the current directory.

Run `zettel` to see the usage.

### Example: Creating notes
The following will create a new note with the name `<ID> Hello World.md` and add the id to your clipboard, as well as echo it.

`zettel -i new "Hello World"`

The following will will do the same as above expect instead echo the filepath and copy it your clipboard.

`zettel -f new "Hello World"`

#### The rest of the commands are more intended for the [zettel-vim](https://github.com/grantmiiller/zettel.vim)

