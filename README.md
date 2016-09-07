# update_stockmarket
Update Stockmarket Card Day 5

Create a Block type called   “Stock Exchange Rate Card” 
	Company Name 
	Symbol 
	Last Price 
	Change 

Create Instances of the block with different sets of values and place them at different spots on the site. Example values ­   (Apple, AAPL), (Bank of America,BAC), (Transocean, RIG), (Freeport, FCX)  .  (Ignore the Last Price and Change fields’ values, we will be dealing them in next step). 

Below API can be used to retrieve Last Price and Change values 
http://dev.markitondemand.com/MODApis/Api/v2/Quote/jsonp?symbol=  BAC  &
callback=myFunction 

Build a custom module, which on Cron run,  

Iterates through each instance of blocks of type “Stock Exchange Price Card” 

For each block, take the symbol value and call the API to retrieve the Last Price and Change values 
Update the block field values programmatically with the values of Last Price and Change retrieved from the API and save the block 
