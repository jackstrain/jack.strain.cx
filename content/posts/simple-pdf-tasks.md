+++
title = 'Simple PDF Tasks on Ubuntu/Linux'
date = 2023-09-28T23:35:31+01:00
tags = ['linux', 'pdf', 'ubuntu']
draft = false
+++
## Converting PDFs to Images
Required is the `poppler-utils` package, which should be installed by default on Ubuntu.  
For a whole file:  
```pdftoppm input.pdf outputname -png```  
For one or more pages of a file:  
```pdftoppm input.pdf outputname -png -f {page} -singlefile```  
where `{page}` is the page number, i.e. `-f 1` would be the first page.  
A range can be specified like so `-f 1 -l 5` where `-l` specifies the last page.  

## Compressing PDFs
Compression can be achieved with `ps2pdf` like so:  
```ps2pdf input.pdf output.pdf```  
