Arabic

apertium-ara  
===

This is an Apertium monolingual language package for Arabic. What  
you can use this language package for:

-   Morphological analysis of Arabic
-   Morphological generation of Arabic
-   Part-of-speech tagging of Arabic

Requirements  
===

You will need the following software installed:

-   lttoolbox (&gt;= 3.3.0)
-   apertium (&gt;= 3.3.0)
-   vislcg3 (&gt;= 0.9.9.10297)

If this does not make any sense, we recommend you look at:
www.apertium.org

Compiling  
===

Given the requirements being installed, you should be able to just run:

$ ./configure  
$ make

You can use ./autogen.sh instead of ./configure if you're compiling  
from SVN.

If you're doing development, you don't have to install the data, you  
can use it directly from this directory.

If you are installing this language package as a prerequisite for an  
Apertium translation pair, then do (typically as root / with sudo):

1.  make install

You can give a --prefix to ./configure to install as a non-root user,  
but make sure to use the same prefix when installing the translation  
pair and any other language packages.

Testing  
===

If you are in the source directory after running make, the following  
commands should work:

$ echo "TODO: test sentence" | apertium -d . ara-morph  
TODO: test analysis result

$ echo "TODO: test sentence" | apertium -d . ara-tagger  
TODO: test tagger result

Files and data  
===

-   apertium-ara.ara.dix - Monolingual dictionary
-   ara.prob - Tagger model
-   apertium-ara.ara.rlx - Constraint Grammar disambiguation rules
-   apertium-ara.post-ara.dix - Post-generator
-   modes.xml - Translation modes

For more information  
===

-   http://wiki.apertium.org/wiki/Installation
-   http://wiki.apertium.org/wiki/apertium-ara
-   http://wiki.apertium.org/wiki/Using\_an\_lttoolbox\_dictionary

Help and support  
===

If you need help using this language pair or data, you can contact:

-   Mailing list: apertium-stuff@lists.sourceforge.net
-   IRC: \#apertium on irc.freenode.net

See also the file AUTHORS included in this distribution.
