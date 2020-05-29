# Capstone Project - The Battle of Neighborhoods
#### Paul Berry 
#### May 2020

### Introduction/ Business Problem

Famous Original Ray's Pizza has five locations in New York City.  A business consortium is looking at establishing a new location in Toronto, and want to find an appropriate location.

They know that the existing locations in New York are appropriate, but don't know anything about Toronto neighbourhoods.  The goal of this project is to identify neighbouthoods in Toronto which are most similar to those in New York City with successful existing locations.

Identifying locations that have similar characteristics will give the new store the best chance of success.


### Data

Using Foursquare data, we well examine the areas around the existing stores in New York City, and neighbourhoods in Toronto, and then use K-means clustering to find neighbourhoods in Toronto that match existing locations in New York City.

The existing stores have the following coordinates:

40.7460427,-74.001496

40.7603983,-73.9841844

40.7632311,-73.981568

40.7642512,-73.9664773

40.7841962,-73.9743688

These locations, as well as locations of Toronto neighbourhoods, as derived in a previous project, will be entered into an API call to Foursquare as follows to obtain information on nearby venues.

https://api.foursquare.com/v2/venues/explore?&client_id={}&client_secret={}&v={}&ll={},{}&radius={}&limit={}

