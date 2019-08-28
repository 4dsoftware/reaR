# reaR

__The same REA, now with R__ 

This analytical tool enables the determination of drug combination effects (i.e., synergy, additivity, or antagonism) at local, regional, and global levels without knowing the inhibition mechanism of drugs. It is written in R, and packaged as a binary file. 

![cover](https://user-images.githubusercontent.com/15344717/32510711-182d3990-c3b7-11e7-9fbc-b1d796fc3706.jpg)

## Installation

To install reaR function from the zip file, open R/RStudio and type:
install.packages('C:/Users/4dsoftware/REA_0.1.0.zip', repos = NULL, type = "win.binary")

## Prerequisites

REA requires two packages to be installed with your R environment, rgl and wvtool. They are available on CRAN. To install, for example, 
install.packages('rgl'). 

## Example

To use REA, one can load it just as other packages using library(). Then load the data whose format should be strictly identical to the example data file. After that, simply run REA with the loaded data, and a draw parameter that controls plotters, 0 for no plot, 2 for 2-D plot, and 3 for 3-D plot. 

_library('REA')_
_data = read.csv('pentamidine_chlorpromazine.csv',header=F)_
_ff = rea(data = data,draw = 2)_


## References
1. Du, D., et al, Response Envelope Analysis for Quantitative Evaluation of Drug Combinations, Bioinformatics, (2019)
