# policemisconductnyc
Looking at FiveThirtyEight's data on police misconduct in NYC by year and location.

This is the first semester I’ve worked with newly available on police misconduct settlements, obtained by FiveThirtyEight and the Marshall Project from a set Freedom of Information Act requests. The data from New York City reports 32,632 cases settled between 2010 and 2019, with the incidents themselves spanning 1980-2019.

A group of students working with this data noticed that, unlike other cities who reported data, New York City has included the incident addresses. They asked if it would be possible to map the incidents. This inspired me to learn more about geocoding using the ggmap package in R and make some maps myself. 

To create my maps, I took stratified samples of the data, with 100 random cases per incident year from 2008 to 2018 (the years for which at least 1000 settlements were reported in the data). In the policedata.pdf file you can follow the steps I used to geocode the data. In the lookingatpolicedata.pdf file you can see the maps. The files for all of this are in the geocoding folder.

There is a clear concentration of incidents in a certain neighborhoods in NYC. These reminded a friend of a map he’d seen elsewhere, of gentrification in NYC. After looking around I found the Urban Displacement Project, which studies gentrification in NYC and classifies neighborhoods using census data. They’ve shared their classifications of each census tract in NYC. Using their data, along with data from the census, I updated my previous map. You can see my new map in the policdatawithclass.pdf. 

To make this final map I worked with the FCC API and the data from the Urban Displacement Project. Files are in the census_tracts folder. The map-making process is from the files in the classification folder. In my analysis I also use the US Census API, and to preserve the data I used I have included a copy in the classification folder as well. 
