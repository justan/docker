# Docker Version History

## 0.2.6

 * Fix a weird bug in SCSS parsing

## 0.2.5

 * Fix for file paths in windows (`\` as a path separator broke things)
 * Throw errors on filesystem exceptions

## 0.2.4

 * Update watchr dependency
 * Tweaks to fileSearch extra

## 0.2.3

 * Lots of minor tweaks and improvements

## 0.2.2

 * Fixes for indented multiline comments and indented comments in CoffeeScript

## 0.2.1

 * Temporarily disable multiline comments in SASS and SCSS as `/*` can be used to open a single-line comment. Will reinstate when I have time to figure it out properly

## 0.2.0

 * Added `--js` and `--css` options to specify extra CSS and JavaScript files to include
 * Added optional `-n` flag to enable line numbers in output
 * Added "disable" value for sidebar to hide it completely
 * Added support for matching files by name rather than just extension (e.g. Makefile)
 * Added first two "extras" - optionally enable-able extras for the output
   - **fileSearch**: performs fuzzy-matching on file names to quickly jump to a file
   - **goToLine**: quickly jump to a line in the source. Currently only works if line numbers are enabled
 * Fixed some bugs in Markdown parsing
 * Improvements to indentation detection
 * Fixed bug where processing only updated files would result in an empty tree

## 0.1.8

 * Removed dependency on dox; wrote more concise version of jsDoc parser based on dox, but which handles headings correctly
 * Bugfixes for watch mode.

## 0.1.7

 * Bugfix: indented jsDoc was breaking.

## 0.1.6

 * Added support for VB.NET, ASP C# and ASP VB courtesy of [peterhost](https://github.com/peterhost)

## 0.1.5

 * Added smarter handling of symbolic links, allowing for handling of dead links

## 0.1.4

 * Added language type detection from shebangs

## 0.1.3

 * Added `-s` option to specify default state of the sidebar
 * Added `-x` option to specify paths to exclude
 * Renamed `tree` to `sidebar` in some of the markup.

## 0.1.2

 * Windows compatibility
 * Resolve infinite loop problem when files aren't actually inside the source dir
 * A few minor typos

## 0.1.1

 * Fixed problem with comment delimiters being matched inside string literals

## 0.1.0

 * Added `-w` flag to watch a directory for changes (experimental). Not sure how useful it'll actually be, but it's cool.
 * Added `-I` switch to ignore hidden files
 * Fixed some rendering bugs for code blocks
 * Added automatic title generation for empty-looking files
 * Various styling tweaks

## 0.0.9

 * Added support for another pile more languages (added perl, php, actionscript, sh and yaml)
 * Ran embedded arrow images through pngcrush.  Saved a load of bytes

## 0.0.8

 * Added support for different colour schemes
 * A few more improvements to showdown for GFM-style bits.

## 0.0.7

 * Minor improvements to code structure
 * Full comments on public script file

## 0.0.6

 * Added support for a pile more languages (now JS, coffeescript, ruby, python, C, C++, C#, Java and Markdown)
 * Tweaks to markdown (particularly, automatic linking of URLs and email addresses)

## 0.0.5

 * Added heading navigation within files

## 0.0.4

 * Added syntax highlighting to fenced code blocks that have a language specified

## 0.0.3

 * Minor improvements to store the scroll position of the folder tree

## 0.0.2

 * Added `-u` flag to only process files that have been updated

## 0.0.1

Initial version indcluded (among other things):

 * Folder tree
 * Syntax highlighting of javascript files
 * Markdown processing of `.md` files and extracted code comments
