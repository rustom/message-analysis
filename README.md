# CS 410 Final Project: Text Message Sentiment Analysis

Name: Rustom Ichhaporia

netID: rustomi2

## Project Description

This project is a text message sentiment analysis tool. It parses  your personal text messages from iMessage as well as your text messages from Facebook Messenger, computes the sentiment of the texts, and outputs some interesting plots and statistics related to these sentiments. My video presentation can be [found on YouTube](https://youtu.be/JhGv-ifR-18).

## How to Run

All of the code for this project is contained in the `exploration.ipynb` notebook. To install necessary packages, please run `pip install -r requirements.txt` in the root directory of this project.

### iMessage Data

To query your iMessage data, you must have a computer running MacOS. There is only one manual step required to help you merge the iCloud contact names with the phone numbers, which is explained in the notebook. You shouldn't need to do any extra work to get the code running, unless you need to give the code permission to access your iMessage files in the settings when prompted. 

### Facebook Messenger Data

To query your Facebook Messenger data, you must go to your Facebook account settings and download your data. You can find the instructions for [downloading your Facebook data here](https://www.facebook.com/help/212802592074644). This will be downloadable in the form of multiple folders labeled `your_activity_across_facebook`. I recommend copying these folders into a new folder called `facebook_data` in the same directory as the `exploration.ipynb` notebook. The notebook will handle the rest. Please note that the analysis will not be able to merge the iMessage and Facebook Messenger conversations of contacts who have different display names on the two platforms (they will be treated as separate conversations), but you can fix this manually in notebook if you have contacts with various nicknames. 

## Questions

If you have any questions on how to run the code, or run into any issues, please feel free to open an issue on this repository. Thank you!

## Credit

The sentiment computation is conducted through the [VADER sentiment analysis tool](https://github.com/cjhutto/vaderSentiment) which is specifically trained on social media data. 

A part of the iMessage code for this project was adapted from this [imessage_tools repository](https://github.com/my-other-github-account/imessage_tools) on GitHub. Thank you to the author of that repository for their help. 