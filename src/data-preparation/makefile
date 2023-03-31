prep: ../../data/reviews.csv data/listings.csv ../../gen/temp/aggregated_df.csv ../../gen/temp/pivot_table.csv

## Sub-build Rules

../../data/reviews.csv data/listings.csv: download.R
	R --vanilla < download.R

../../gen/temp/aggregated_df.csv: clean.R ../../data/reviews.csv ../../data/listings.csv
	R --vanilla < clean.R

../../gen/temp/pivot_table.csv: pivot_table.R ../../gen/temp/aggregated_df.csv
	R --vanilla < pivot_table.R
