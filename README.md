# TechWeek Website #
This repository contains the Techweek website for the year 2015

---

The website was written to have the Google Material Design look and feel. MaterializeCSS was used to speed up the process.  

## How it works ##

The events.json contains a JSON object containing all events (duh). The schema was just made up on the spot and seemed most appropiate. `js/main.js` is it main JavaScript file that is responsible for loading the content.
It uses jQuery (because I don't like XHR) to load the events from the JSON. It then gets populated to appropriate tables.  

The `main.js` file is also responsible for displaying the countdown and loading the video feed. Also, it changes colour of the header and individual days, depending on the amount of times you have visited the page.

---

## Notes ##
* When running the files locally, run it using a web server or you will have problems with Same-origin policy (because apparently different files with file:/// are on different protocols or something like that...).
A simple solution is to run a simple Python webserver (which I used for development) inside your current work directory:
> `python -m SimpleHTTPServer`

* If you break it, its not my fault. It works on my machine
