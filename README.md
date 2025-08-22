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

min(),max()  ## finds and returns the smallest or largest number. and you have to use $ to specify what column. and you need to specify the dataset.   EXAMPLE: max(hotel_bookings$lead_time)

mean()  ## Generic function for the (trimmed) arithmetic mean.

na.rm = FALSE ## a logical value indicating whether NA values should be stripped before the computation proceeds.

filter()  ## Use filter() find rows/cases where conditions are true.  EXAMPLE: filter(starwars, hair_color == "none" & eye_color == "black")

##
```{r group and summarize}
hotel_summary <- 
  hotel_bookings %>%
  group_by(hotel) %>%
  summarise(average_lead_time=mean(lead_time),
            min_lead_time=min(lead_time),
            max_lead_time=max(lead_time))
```
##

summarize()  ## The summarize() function is used to summarize a DataFrame or vector into a single value.

ggplot2() ## includes a dataset, geoms(line graph(geom_line), bar graph(geom_bar), scatter plot(geom_point), etc...), and aesthetics such as color, shape, size, etc..., mapping always goes with aes(aesthetic)  EXAMPLE: ggplot(data=penguins)+geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g))

facet_wrap()  ## used to graph each variable individually. At the end of ggplot() --- EXAMPLE: +facet_wrap(~species)

facet_grid()  ## vertical by first variable and horizontal by second --- EXAMPLE +facet_grid(sex~species)

fill=  ## colors bar graphs --- EXAMPLE: ggplot(data = hotel_bookings) +
  geom_bar(mapping = aes(x = distribution_channel,fill=market_segment ))

 theme(axis.text.x = element_text(angle = 45))  ## makes the text a different angle if too cluttered

 labs()  ## to label title or axis. can do title, subtitle, and caption --- EXAMPLE: labs(title= "palmer penguins wing size comparison")

annotate()  ## to add text inside the chart --- EXAMPLE: annotate("text", x=200, y=3500, label="the penguings", color="purple", fontface="bold", size:4.5, angle=25)

ggsave()  ## used to save a chart as png, jpeg, etc... --- EXAMPLE: ggsave("palmer_penguins.PNG")

Rmarkdown  ## Here are some basic formatting options:

  To start a new paragraph, end a line with two spaces

    To apply italics to a word or phrase, place an asterisk at the beginning and at the end of the word or phrase, for example, *italics works*

      To apply bold to a word or phrase, place two asterisks at the beginning and at the end of the word or phrase, for example, **bold is useful**

        To create a header, type a hashtag (#) followed by a space and your text for example: # Getting Started with R Markdown

          When creating headers keep the following in mind:

            Headers will appear in blue

              A single hashtag is the largest header

                The more hashtags you add (up to six), the smaller the header

                  This is a way to save files as html or word document to present
                    
                    Copy code chunks into it such as install.packages(), and library(), and read.csv 
