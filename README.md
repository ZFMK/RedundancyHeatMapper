# RedundancyHeatMapper
A perl script designed to generate heat maps from matrices of lambda values generate by Saturation v1.0

## NOTES REGARDING SOFTWARE

### NAME        
RedundancyHeatMapper

### VERSION     
1.1

### COPYRIGHT   
Copyright © 2013-2022 Bernhard Misof. All rights reserved.

### WARNING     
The copyright holder takes no legal responsibility for the correctness of results obtained using this program.

### AUTHOR      
Bernhard Misof

### ADDRESS     
Center for Molecular Biodiversity Research
Zoological Research Museum A. Koenig
Bonn, Germany

### CONTACT     
b.misof@leibniz-zfmk.de

### DATE        
17 May 2013

### UPDATE      
16 June 2022

### PURPOSE     
RedundancyHeatMapper produces a heat map from a distance matrix with values of lambda obtained by SatuRation (https://github.com/lsjermiin/SatuRation.v1.0).
            
Lambda is a measure of the strength of the historical signal between a pair of sequences. If lambda = 0, there is no evidence of loss of historical signal; 
if lambda = 1, the historical signal has decayed completely.
            
The higher lambda is, the darker the corresponding pixel in the heat map is.

Emphasis is on lambda values between 0.0 and 0.37, allowing pairs of sequences that are most similar to one another to be identified.
            
### FORMAT      
Lambda values must be saved in a text file with comma-separated values (.csv).

The first line must contain the number of samples being compared. 

Each of the following lines must start with a sample name, and then followed by the lambda values, one for each comparison involving the named sample.
 
### EXAMPLE     
See file labelled 0_Recombination_lambda.csv.

### INSTALL     
To install RedundancyHeatMapper.pl, type (in the command line):

    sudo cp RedundancyHeatMapper.pl /usr/local/bin/. 

### EXECUTE     
    RedundancyHeatMapper -i <infile.csv> <-t|f>

### HELP        
    -t = triangular heat map; -f = square heat map

### STATUS      
Software complete

### NOTE        
Contact author for updates, etc

### REFERENCE   
Jermiin LS, Misof B. Quantifying the historical signal in phylogenetic data. Syst. Biol. (In prep.)