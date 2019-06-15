# LIRI Bot App

* [Video Demo](https://drive.google.com/file/d/1TDNk54vCh87K3IkN8FGgPGnatNGpx2F8/view)

### How to use this app
liri.js can take in one of the following commands:
* concert-this
* spotify-this-song
* movie-this
* do-what-it-says

### What Each Command Should Do

#### Example 1) concert-this
* This will search the Bands in Town Artist Events API for an artist and render the following information about each event to the terminal:
  * Name of the venue
  * Venue location
  * Date of the Event (use moment to format this as "MM/DD/YYYY")

    node liri.js concert-this <artist/band name here>

![concert-this](/images/concert-this.png)

#### Example 2) spotify-this-song
* This will show the following information about the song in your terminal/bash window
  * Artist(s)
  * The song's name
  * A preview link of the song from Spotify
  * The album that the song is from

    node liri.js spotify-this-song '<song name here>'

![spotify-this](/images/spotify-this.png)

* If no song is provided then your program will default to "The Sign" by Ace of Base.

![spotify-this-song](/images/spotify-this-song.png)

#### Example 3) movie-this
* This will output the following information to your terminal/bash window:
  * Title of the movie
  * Year the movie came out
  * IMDB Rating of the movie
  * Rotten Tomatoes Rating of the movie
  * Country where the movie was produced
  * Language of the movie
  * Plot of the movie
  * Actors in the movie

    node liri.js movie-this '<movie name here>'

![movie-this](/images/movie-this.png)

* If the user doesn't type a movie in, the program will output data for the movie 'Mr. Nobody.'

![movie-this-none](/images/movie-this-none.png)
 
#### Example 4) do-what-it-says
* Using the fs Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.
  * It should run spotify-this-song for "I Want it That Way," as follows the text in random.txt
  * Edit the text in random.txt to test out the feature for movie-this and concert-this

    node liri.js do-what-it-says

![do-what-it-says](/images/do-what-it-says.png)


### Overview

In this assignment, you will make LIRI. LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a Language Interpretation and Recognition Interface. LIRI will be a command line node app that takes in parameters and gives you back data.

### Before You Begin
* LIRI will search Spotify for songs, Bands in Town for concerts, and OMDB for movies.
* Make a new GitHub repository called liri-node-app and clone it to your computer.
* To retrieve the data that will power this app, you'll need to send requests using the axios package to the Bands in Town, Spotify and OMDB APIs. You'll find these Node packages crucial for your assignment.

* [Node-Spotify-API](https://www.npmjs.com/package/node-spotify-api)
* Axios
  * You'll use Axios to grab data from the OMDB API and the Bands In Town API
  * http://www.omdbapi.com/
  * http://www.artists.bandsintown.com/bandsintown-api
* [Moment](https://www.npmjs.com/package/moment)
* [DotEnv](https://www.npmjs.com/package/dotenv)

### Submission Guide

Create and use a standard GitHub repository. As this is a CLI App, it cannot be deployed to GitHub pages or Heroku. This time you'll need to include screenshots, a GIF, and/or a video showing us that you have the app working with no bugs. You can include these screenshots/GIFs or a link to a video in a README.md file.

In order to meet the Employer Competitive standards and be ready to show your application to employers, the README.md file should meet the following criteria:
* Clearly state the problem the app is trying to solve (i.e. what is it doing and why)
* Give a high-level overview of how the app is organized
* Give start-to-finish instructions on how to run the app
* Include screenshots, gifs or videos of the app functioning
* Contain a link to a deployed version of the app
* Clearly list the technologies used in the app
* State your role in the app development

Because screenshots (and well-written READMEs) are extremely important in the context of GitHub, this will be part of the grading in this assignment.

If you haven't written a markdown file yet, click here for a rundown, or just take a look at the raw file of these instructions.
* https://guides.github.com/features/mastering-markdown/
