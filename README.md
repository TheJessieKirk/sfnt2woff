# *sfnt2woff* README
This is a mirror and build of Jonathan Kew's *sfnt2woff* tool.

*sfnt2woff* and *woff2sfnt* are built for *x86_64-linux-pc-gnu* hosts.

They convert font files from SFNT (OpenType and TrueType) formats to WOFF format and *vice-versa*.<br />
(Note: they can't handle WOFF2 files.)

Jonathan Kew's website has been down since 2017, but an archived version is available from the [Internet Archive](https://web.archive.org/web/https://people.mozilla.org/~jkew/woff/).

## Usage

### Converting an SFNT font to a WOFF font

<code>./sfnt2woff [-v \<maj>.\<min> [-m \<metadata.xml>] [-p \<private.dat>] \<sfntfile></code>
      
Options:

<code>-v \<maj>.\<min></code> - set font version number (major and minor, both integers).<br />
<code>-m \<metadata.xml></code> - inlude metadata from <metadata.xml> (not validated).<br />
<code>-p \<private.dat></code> - include private data block.<br />
    
Parameters:
    
<code>\<sfntfile></code> - OTF or TTF file to be converted to WOFF.

### Converting a WOFF font to an SFNT font

<code>./woff2sfnt [-v | -m  | -p] \<wofffile></code>

Options (only one option can be specified at a time):

<code>-v \<maj>.\<min></code> - write font version to stdout, instead of converting WOFF file.<br />
<code>-m \<metadata.xml></code> - write WOFF metadata block to stdout, instead of converting WOFF file.<br />
<code>-p \<private.dat></code> - write WOFF private data block to stdout, instead of converting WOFF file.<br />

Parameters:
    
<code>\<wofffile></code> - WOFF file to be converted to OTF.
    
## Mirror Differences

The following files are new and were not in the original *sfnt2woff* release:

* LICENSE-gpl-2
* LICENSE-lgpl-2-0
* LICENSE-mpl-1-1
* LICENSE.md
* README.md
* sfnt2woff
* sfnt2woff.o
* woff.o
* woff2sfnt
* woff2sfnt.o

All other files are original and unedited.

## License

See [LICENSE.md](https://github.com/TheJessieKirk/sfnt2woff/blob/main/LICENSE.md) for details.

## Copyright

I don't own this software and I'm simply providing a mirror of it, but I'm Jessie Kirk. Anyways…

*sfnt2woff* is Copyright © 2009, Trademark ™ and/or Registered Trademark ® Jonathan Kew and [Mozilla Corporation](https://www.mozilla.org/).

*WOFF* is Copyright © 2009, Trademark ™ and/or Registered Trademark ® [LettError Type/Erik van Blokland](https://letterror.com/), [Microsoft Corporation](https://www.microsoft.com/), [Mozilla Corporation](https://www.mozilla.org/), [Opera](https://www.opera.com/) and [Type Supply LLC/Tal Leming](https://typesupply.com/).
