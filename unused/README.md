# blandr: a Bland-Altman package for R

*blandr* is a package to carry out Bland-Altman analyses (also known as a Tukey mean-difference plot) in R. This package was started in 2015 as existing Bland-Altman R functions did not calculate confidence intervals: my belief is that when drawing Bland-Altman plots, confidence intervals should be considered the gold-standard. *blandr* fills this need!

*blandr* further generates plotting data to allow easy generation of charts using ggplot, as well as R's in-built drawing capabilities.

## Why should I use it?

To get an open-source library that allows replicable Bland-Altman analysises using R. Further it generates and plots confidence intervals for Bland-Altman method comparisons: something that other libraries do not seem to generate.

## How do I get it?

Currently the code is hosted at https://github.com/deepankardatta/blandr/ - in future I hope it will be available on CRAN for easy integration into R

## How do I use it?

As the library is not on CRAN (yet) the best way is to:
1. download the code
2. build the package
3. load the package - library(blendr)
4. see the vignettes for test cases

## Why release a version <1.0?

I am believer that if the function is good enough to work, I should just publish, see if others can improve it and just iterate slowly to get to a version 1.0. What counts as a 1.0? Well I'd like other people to help validate it, and add a few more functions, to a point there should not be much more to add to this.

From what I've read this is what's called a "Minimum Viable Product" (https://en.wikipedia.org/wiki/Minimum_viable_product).

## Why the name?

Thinking of a unique name was difficult - and it wasn't worth spending/wasting time on this initially. Curiously it was going to be called BlandAltmanEdinburgh (as I was in Edinburgh at the time I made this) until I considerd uploading this to GitHub and CRAN.

Hadley Wickham has an excellent set of documentation on creating packages. The one on naming (http://r-pkgs.had.co.nz/package.html) is worth a read. Reflecting on it a lot of the naming issues are to prevent collisions with similarly named packages, so using *blandaltman* in the name might have cause problems. Mirroring the pre-existing *plyr* and *knitr* I thought I'd just add a "r" to "bland": yes it doesn't involve Altman's name, but I couldn't think of anything better.

If you can think of a better name please let me know!

## Further information

Further information can be found in the function help files in the package, as well as in the vignettes.

## Future improvements

Whilst this package is good enough for use, there is the scope for iterative improvements.

Future works include:
* I need to take out the last references to *BlandAltmanEdinburgh* and change it to *blandr*.
* There are a further few deprecated functions to delete (I just need to finish a few projects first!!).
* The package needs to have to go through some validation and testing
* For further testing I need to write some *testhtat* modules
* The function descriptions needs to be improved
* Some of the roxygen2 documentation can be improved by calling the import parameters function
* I want to add a few more sample data packs: including some of my own if possible!

## Help wanted!

Comments on the code, suggestions for improvement, verification tests, validation studies, and even code contributions would be gratefully accepted. Email me at deepankardatta@users.noreply.github.com and I'll try and get back to you as soon as possible. Please do bear in mind this is a side-project, and I can be otherwise busy with a lot of other work.
