# Biology-Assignment-2
The functionality of the code is explained within the assignment writeup, an overview of each step can be found below:

- Steps 1->5: read_delim() function is used to import all the data from the dataset
- Step 6: Since the patient ID is slightly different between the datasets, the string is reduced to just the first 12 characters and the \\ are replaced by -. The number of IDs and the heads of the datafrane were then printed out to ensure everything was working properly. Once the IDs were all formatted the same way, they could be matched using the intersect function.
- Step 7: A bar chart was then created showing the distribution of which samples had an amplified or non-amplified ERBB2 gene. 
- Step 8 & 9: The DESeq2 library is an excellent package for numerical processing and we can use it to find the most differentially expressed genes by ranking them based on the log2FoldChange of each gene.
- Step 10: Pathway enrichment analysis was carried out using 3 different reference datasets, the gene ontology dataset is used with the enrichGO() function, the Reactome with the enrichPathway() function and the Kegg repository with the enrichKEGG() function . Dotplots were then created using the dotplot() function to find which types of genes were most differentially expressed.
- Step 11: The variance stabilised transformed expressio values were calculated using the vst() function
- Step 12: The PCA plot was visualised using the plotPCA() function and the heatmap was created using the pheatmap library.
-Step 13: Finally a survival cox model was created using the survival package and a cv model. The specifics for this can be found in the assignment write up. The final survival probability was then plotted using the plot() function
