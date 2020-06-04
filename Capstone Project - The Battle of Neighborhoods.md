# Capstone Project - The Battle of Neighborhoods
#### Paul Berry 
#### May 2020

### Introduction/ Business Problem

Famous Original Ray's Pizza has five locations in New York City.  A business consortium is looking at establishing a new location in Toronto, and want to find an appropriate location.

They know that the existing locations in New York are appropriate, but don't know anything about Toronto neighbourhoods.  The goal of this project is to identify neighbouthoods in Toronto which are most similar to those in New York City with successful existing locations.

Identifying locations that have similar characteristics will give the new store the best chance of success.


### Data

Using Foursquare data, we well examine the areas around the existing stores in New York City, and neighbourhoods in Toronto, and then use K-means clustering to find neighbourhoods in Toronto that match existing locations in New York City.

There are five existing stores, we have codes for the existing stores, their relative financial performance, and coordinates:

Existing Store A, Below Average, 40.7460427,-74.001496

Existing Store B, Above Average, 40.7603983,-73.9841844

Existing Store C, Average, 40.7632311,-73.981568

Existing Store D, Average, 40.7642512,-73.9664773

Existing Store E, Average, 40.7841962,-73.9743688

These locations, as well as locations of Toronto neighbourhoods, as derived in a previous project, will be entered into an API call to Foursquare as follows to obtain information on nearby venues.

https://api.foursquare.com/v2/venues/explore?&client_id={}&client_secret={}&v={}&ll={},{}&radius={}&limit={}

This will provide information of nearby venues, which will be aggregated by category (pizza store, asian market, etc.) for analysis.

Ideally, as well as finding a location that is similar to existing stores, we will be able to identify which of these locations most closely matches the best performing store.
