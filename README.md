# project_1
Group project number 1


This was our first group project. Teams were randomly assigned. 

From a personal standpoint there were struggles because my group did not submit a single line of code to the project. We were given 12 days to complete the project, by day 10 I realized they were not going to have any code to submit and was forced to complete as much functionality as possible from their sections in order for us to present to the class. In the future I would have discussed their lack of work with the teaching staff sooner, however they had given me the impression that they were working on their respective sections. 

From a technical standpoint this was a very fun project, but also difficult in many different ways as this was my first time building an application, first time utilizing each of the 3 API's, and first time using the Materialize CSS library. Each part of the project was both fun and difficult. 

Areas of struggle and the solutions I implemented:
Mapping: I struggled getting the mapping API to work properly because it was telling me that it was taking in too many geolocation points. Eventually I realized that I had a syntax error of an extra bracket wrapping the array when it was getting passed into the map function. Finding this error resolved the mapping error.

Button click: I wanted all functionality to run on as few clicks as possible. In order to do this, I had to call the API's in the background and log specific returned info to Firebase in order to use it later. This proved to be a somewhat slow solution, but ultimately it worked decently well. The end esult is that the user clicks 'find a hike' which takes their address, converts it to a lat/lon and then stores that to Firebase for later use with the mapping. When the lat/lon info is returned from the mapping api it is instantly used to call the hiking API and return hikes to the user that are near their location. 

The second button click is when the user finds a hike they want to do. On this click, the previously stored lat/lon is used as well as the lat/lon from the hike they chose to route directions from their address to the hike trailhead. At this same time local weather and a 5 day forecaset for the specific trail are shown on the screen.

At the time of this writing, the weather is not currently functional as I am trying to get it so that only useful daylight hours are shown in the forecast. This has proven difficuly as I'm under the impression that each set of data needs unique identifiers. Unfortunately I was unable to get this section completed in time for our presentation.

Another area of struggle was the to-do list. As it shows on the screen, all works well with adding and removing items. However, I wanted to build this page to be scalable for future users and allow for logins. I used Firebase to implement this functionality. Currently, I ran out of time to complete the final piece of removing only the specific piece of data from Firebase when the user removes it from the screen.

Final note- I did not have enough time to really dial in the CSS. I would like to improve this at a future time.

Updated: 08/18/19