# internaldata

The goal of internaldata is to demonstrate a problem with trying to call internal package data objects in a function factory sourced from the `R/` directory.

```
> install()
Installing internaldata
'/Library/Frameworks/R.framework/Resources/bin/R' --no-site-file --no-environ --no-save --no-restore --quiet CMD  \
  INSTALL '/Users/admin/Development/internaldata'  \
  --library='/Library/Frameworks/R.framework/Versions/3.5/Resources/library' --install-tests 

* installing *source* package ‘internaldata’ ...
** R
** byte-compile and prepare package for lazy loading
Error in lapply(list(x = x), function(x) return(x)) : 
  object 'x' not found
Error : unable to load R code in package ‘internaldata’
ERROR: lazy loading failed for package ‘internaldata’
* removing ‘/Library/Frameworks/R.framework/Versions/3.5/Resources/library/internaldata’
* restoring previous ‘/Library/Frameworks/R.framework/Versions/3.5/Resources/library/internaldata’
Error: Command failed (1)
```
