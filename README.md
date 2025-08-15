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

