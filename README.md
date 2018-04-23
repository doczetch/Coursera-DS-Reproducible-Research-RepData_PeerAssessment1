# Peer-graded Assignment: Course Project 1

## By: Cecilia Cruz-Ram, MD DPCOM

### Introduction:

It is now possible to collect a large amount of data about personal movement using activity monitoring devices such as a 
<a href="http://www.fitbit.com/">Fitbit</a>, <a href="http://www.nike.com/us/en_us/c/nikeplus-fuelband">Nike Fuelband<a/>, or 
<a href="https://jawbone.com/up">Jawbone Up<a/>. These type of devices are part of the “quantified self” movement – a 
group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in 
their behavior, or because they are tech geeks. But these data remain under-utilized both because the raw data are 
hard to obtain and there is a lack of statistical methods and software for processing and interpreting the data.

This assignment makes use of data from a personal activity monitoring device. This device collects data at 5 minute intervals 
through out the day. The data consists of two months of data from an anonymous individual collected during the months of 
October and November, 2012 and include the number of steps taken in 5 minute intervals each day.

The data for this assignment can be downloaded from the course web site:

* Dataset: <a href="https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip">Activity monitoring data<a/> [52K]

The variables included in this dataset are:

* <b>steps</b>: Number of steps taking in a 5-minute interval (missing values are coded as 𝙽𝙰)
* <b>date</b>: The date on which the measurement was taken in YYYY-MM-DD format
* <b>interval</b>: Identifier for the 5-minute interval in which measurement was taken

The dataset is stored in a comma-separated-value (CSV) file and there are a total of 17,568 observations in this dataset.

## Assignment:

This assignment will be described in multiple parts. You will need to write a report that answers the questions detailed below. 
Ultimately, you will need to complete the entire assignment in a <b>single R markdown</b> document that can be processed by <b>knitr</b>
and be transformed into an HTML file.

Throughout your report make sure you always include the code that you used to generate the output you present. When writing code 
chunks in the R markdown document, always use 𝚎𝚌𝚑𝚘 = 𝚃𝚁𝚄𝙴 so that someone else will be able to read the code. <b>This assignment 
will be evaluated via peer assessment so it is essential that your peer evaluators be able to review the code for your analysis.</b>

For the plotting aspects of this assignment, feel free to use any plotting system in R (i.e., base, lattice, ggplot2)

Fork/clone the <a href="http://github.com/rdpeng/RepData_PeerAssessment1">GitHub repository created for this assignment<a/>. You 
will submit this assignment by pushing your completed files into your forked repository on GitHub. The assignment submission 
will consist of the URL to your GitHub repository and the SHA-1 commit ID for your repository state.

NOTE: The GitHub repository also contains the dataset for the assignment so you do not have to download the data separately.

Loading and preprocessing the data

Show any code that is needed to

1. Load the data (i.e. 𝚛𝚎𝚊𝚍.𝚌𝚜𝚟())
2. Process/transform the data (if necessary) into a format suitable for your analysis

#### What is mean total number of steps taken per day?

For this part of the assignment, you can ignore the missing values in the dataset.

1. Calculate the total number of steps taken per day
2. If you do not understand the difference between a histogram and a barplot, research the difference between them. 
Make a histogram of the total number of steps taken each day
3. Calculate and report the mean and median of the total number of steps taken per day

#### What is the average daily activity pattern?

1. Make a time series plot (i.e. 𝚝𝚢𝚙𝚎 = "𝚕") of the 5-minute interval (x-axis) and the average number of steps taken, 
averaged across all days (y-axis)
2. Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?

#### Imputing missing values

Note that there are a number of days/intervals where there are missing values (coded as 𝙽𝙰). The presence of missing 
days may introduce bias into some calculations or summaries of the data.

1. Calculate and report the total number of missing values in the dataset (i.e. the total number of rows with 𝙽𝙰s)
2. Devise a strategy for filling in all of the missing values in the dataset. The strategy does not need to be 
sophisticated. For example, you could use the mean/median for that day, or the mean for that 5-minute interval, etc.
3. Create a new dataset that is equal to the original dataset but with the missing data filled in.
4. Make a histogram of the total number of steps taken each day and Calculate and report the <b>mean</b> and <b>median</b> 
total number of steps taken per day. Do these values differ from the estimates from the first part of the assignment? 
What is the impact of imputing missing data on the estimates of the total daily number of steps?

#### Are there differences in activity patterns between weekdays and weekends?

For this part the 𝚠𝚎𝚎𝚔𝚍𝚊𝚢𝚜() function may be of some help here. Use the dataset with the filled-in missing values for this part.

1. Create a new factor variable in the dataset with two levels – “weekday” and “weekend” indicating whether a given 
date is a weekday or weekend day.
2. Make a panel plot containing a time series plot (i.e. 𝚝𝚢𝚙𝚎 = "𝚕") of the 5-minute interval (x-axis) and the average 
number of steps taken, averaged across all weekday days or weekend days (y-axis). See the README file in the GitHub 
repository to see an example of what this plot should look like using simulated data.

### Submitting the Assignment:

To submit the assignment:

1. Commit your completed 𝙿𝙰𝟷_𝚝𝚎𝚖𝚙𝚕𝚊𝚝𝚎.𝚁𝚖𝚍 file to the 𝚖𝚊𝚜𝚝𝚎𝚛 branch of your git repository (you should already be on 
the 𝚖𝚊𝚜𝚝𝚎𝚛 branch unless you created new ones)
2. ommit your PA1_template.md and PA1_template.html files produced by processing your R markdown file with 
knit2html() function in R (from the knitr package) by running the function from the console.
3. If your document has figures included (it should) then they should have been placed in the figure/ directory by 
default (unless you overrided the default). Add and commit the figure/ directory to your git repository so that 
the figures appear in the markdown file when it displays on github.
4. Push your 𝚖𝚊𝚜𝚝𝚎𝚛 branch to GitHub.
5. Submit the URL to your GitHub repository for this assignment on the course web site.

In addition to submitting the URL for your GitHub repository, you will need to submit the 40 character SHA-1 hash 
(as string of numbers from 0-9 and letters from a-f) that identifies the repository commit that contains the 
version of the files you want to submit. You can do this in GitHub by doing the following

1. Going to your GitHub repository web page for this assignment
2. Click on the “?? commits” link where ?? is the number of commits you have in the repository. For example, 
if you made a total of 10 commits to this repository, the link should say “10 commits”.
3. You will see a list of commits that you have made to this repository. The most recent commit is at the 
very top. If this represents the version of the files you want to submit, then just click the “copy to clipboard” 
button on the right hand side that should appear when you hover over the SHA-1 hash. Paste this SHA-1 hash into 
the course web site when you submit your assignment. If you don't want to use the most recent commit, then go 
down and find the commit you want and copy the SHA-1 hash.

A valid submission will look something like (this is just an example!)

![screenshot of chunk table1](table.png)
