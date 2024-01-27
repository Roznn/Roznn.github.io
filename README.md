# Roznn.github.io

This repo has the files for my website  [https://roznn.github.io/](https://roznn.github.io/)

Using icons from [https://jpswalsh.github.io/academicons/](https://jpswalsh.github.io/academicons/)

The file [works.bib](works.bib) is exported from/imported to my [Orcid](https://orcid.org/0000-0003-0983-3052)  and processed with https://bibbase.org/ using the raw path https://raw.githubusercontent.com/Roznn/Roznn.github.io/master/works.bib . 
The script created by [bibbase](https://bibbase.org/) is included  in the publication section of my webpage [index.html](index.html) to create the list of publications. 

Updating  [works.bib](works.bib) automatically update the list of publications via bibbase.

To check formatting errors in the bib file, use biber:
```
biber --tool -V works.bib
```

## Alternative to bibbase 


Using pandoc the bib file can be converted in html: 
```
pandoc test.tex -o pub.html --bibliography works.bib
```
or in PDF
```
pandoc test.tex -o pub.pdf --bibliography works.bib
```

## with tex4ht

https://www.tug.org/tex4ht/

```
pdflatex test
biber test
make4ht  test.tex 
```

## mindmap tool used 

https://forge.aeif.fr/eyssette/myMarkmap/



## Author: 

[Rozenn Dahyot](https://roznn.github.io/)

