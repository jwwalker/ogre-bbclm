# ogre-bbclm

## What it is

When developing 3D rendering software using [Ogre](https://github.com/OGRECave/ogre) or
[Ogre-Next](https://github.com/OGRECave/ogre-next), you'll probably need to write some
script files for compositors, materials, and perhaps particle systems.  You can do that
using any plain text editor, but it's easier to write and maintain these scripts with
the aid of features like syntax coloring, code folding, and a menu of top-level objects.

If you're developing on macOS, you may be using [BBEdit](https://www.barebones.com/products/bbedit/)
for code editing.  BBEdit has built-in support for many common programming languages, but
provides for a plug-in called a [Codeless Language Module](https://www.barebones.com/support/develop/clm.html)
to help BBEdit understand other languages.  I have constructed a BBEdit language module
for Ogre scripts of types `.compositor`, `.material`, and `.particle`.  The features
provided are:

* Syntax coloring for keywords, comments, numbers, and strings
* Names of top-level constructs such as `compositor_node` and `material` appear in BBEdit's
pop-up menu of "functions", making it possible to quickly jump to those sections of the
script
* code folding is available for those top-level groups

## How to Use It

BBEdit language modules are stored in the folder `~/Library/Application Support/BBEdit/Language Modules`.
Insert the `Ogre script language module.plist` file in that folder.  If BBEdit was already
running, you will need to restart it to make it notice the new language module.

When you open a file with extension `.compositor`, `.material`, or `.particle`, BBEdit
should automatically select "Ogre script" in the pop-up menu of languages at the bottom
of the editing window.  If you're creating a new script, you may need to select
"Ogre script" yourself.


