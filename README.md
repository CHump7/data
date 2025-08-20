<-c("","")  ## is for naming variables to reference --- put what it currently is to the right and what you want it to be on the left.

ymd()  ## can turn dates into a consistent format. EXAMPLE: mdy("January 20th, 2023")
                                                          # code output:
                                                          # [1] "2023-01-20"

as_tibble()  ## will pull the first 10 rows and all columns that can fit on the screen

head()  ## preview first several rows in spreadsheet like form

glimpse() and "str()"  ## show preview of info like how many rows and columns and the data type 

colnames()  ## shows the column names 

mutate() ##  can both create new variables and overwrite existing ones.

# or ## to write comments

<- data.frame( , )  ## to make spreadsheet, use head() to look at it

data()  ## loads a dataset

view()  ## will bring up the entire spreadsheet

read_csv()  ## read the csv files and makes a tibble


&,|,!  ## AND  OR  NOT 

install.package() and library()  ## will install and load packages such as tidyverse

%>%  ## Provides a mechanism for chaining commands with a new forward-pipe operator, %>%. This operator will forward a value, or the result of an expression, into the next function call/expression

pivot_longer() or  pivot_wider()  ## can mkae the spreadsheet into long or wide format

arrange()  ## can be used to sort by ascending or insert "-" inside the parenthesis before the column name to sort descending

unite()  ## will combine 2 columns or more into 1

clean_names()  ## clean_names() function will automatically make sure that column names are unique and consistent

group_by()  ## takes an existing tbl and converts it into a grouped tbl where operations are performed "by group"

## save as a data frame if you want to keep the manipulated data
