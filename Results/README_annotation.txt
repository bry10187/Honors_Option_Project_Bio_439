#### How extracted file was annotated

#Open both raw_counts_annotated.csv and results csv file on two windows in excel

#Create a new empty column in excel in the results file to the right the Gene id column

#Name gene id column as Gene_id and the new column as Gene_name

#Use the following command in cel B2
VLOOKUP(A2, raw_counts_annotated.csv!$B:$C, 2, FALSE)

#A2 is the cell with the first gene id
#Next part specifies the matrix in the annotation file, which consists of the gene.id column and the gene.name column
#The next number 2 indicates that number of column index number, in this case we have 2 columns
#FALSE indicates that we are looking for an exact match

Then, saved the file as an Excel workbook as "results_atphb3.ANAC017_vs_wild.xlsx" to prevent data loss