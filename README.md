# Development

### Link to Deployed Website
https://bloatedpanda444.github.io/Develop/

### Goal and Value of the Application
The goal of this application is to allow users to track all of the marvel movies they have watched and find out information about them! Marvel now has an impressive 30 movies, so it is a lot to keep track of! This application also can help teach people what phase each movie is in, and allow them to see what movies are the longest and cost the most to make!

### Usability Principles Considered
I consider usability by having all of the filters labeled and displayed on the left, because people usually read left to right so they will think the filters affect the data. I consider memorability by incorporating movie posters that allow the user to know we are talking about movies. I also consider learnability as the buttons have clear text making it obvious what they do.

### Organization of Components
I only use one component, and that is the movie component. This component is a flexbox that is a row that has the movie poster to the left and the movie information on the right. The movie information is simply another flexbox column that has all of its information and buttons displayed.

### How Data is Passed Down Through Components
The component accesses its movie data through props. When the button is pressed on a specific movie component, it has another prop that updates the watched list. This will take the movie components' unique id and then using the unique id add all its information to the watched list. When the watched list is updated so is the total time watched.

### How the User Triggers State Changes
Users trigger state changes when using the filters and selecting they have watched a movie. When a sort is selected, a sort state is changed that is used to sort the dataset. When a filter is selected, the state representing the filter will change to be what we want included in the movie dataset before a filter function is called. Finally, everytime a movie is set as watched or unwatched, the watched movies list changes. This list is used to update the aggregator by summing all movie scores, but also the list is used to tell the movie component to either render saying the movie is watched or not.


