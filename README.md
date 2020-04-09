# springboard_capstone_00
The subsequent notebooks in this repository are written in python. Each section is outlined below following a pipe ('|'). Operations performed in the section are noted following a hyphen ('-'). Python libraries used are listed at the end of each operation within parenthesis (). 

    | 00_data_wrangling
        | 00_original_wrangle
		     - Acquire data from CMU CS downloaded folders (OS)
			 - Wrangle data from email block text to 19 columns of header fields, body using (RE, concurrent.futures)
			 - Convert to dataframe using python (pandas)
		| 01_first_clean
		     - Remove whitespace, redundancies, non-enron email addresses, forwarded emails (pandas)
			 - Aggregate count of emails sent from each email addresses
		| 02_add_gender
		     - Parse firstname, lastname from email address, 'x-from' columns (RE)
			 - Clean returned name values
			 - Parse firstname for querying gender
			 - Web scrape assumed gender using firstname (requests_html, csv, concurrent.futures)
			 - Generate n=100 sample to evaluate accuracy (pandas)
