**Author**: Swetha Yadavalli

**Programming Language**: Python

**Dependencies**:
- pandas
- gzip

**Files required**:
- E_coli_K12_MG1655.ptt.gz
- B_subtilis_168.ptt.gz
- Halobacterium_NRC1.ptt.gz
- Synechocystis_PCC6803_uid159873.ptt.gz

## Description

This script predicts operons from .ptt and .gff files. It creates dataframes for each file and then does the pre-processing steps required to produce the correct format of the dataframes. The operons function is used on these DataFrames to discover potential operons based on gene proximity and strand orientation. Genes are grouped into operons if they are on the same strand and less than 50 base pairs away. The script also processes a .gff file in a similar fashion, renaming columns for consistency and using the same operon identification algorithm.

## Execution Steps

1. Intially load the .gz files and unzip them.  
2. Create the dataframes from each files. 
3. Split the location column into start and end. 
4. Write the operons function to predict the operons for each .ptt file 
5. Use the same function to find the operons in the .gff file. 
6. The final outputs can be checked after running the code. 

## Output Files

The final .pynb can be accessed for the output. 
