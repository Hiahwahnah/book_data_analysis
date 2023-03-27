# Book Data Analysis

I did this project for the Code Louisville - Data Analysis program. The requirements ask for me to read in data, clean it, analyze it, and interpret it. I chose to use a dataset that featured over 9000 titles and data about those titles according to Goodreads.com. Going into this project the goal was to see what the top genres were based on the ratings from Goodreads.com. I was able to find that and much more about these titles while doing this project.

**Features Included**

### Read Data In

* Use pandas read_csv to bring in the local csv

### Manipulate and Clean Your Data

* Drop unneeded columns using the drop() function
* Use the info() function to gather information and see what else is needed to clean the data
* Use value_counts() function to find duplicate titles
* Use drop_duplicates() function to drop any duplicate titles making sure to keep the first instance of each duplicate so that we don't lose any data
* Use isnull().sum() to see the number of missing values in the dataset
* Use dropna() function to remove the rows that contain null values
* Use split() function to drop the comma and everything after it in the genre column
* Convert the review_count and the rating_count columns to float64 using astype() function
* Rename the "rate" colum to "rating" using the rename() function

### Analyze Your Data

* Use .mean() function to find the average rating of all the titles on a scale of 1-5
* Use .sum() to find the total number of pages in all of the books combined
* Use .nlargest() to create a new dataframe that shows the 5 titles with the highest number of pages
* Use .count() function along with .nlargest() function to show the 5 authors with the most titles
* Use .groupby(), .agg(), and sort_values() functions to identify the top five book genres based on their average rating and total number of reviews, but only considering genres that have at least 100 reviews.

### Visualize Your Data

* Graph 5 authors with the most titles using matplotlib
* Graph top 5 genres based on ratings using matplotlib

### Interpret Your Data and Graphical Output

* The average rating between all titles is 3.96 out of 5. I found this to be higher than I expected.
* There is a total of 2882223 pages combined between all of the titles. 
* The title with the highest number of pages was Harry Potter Boxset (Books #1-7). Not surprising as there are 7 very large titles rolled into 1 title.
* The author with the most titles was Lynsay Sands with 26. This wassurprising because I expected someone like Stephen King.
* Finally the top genre based on ratings was the Urban genre. I expected it to be Science Fiction or Classics but, alas, that was not the case.

**Required Packages**

* python==3.11.1
* pandas==1.5.2
* matplotlib==3.6.3
* see requirements.txt for further information

**Instructions**

To run this project, you will need to install the required packages listed in the requirements.txt file. To do so, run the following command in your terminal:

```
 pip install -r requirements.txt
```

Once the packages are installed, you can run the project by running the book_analysis.ipynb file.

**Guide to Markdown**

For more information about how to use markdown, check out the [GitHub Guide to Mastering Markdown](https://guides.github.com/features/mastering-markdown/).

**Data Description**

The data used in this analysis was collected from Goodreads and contains information about books and their genres. The data was collected using the Goodreads API and includes information such as the book title, author, and genre. The data is in JSON format and is approximately 10,000 records.
