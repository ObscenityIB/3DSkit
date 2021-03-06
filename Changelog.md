**v1.0**

*	v1.0.0:
	*	Initial release (basic pluggable program)

**v1.1**

*	v1.1.0:
	*	Added unpack.SARC
*	v1.1.1:
	*	Added support for SARCs without files names
	*	Fixed some minor console display issues with packed SARCs due to padding issue

**v1.2**

*	v1.2.1:
	*	Added unpack.DARC and introduced rawutil
	*	rawutil is a module based on struct to handle binary data. It can be used as struct with strings as structures (but wit new elements), or as a TypeReader or TypeWriter object
*	v1.2.2:
	*	Many fixes in rawutil (TypeReader didn't work...)
*	v1.2.3:
	*	Fixed some errors in unpack.DARC, like encoding errors, offsets mismatch or issues due to padding
*	v1.2.4:
	*	Updated rawutil

**v1.3**

*	v1.3.4:
	*	Added pack.SARC and pack.DARC
*	v1.3.5:
	*	Fixed some issues in pack.DARC (other encoding issues and padding errors)

**v1.4**

*	v1.4.5:
	*	Added LZ10 and LZ11 decompression
*	v1.4.6:
	*	Fixed some issues in compress.LZ11

**v1.5**

*	v1.5.6:
	*	Imported ALYTtool content:
	*	Added unpack.BFLYT
*	v1.5.7:
	*	Added pack.BFLYT
*	v1.5.8:
	*	Added unpack.ALYT
	*	Removed usage of formats list in unpack module loading
*	v1.5.9:
	*	Fixes in filesystem utilities (util.fileops)
	*	Updated rawutil

**v1.6**

*	v1.6.9:
	*	Added unpack.CBMD
*	v1.6.10:
	*	Added extraction of LTBL section in unpack.ALYT
*	v1.6.11:
	*	Fixed some rawutil issues with int24 and uint24

**v1.7**

*	v1.7.12:
	*	Added unpack.BCSAR (partial)
*	v1.7.13:
	*	Fixed an issue in pack.BFLYT (pane sections order)

**v1.8**

*	v1.8.14:
	*	Added unpack.BCLYT (partial)
*	v1.8.15:
	*	Little extension of the BCLYT support

**v1.9**

*	v1.9.15:
	*	Added unpack.BFLIM (partial)
	v1.9.16:
	*	Fixed some swizzling issues in unpack.BFLIM

**v1.10**

*	v1.10.16:
	*	Added unpack.GARC
	*	Moved format detection in a new module to avoid recursive imports issue in unpack.GARC
*	v1.10.17:
	*	Added support for version 6 GARCs
*	v1.10.18:
	*	Updated rawutil

**v1.11**

*	v1.11.18:
	*	Added LZH8 and Yaz0 decompression
	*	Fixed issues with int24 in rawutil

**v1.12**

*	v1.12.18:
	*	Added NDS ROMs extraction
*	v1.12.19:
	*	Added support for DSi-specific content
*	v1.12.20:
	*	Updated rawutil
*	v1.12.21:
	*	Fixed some filesystem issues in NitroROM FS extraction

**v1.13**

*	v1.13.21:
	*	Added the plugin system (-g options)
	*	Added FULL support for GFA (GFAC) archives extraction
*	v1.13.22:
	*	Fixed errors in pluginCompiler
	*	Fixed submodule loading issue
*	v1.13.23:
	*	Added plugins.readdata
	*	Added plugins.breaddata
*	v1.13.24:
	*	Fixed readme
	*	Fixed options help
	*	Added plugins help

**v1.14**

*	v1.14.24:
	*	Added pack.ALYT
	*	Fixed a minor padding issue in unpack.SARC
	*	Updated rawutil
	*	Fixed plugin loading issue when other options are specified <br>
*	v1.14.25:
	*	Fixed some bugs in color packing by rawutil
	*	Fixed some bugs in pack.BFLYT (mat1 offsets table length calculation issue, thanks to ericjwg, and materials offsets mismatch)
*	v1.14.26:
	*	Fixed a huge bug with {} structures packing in rawutil
	*	Fixed a stupid error in unpack.SARC

**v1.15**

*	v1.15.26:
	*	Completely rewrote unpack.BFLIM for uncompressed textures, now works fine
*	v1.15.27:
	*	Fixed ETC1 decompression in unpack.BFLIM, now full support of these files
*	v1.15.28:
	*	Changed format-specific options system, now use -O option, see detailed help
	*	Fixed a little problem in rawutil
*	v1.15.29:
	*	Fixed some bugs in RGBA5551, RGB565 and RGB8 packing and unpacking in BFLIM
*	v1.15.30
	*	Fixed the last bug in BFLIM packing on non-power of two textures

**v1.16**

*	v1.16.30
	*	Added BL archives extraction
	*	Added the newmod plugin to replace and extend pluginCompiler
*	v1.16.31
	*	Added BL archive repacking
	*	Fixed a stupid error in unpack.BL
*	v1.16.32
	*	Added a substructure replacement function in rawutil
	*	Completed the changelog and the readme

**v1.17**

*	v1.17.32
	*	Added unpack.NCCH
	*	Added unpack.ExtHeader
	*	Added an error codes system and added the errors help
*	v1.17.33
	*	Updated the readme
	*	Improved colors precision for RGB565 and RGBA5551 formats of BFLIM files
	*	Updated rawutil
*	v1.17.34
	*	Added unpack.ExeFS
	*	Added the dochecks option for unpack.NCCH and unpack.ExeFS to check files and sections hashes
	*	Small orthographic fixes in the help and the changelog
