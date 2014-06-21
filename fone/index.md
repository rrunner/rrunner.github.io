---
title       : Fone
subtitle    : Formula 1 results and locations
author      : rrunner
job         : Developing Data Products
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []   # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---




## Fone

- **Fone** is a simple shiny application that presents circuit location on a world map and race results in two separate tabs
- Receives two user inputs: Year and circuit

---

## Source data and API

> - **Fone** utilises the [Ergast API](http://ergast.com/mrd/)
> - Downloads data as JSON objects 
> - Convert to data frames before display 

---

## Race locations

- Race locations are displayed in the first tab
- The current selected circuit is marked red on the world map

![plot of chunk worldmap](assets/fig/worldmap.png) 


---

## Race results

- Results are listed in the second tab
- For example, the podium finishers at the Melbourne 2014 race are:

<!-- html table generated in R 3.1.0 by xtable 1.7-3 package -->
<!-- Sat Jun 21 02:49:09 2014 -->
<TABLE border=1>
<TR> <TH>  </TH> <TH> pos </TH> <TH> no </TH> <TH> driver </TH> <TH> constructor </TH> <TH> laps </TH> <TH> grid </TH> <TH> status </TH> <TH> points </TH>  </TR>
  <TR> <TD align="right"> 1 </TD> <TD> 1 </TD> <TD> 6 </TD> <TD> Nico Rosberg </TD> <TD> Mercedes </TD> <TD> 57 </TD> <TD> 3 </TD> <TD> Finished </TD> <TD> 25 </TD> </TR>
  <TR> <TD align="right"> 2 </TD> <TD> 2 </TD> <TD> 20 </TD> <TD> Kevin Magnussen </TD> <TD> McLaren </TD> <TD> 57 </TD> <TD> 4 </TD> <TD> Finished </TD> <TD> 18 </TD> </TR>
  <TR> <TD align="right"> 3 </TD> <TD> 3 </TD> <TD> 22 </TD> <TD> Jenson Button </TD> <TD> McLaren </TD> <TD> 57 </TD> <TD> 10 </TD> <TD> Finished </TD> <TD> 15 </TD> </TR>
   </TABLE>
