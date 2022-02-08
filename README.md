Convert PRESTO's rfifind mask output to ascii files. 

Use:
-----------------
If you want the code to run its own rfifind command then just supply filterbank with necessary parameters 
> python rfi_filter.py -fil <input filterbank file> -time 30.0 -timesig 10.0 -freqsig 4.0 -chanfrac 0.7 -intfrac 0.3 -max_percent 20.0 

If you already have a .mask file from your own rfifind run then just supply filterbank file (required to get the source name) and mask file.

> python rfi_filter.py -fil <input filterbank file> -mask <your mask file> 


output:
-----------------
It outputs various files. The file with chan.kill has a two columns, with first column showing channel number and second column showing flagging status. 

