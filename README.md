This document aims to instruct how to use new tree algorithms "EXICtree" in R program. The source codes  include four function according to  four kinds of tree. 
A  R package"EXICtree" is created. "EXICtree" is implemented based on the "partykit" R package .
Step 1) Activate "partykit" R package, ie. library(partykit).
Step 2)Load "EXICtree_0.1.0.tar.gz" file to R ,library(EXICtree).
Example
library(partykit)
library(interval)
library(EXICtree)
data(bcos)
tree <- ICStree1(Surv(left,right,type="interval2")~treatment, data = bcos,0.05,0.2)
