# Wrangle-and-Analyze-Data

the goal is to wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. The Twitter archive is great, but it only contains very basic tweet information. Additional gathering, then assessing and cleaning is required for "Wow!"-worthy analyses and visualizations.

## Data description 
In this project, I will work on the following three datasets 

Enhanced Twitter Archive :
- The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, I have filtered for tweets with ratings only (there are 2356).
![Screenshot 2022-10-19 at 12 58 13](https://user-images.githubusercontent.com/74813723/196673122-797ba39a-9813-4499-b446-f24939810f38.png)

I extracted this data programmatically, but I didn't do a very good job. The ratings probably aren't all correct. Same goes for the dog names and probably dog stages (see below for more information on these) too. You'll need to assess and clean these columns if you want to use them for analysis and visualization. ![Screenshot 2022-10-19 at 12 57 23](https://user-images.githubusercontent.com/74813723/196674100-023b1b6d-3484-42fd-8818-b70c81941ca2.png)


## Additional Data via the Twitter API

- Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered by anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent tweets, at least. But you, because you have the WeRateDogs Twitter archive and specifically the tweet IDs within it, can gather this data for all 5000+. And guess what? You're going to query Twitter's API to gather this valuable data.

## Image Predictions File

- One more cool thing: I ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs*. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).
![Screenshot 2022-10-19 at 12 51 53](https://user-images.githubusercontent.com/74813723/196672158-f423d358-cb25-44a3-994a-b5b0792cbce9.png)



## Project Steps Overview
Your tasks in this project are as follows:

Step 1: Gathering data

Step 2: Assessing data

Step 3: Cleaning data

Step 4: Storing data

Step 5: Analyzing, and visualizing data

Step 6: Reporting

# commentaires

wrangle_act.ipynb: code for gathering, assessing, cleaning, analyzing, and visualizing data
wrangle_report.pdf or wrangle_report.html: documentation for data wrangling steps: gather, assess, and clean
act_report.pdf or act_report.html: documentation of analysis and insights into final data
twitter_archive_enhanced.csv: file as given
image_predictions.tsv: file downloaded programmatically
tweet_json.txt: file constructed via API
twitter_archive_master.csv: combined and cleaned data


## Results
Pease see my notebook for all analyse (wrangle_act.ipynb)

## Conclusions
Even a dog breed is very popular for the most tweeters don’t mean is the most favorited or retweeted by other users. The selection of a preferable dog breed is up to others criteria, which need a depth analysis with more variables. In other side, the increase of tweets number do not mean the increase of the visitors reaction for the tweeted dog breed. It can be explained by confusion of visitors for choosing the preferable dog breed when the number of tweets increase or the rate of dog breed tweets increasing is greater than the rate of favorite and retweet average increasing. Finally, the originality of humorist rating is what almost visitors prefer for rating the dogs, which mean is the asset of this twitter account.
