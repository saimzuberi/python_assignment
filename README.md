# Python_assignment
## Unit 2 | Homework Assignment: Automate Your Day Job with Python

### Background
You've made it! It's time to put away the Excel sheet and join the big leagues. Welcome to the world of programming with Python. In this homework assignment, you'll be using the concepts you've learned to complete the required PyBank Python activity, and if you wish to stretch your skills even further, the optional PyRamen Python activity. Both activities present a real-world situation in which your newfound Python skills will come in handy. These activities are far from easy, though, so expect some hard work ahead!

### Actions performed


Created a new GitHub repo called python-assignment. Then, cloned it to my computer.


In my local git repository, created a directory for both of the Python activities. Use folder names that correspond to the activities: PyBank and PyRamen.


In each folder I created main.ipynb and i pushed the changes to GitHub


### PyBank (Required)

In this activity, I created a Python script for analyzing the financial records of the company without using pandas. 

I used the financial dataset in this file: budget_data.csv. 

This dataset was composed of two columns, Date and Profit/Losses. 

The total number of months included in the dataset.
    I calculated this by adding total number of rows in the col - 1 to get the total number of months. 

The net total amount of Profit/Losses over the entire period.
    I calculated this by sum of all rows of the profit/loss column.

The average of the changes in Profit/Losses over the entire period.
    I calculated this by using a while loop and adding differences between each months profit and loss and adding this as a separate column. 


The greatest increase in profits (date and amount) over the entire period.
    In order to perform the maximum increase with data and amount i created a dictionary with differential month and differential amounts and used max function to identify the increase in profits. 

The greatest decrease in losses (date and amount) over the entire period.
    In order to perform the maximum increase with data and amount i used the previously created dictionary with differential month and differential amounts and used min function to identify the increase in profits.

Your resulting analysis should look similar to the following:

### Financial Analysis
----------------------------
Total Months: 86
Total: $38382578
Average  Change: $-2315.12
Greatest Increase in Profits: Feb-2012 ($1926159)
Greatest Decrease in Profits: Sep-2013 ($-2196167)


Your final script should print the analysis to the terminal and export a text file with the results.
    my final output is available in Financial_Ananlysis.txt file which i created using output file.  

## PyRamen (Optional)


### Background
In order to perform analysis of PyRamen business, i have utilized the full capabilities of Pandas which we have learned so far. 

    Imported the 2 files and saved them as data frames 
    I tried to concatecate the files but realized that this will not work as it concatenates the row and and i had to use merge based on index. 
    Once the new data frame was created, i cleaned the data by droping unnessary columns. 
    created new columns with new calculations including
        Revenue = Quantity x Price
        Cost of Goods = Quantity x Cost
        Profit = Revenue - Cost of Goods

    Imported the data in a new data frame and cleaned unnessary columns including price and cost of goods
    The final data was presented in the file Financial_Analysis.txt

FINANCIAL ANALYSIS 
-------------------------------------------------------------------------------------
                                                Quantity   revenue    cog  \
index                                                                       
burnt garlic tonkotsu ramen                         9070  126980.0  54420   
miso crab ramen                                     8890  106680.0  53340   
nagomi shoyu                                        9132  100452.0  45660   
shio ramen                                          9180  100980.0  45900   
soft-shell miso crab ramen                          9130  127820.0  63910   
spicy miso ramen                                    9238  110856.0  46190   
tonkotsu ramen                                      9288  120744.0  55728   
tori paitan ramen                                   9156  119028.0  54936   
truffle butter ramen                                8982  125748.0  62874   
vegetarian curry + king trumpet mushroom ramen      8824  114712.0  61768   
vegetarian spicy miso                               9216  110592.0  46080   

                                                 profit  
index                                                    
burnt garlic tonkotsu ramen                     72560.0  
miso crab ramen                                 53340.0  
nagomi shoyu                                    54792.0  
shio ramen                                      55080.0  
soft-shell miso crab ramen                      63910.0  
spicy miso ramen                                64666.0  
tonkotsu ramen                                  65016.0  
tori paitan ramen                               64092.0  
truffle butter ramen                            62874.0  
vegetarian curry + king trumpet mushroom ramen  52944.0  
vegetarian spicy miso                           64512.0 

