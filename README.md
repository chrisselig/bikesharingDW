# bikesharingDW
My first data engineering project, creating a Synapse datawarehouse

## Introduction

Some of the data is from Divvy, a bike sharing program in Chicago, Illinois. This data is anonymous, so Udacity provided some fake rider and account profiles to go along with fake payment data.

A rider can purchase a pass at a kiosk or use a mobile application to unlock a bike at stations around the city and use the bike for a specified amount of time. The bikes can be resturned to the same station or to another station.

## Project Description

Using the Azure tech stack, I wanted to create the following architecture:

![architecture diagram](https://github.com/chrisselig/bikesharingDW/blob/main/80_imgs_for_readme/architecture_image.png)

In Azure, I needed to create a Postgres database and loaded the original data into it.

I performed some [exploratory data analysis (eda)]() using python to get a look at the original datasets. 

I then created a Synapse workspace and created a datawarehouse. I then created a pipeline to copy the data from the Postgres database to the datawarehouse, but along the way I transformed it into a star schema. The data models are shown below.

***** Insert image here *****
