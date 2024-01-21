Pandas_challenge_1

The purpose of the project is to explore, transform, and draw
conclusions about a Client Dataset CSV file.

Explore the Data

Part 1 imports and reads the csv file. I used df.info() to familiarize
myself with the column names, check for null values, and list the data
types of the various columns.

The value_counts()function returned the number of unique items in the
category, subcategory, and client_id columns of the dataset and
was used to determine the most entries for each column.

Transform the Data

Part 2 manipulated the data for further analysis.

Columns were created for subtotal, shipping_price, total_price,
cost, and profit.

To create the shipping_price column. The lambda function was used to
apply a predetermined shipping price to the row based on the result of
multiplying the unit_weight and qty columns.

The total_price column included the subtotal and shipping_price
columns along with a given sales tax of 9.25%.

The other columns are straightforward formulas and are detailed in the
comment sections of the .ipynb file.

Confirm Your Work

The purpose of Part 3 is to verify the calculations and conclusions
drawn in Parts 1 and 2. A dictionary was created using given key: value
pairs. A loop was used to iterate over the dictionary to verify the
information given.

Summarize and Analyze

Part 4 analyzes and draws conclusions based on the work done thus far. A
summary data frame was created for the top clients identified in Part 1
and stored in the top_five_list. Columns were renamed into a more
readable format and were converted to \$1,000,000. The lambda function
was applied to the currency columns to convert them to the given format
of \$x.xxM, with x being the numerical values contained in each
column.
