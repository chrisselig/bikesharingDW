# bikesharingDW
My first data engineering project, creating a Synapse datawarehouse

## Introduction

Some of the data is from Divvy, a bike sharing program in Chicago, Illinois. This data is anonymous, so Udacity provided some fake rider and account profiles to go along with fake payment data.

A rider can purchase a pass at a kiosk or use a mobile application to unlock a bike at stations around the city and use the bike for a specified amount of time. The bikes can be resturned to the same station or to another station.

## Project Description

Using the Azure tech stack, I wanted to create the following architecture:

![architecture diagram](https://github.com/chrisselig/bikesharingDW/blob/main/80_imgs_for_readme/architecture_image.png)

In Azure, I needed to create a Postgres database and loaded the original data into it.

Then, I performed some [exploratory data analysis (eda)](https://github.com/chrisselig/bikesharingDW/tree/main/02_eda) using python to get a look at the original datasets. 

Next, the PostgreSQL database was linked to Azure blob storage and the data was loaded as external tables to SQL database in Azure Synapse Analytics.

During the transfer to Synapse, the data was transformed from a relational datamodel, to a star schema.

The original model:

![Original Relational Model]()

The newly created star schema:

![Star Schema]()


