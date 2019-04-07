## Matlab deployed FINCH executable

If you do not have Matlab to run [FINCH](https://github.com/ssarfraz/FINCH-Clustering). You can download the deployed [FINCH executable here](https://drive.google.com/open?id=1l6JhMjlTCwirA1M0vIHRe1FZsfYPMqkX)

Download and install [Matlab runtime](http://www.mathworks.com/products/compiler/mcr/index.html) (free). Go to the downloaded FINCH executable dir and run the FINCH from the command prompt as follows


```
./run_FINCH.sh YOUR-MCR-PATH/v95/ YOUR-Data-PATH/data.csv Output-Path verbose req_clust
```
Please also see the matlab generated readme.txt for more details.

You can run it on your data written as a csv file (feature vectors/samples to cluster should be written as rows). A sample mice protein data.csv is provided (1077 samples each 77 dimensional).

** Input arguments
* path to the matlab runtime MCR
* path to your data csv file
* path to write the output, it will write the returned c mat, num_clust and req-clust (if specified) as csv files here
* verbose. 1 for write some output on screen
* req_clust: 0 (to not run into required number of cluster mode) OR provide your required number of cluster

Typical command

```
./run_FINCH.sh YOUR-MCR-PATH/v95/ YOUR-Data-PATH/data.csv Your-output-Path 1 0
```
   





See the read me of  [FINCH repo here](https://github.com/ssarfraz/FINCH-Clustering) for details on the meaning of these outputs.

