# gol-apps-tech-test

GOL Apps Coding Challenge

Introduction
You have been asked to kick off a new groceries app, initially consisting of two screens

The first screen will simply display a list of the products (fetched from a server - see below) and the prices
When the user taps on a product, the application then shows a second screen containing the product and the price again, as well as the description paragraph
The designer has asked that the typography be as follows:

Components	Color	Font
name	#000000	bold, 20sp, system font (roboto)
price	#3d3d3d	normal, 12sp, system font (roboto)
description	#000000	normal, 14sp, system font (roboto)

The user should also be able to trigger a reload of the data from the server.

API
The list of items is available at https://github.com/sainsburys-tech/gol-apps-tech-test/master/groceries.json

curl -G https://github.com/sainsburys-tech/gol-apps-tech-test/master/groceries.json

Analytics
The product manager needs you to record interaction and network events as people use the app. This can be done by issuing “fire and forget” GET requests to https://github.com/sainsburys-tech/gol-apps-tech-test/master/analytics

Event specific query parameters should be appended to the URL as follows:

event=load – any network request
time=xxx - the time (in ms) for the network request to complete
event=display – whenever a screen is shown 
screen=XXX - an identifier for the screen that was shown (the product list or the product description page)
curl -G https://github.com/sainsburys-tech/gol-apps-tech-test/master/analytics?event=load&time=100
curl -G https://github.com/sainsburys-tech/gol-apps-tech-test/master/analytics?event=display&screen=XXX

Considerations
This is an opportunity to demonstrate your understanding of what modern Android app development looks like. We believe that good contributors to achieving this are typically code readability, unit testing, separation of concerns, the open/closed principle, error handling, and an intuitive, responsive, user interface.

Please write the app in Kotlin for Android or Swift for iOS.

Remember we are looking for a demonstration of your skills - not perfection. A comment about what you would do next might be better than squeezing in everything, but not doing anything to your usual standard.
