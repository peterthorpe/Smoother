# Smoother
Smooths data from plate-based assays.
############################## Z score smoothing script  #####################################
# This script takes an input table with the following format, usually copied from a spreadsheet.
# Please ensure that you have saved the input table using a text editor that uses standard line breaks
# Note that saving the file from excel often does not have standard line breaks.
#
# plate <tab> row <tab> column <tab> ORF <tab> score <tab> score etc... as many scores as you like
# please include column headings in the first row, particularly if you have many scores.
# The first column heading must be the word "plate" (case not important), otherwise the heading won't be recognised
#
# There can be any number of plates, and each plate can have any number of rows and columns
# Columns are numerical, where as rows are letters (A, B, C etc)
#
# The script adjusts the scores (assumed to be Z scores) based upon column and row averages relative to the median plate value
# The scores should be numerical not text, although the script makes some attempt to parse out text from the scores
# 
#
# Written in 2013 by Peter Thorpe
