# UFOs

## Overview
For this project, our goal is to put together a dynamic website with a table that displays our dataset, and filters that visually adjust the table as users refine their search. Specifically, our dataset consists of UFO sightings with various details. With our website we want the user to be able to filter the sightings by date, the city, state, or country where the sighting took place, as well as the shape of the witnessed object.

The tools we are working with include:

* JavaScript, a very popular language in part for its usefulness as a front-end development language with high degrees of functionality and customization
* Basic HTML, Bootstrap, and CSS to build and style the page


## Results 
This is the website the user sees on first "close encounter"...

![UFO sighting homepage](https://github.com/flowersmichael/UFOs/blob/main/static/images/homepage.png)

From here, the user can search on one or multiple criteria. We've included placeholders in each of the filters that display the format the user should follow, for example "1/10/2010" for the date, "roswell" for the city, "nm" for the state, or "circle" for the shape.

![UFO filter](https://github.com/flowersmichael/UFOs/blob/main/static/images/UFO%20filters.png)


## Summary
This design is useful but could be improved. 

One clear drawback is that the table doesn't update "live" as the user inputs data in the filter. By this, I mean that in an improved state, the table would visually adjust as the user types, for example immediately narrowing the data to only states with abbreviations that start with the letter "n" when the user types that character in the filter.

Additionally, as it stands now, not only will the table *not* adjust in "live" fashion, but if the user hits enter after typing the letter "n" then *no* records will be shown. Even if the user inputs a wildcard character after the letter, for example "n*", no records are shown.

Two possibilities for improvement include:
1) allowing for partial data and/or wildcards to generate results ("n" or "n*" would return all states with abbreviations either beginning with "n")
2) live updating as the user enters characters in the filter
