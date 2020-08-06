This file, and other associated files, make up my contribution to the final Peer Reviewed Assignment for the Coursera Capstone Project for Applied Data Science Capstone. This was my final module in the IBM Data Science Professional Certificate programme.

For reference I include the original definition for each part of the assignment.

Part 1 [Week 1]
Clearly define a problem or an idea of your choice, where you would need to leverage the Foursquare location data to solve or execute. Remember that data science problems always target an audience and are meant to help a group of stakeholders solve a problem, so make sure that you explicitly describe your audience and why they would care about your problem.

This submission will eventually become your Introduction / Business Problem section in your final report. So I recommend that you push the report (having your Introduction/Business Problem section only for now) to your Github repository and submit a link to it.

Part 2 [Week 1]
Describe the data that you will be using to solve the problem or execute your idea. Remember that you will need to use the Foursquare location data to solve the problem or execute your idea. You can absolutely use other datasets in combination with the Foursquare location data. So make sure that you provide adequate explanation and discussion, with examples, of the data that you will be using, even if it is only Foursquare location data.

This submission will eventually become your Data section in your final report. So I recommend that you push the report (having your Data section) to your Github repository and submit a link to it.

Part 3 [Week 2]
In this week, you will continue working on your capstone project. Please remember by the end of this week, you will need to submit the following:

A full report consisting of all of the following components (15 marks):
Introduction where you discuss the business problem and who would be interested in this project.
Data where you describe the data that will be used to solve the problem and the source of the data.
Methodology section which represents the main component of the report where you discuss and describe any exploratory data analysis that you did, any inferential statistical testing that you performed, and what machine learnings were used and why.
Results section where you discuss the results.
Discussion section where you discuss any observations you noted and any recommendations you can make based on the results.
Conclusion section where you conclude the report.
A link to your Notebook on your Github repository pushed showing your code. (15 marks).
Your choice of a presentation or blogpost. (10 marks)
Section 1: Introduction
In this section I will clearly define the idea of my choosing, where I leverage the Foursquare location data to solve the imagined business opportunity.

Background
There are 100's, maybe even 1000's, of travel sites on the Internet, including FourSquare, that will tell you all about places to go, things to see, restaurants to eat at, bars to drink in, nightclubs to part the night away in and then where to go in the morning to get breakfast and a strong coffee. The problems with these sites is that they are one dimensional. If you want to find out all this information about a city you plan to visit next month, you have to do the hard work. Also, just because a venue is the hottest place to go for a night out does not always mean that the unwitting tourist should just ramble in unprepared. The areas surrounding this new venue might be riddled with crime including muggings, car theft and assault, for example. Approach the venue from any direction other than from the north and you could be putting your life in danger. This is when my idea comes in.

Imagine the following scenario:

You like to plan ahead and always review your options and make your choices about where you will visit and eat up front before you travel.
You are flying to Chicogo for a Data Science Conference.
You arrive in Chicago the day the conference starts but you've managed to convince your boss to delay your return by a few days giving you time to explore.
But you know no one in Chicago to show you around to all the top sites and to bring you to the best restaurants.
Also the last time you went to a conference you were mugged and had you passport. money and credit cards stolen so you're now nervous of going somewhere without first researching the venue and the surrounding area.
The conference is next week and you don't have time to do all the research you'd like.
What do you do ... ?

Project Idea
My idea for the Capstone Project is to show that when driven by venue and location data from FourSquare, backed up with open source crime data, that it is possible to present the cautious and nervous traveller with a list of attractions to visit supplementd with a graphics showing the occurance of crime in the region of the venue.

A high level approach is as follows:

The travellers decides on a city location [in this case Chicago]
The ForeSquare website is scrapped for the top venues in the city
From this list of top venues the list is augmented with additional grographical data
Using this additional geographical data the top nearby restaurents are selects
The historical crime within a predetermined distance of all venues are obtained
A map is presented to the to the traveller showing the selected venues and crime statistics of the area.
The future probability of a crime happening near or around the selected top sites is also presented to the user
Who is this solution targeted at
This solution is targeted at the cautious traveller. The want to see all the main sites of a city that they have never visited before but at the same time, for whatever reaons unknown, they want to be able to do all that they can to make sure that they stay clear of trouble i.e. is it safe to visit this venue and this restaurant at 4:00 pm in the afternoon.

Some examples of envisioned users include:

A single white female traveller
An elderly traveller that has had previous back experiences when travelling
There are many data science aspect of this project including:

Data Acquisition
Data Cleansing
Data Analysis
Machine Learning
Prediction
Now that the conference is over the Data Sceintist can explore Chigago and feel much safer.

Section 2: Data
Data Description
In this section, I will describe the data used to solve the problem as described previously.

As noted below in the Further Development Section, it is possible to attempt quite complex and sophisticated scenarios when approaching this problem. However, given the size of the project and for simplicity only the following scenario will be addressed:

Query the FourSqaure website for the top sites in Chicago
Use the FourSquare API to get supplemental geographical data about the top sites
Use the FourSquare API to get top restaurent recommendations closest to each of the top site
Use open source Chicago Crime data to provide the user with additional crime data
Top Sites from FourSquare Website
Although FourSquare provides a comprehensive API, one of the things that API does not easily support is a mechanism to directly extract the top N sites / venues in a given city. This data, however, is easily available directly from the FourSquare Website. To do this simply go to www.foursquare.com, enter the city of your choise and select Top Picks from I'm Looking For selection field.

Conclusions and Discussions
Although all of the goals of this project were met there is definitely room for further improvement and development as noted below. However, the goals of the project were met and, with some more work, could easily be devleoped into a fully phledged application that could support the cautious traveller in an unknown location.

Of the contributing data the Chicago Crime data is the one where more data would be good to have. Also not every city in the world makes this data freely available so that is a drawback.

FourSquare proved to be a good source of data but frustrating at times. Despite having a Developer account I regularly exceeded my hourly limit locking me out for the day. This is why Pickle was used to store the captured data.

Further Development
The following are suggestions how this project could b efurther developed:

Best time to visit each venue

Suggestions for morning, afternoon, evening and night time

Daily itineraries

Route planning and transportation

Time lapse of the crime in the area of the venue

Favourite dining preferences could be used to choose the restaurants
