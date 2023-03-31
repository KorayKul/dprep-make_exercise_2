analysis: ../../gen/output/plot_all.pdf ../../gen/output/plot_Antwerp.pdf

../../gen/output/plot_Antwerp.pdf: plot_Antwerp.R ../../gen/temp/pivot_table.csv
	r --vanilla < plot_Antwerp.R

../../gen/output/plot_all.pdf: plot_all.R ../../gen/temp/aggregated_df.csv
	r --vanilla < plot_all.R







# Variables can be used like this: 
# TEMP = ../../gen/temp
# DATA = ../../data
# $(TEMP)/aggregated_df.csv: $(DATA)/listings.csv $(DATA)/reviews.csv  clean.R
#    R --vanilla < clean.R