# Supplementary material for ExtnSpaces paper

This repository contains the Figures shown in the Supplementary material of the paper, as well as the Results discussed in the Exploration of the Algorithm Performance and the Real World Application, along with the necessary code and instructions to reproduce it. 

To perform the following analysis, download both the .jar and the Input Files to the same folder in your computer. 
    
## Algorithm Performance  

To reproduce the exploration in this repository, employ the following code:

```sh
java -jar ExtDistExecutor.jar InputTreeList.txt -d Results -o ExtDistance -T -l 500
```

Here we require the Table with information for each Orthant Pair to be printed, but only with 500 lines to keep the file size small. To see the whole data used in the paper: 


```sh
java -jar ExtDistExecutor.jar InputTreeList.txt -d Results -o ExtDistance -T
```

## Data Analysis

To reproduce the data analysis, employ

```sh
java -jar ExtDistExecutor.jar GeneTrees.txt -d Results -o Distance -T -l 500 -k 8
```

Here we are multi-threading with 8 threads in total. Again, remove `sh -l 500` to obtain the full data we use in our analysis. 