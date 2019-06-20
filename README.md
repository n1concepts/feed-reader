# Jasmine-Test-FeedReader
- Build testing suites with Jasmine to check business logic of the (Feed Reader) application as well as the event handling and DOM manipulation.
- Created for the Udacity, Front End Web Developer, Nanodegree.

## Table of Contents:
* [Instructions](#instructions)
* [Installation](#installation)
* [FeedReader Functionality](#functionality)
* [Requirements](#requirements)
* [Project Review](#review)
* [Code Dependencies](#dependencies)
* [Contribution](#contribution)
* [Licence](#licence)
* [Acknowledgements](#acknowledgements)

## Instructions:
- Students are given the `RSS feedreader as Udacity startercode`,features included.
- __Goal__ is to __test the RSS feedreader with Jasmine "test-driven development"__ by modifying the feedreader.js file. 
- The Feedreader consists of the following:
1) You can select 4 different feed sources in a menu. 
2) Each time a new source is selected, a new news feed is loaded.
3) hidden menu (by default).
4) The menu displays when click on menu icon with CSS/HTML class.

## Installation:
- __Clone__ this repository or __download__ it as a .zip file.
- Open the `index.html` file in the browser, to open the RSS reader.
- Check the test results on the page bottom.

## FeedReader Functionality: (Test suites and tests)
There are 4 different __test suites__, with 8 separated Jasmine tests:
1: `RSS feeds` definition
2: `Menu` behaviour
3: `Initial Entries` loaded on the page
4: `New Feed selection` load asynchronously, once another source is selected. 

1) Testsuite 1 __`RSS Feeds`__checks, if:
- RSS sources `are defined`, 
- RSS `contain a valid URL`, 
- RSS have `a valid name` (not be empty or undefined)

2) Testsuite 2 __`The menu`__checks, if:
- The Menu `is hidden by default` 
- The Menu `change visibility if icon is clicked`. 
- The Menu is hidden, if the body has the 'menu-hidden' class.  
- The Menu displays if click on menu icon.
- Body's class is available at page load
- Body class is hidden en displayed if the icon is clicked.

3) Testsuite 3 __`Initial Entries`__ checks, if:
- First feed collection (`allFeeds`array) loads within feed container (in HTML). 
- Test starts _AFTER_ this content feed is loaded. 
- The `loadFeed` function is asynchronously called by the `beforeEach` function.
- Test store the feed elements in an array.
- Array elements need to contain at least 1 array element (>0).

4)Testsuite 3 __`New Feed Selection`__ checks, if: 
- The `newFeed` contents a user selects, loads within feed container (in HTML) to replace the `oldFeed`. 
- The content is asynchronously called by the `beforeEach` function to load correctly.
- Both `newFeed` and `oldFeed` contents are stored in a variable.
- Both variables are compared. If their content differ, the HTML content(= Feeds) will be different as well.

## Requirements:
The FeedReader testing need to fullfill the following code criteria [Project Rubric Link](https://review.udacity.com/#!/rubrics/18/view).

## Project Review:
The FeedReader code can be view at [Feed Reader Application](http://niconcepts.com/study/feed-reader).

## Code Dependencies:
- This project is created based on the `Udacity starterscode` from the original [Udacity's Project](https://github.com/udacity/frontend-nanodegree-feedreader).

__Starterscode included:__
- [Google Roboto Font](https://fonts.google.com/specimen/Roboto)
- [Google's JavaScript Loader API](https://www.google.com/jsapi)
- [Handlebars](https://handlebarsjs.com/)
- [Icomoon](https://icomoon.io/)
- [jQuery](https://jquery.com/)

Additional __Javascript Code resources:__
- [Jasmine](https://jasmine.github.io/)


## Contribution:
No pull requests are accepted.

## License:
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgements:
* Thanks to Udacity, (Deb in particular - an awesome mentor!). 