# Frontend Exercise
In this exercise you will have build a responsive site navigation with a simple session management in php

## Here are the guidelines for this exercise
* It must be developed using only css (you can use less, sass...), javascript, HTML 5 & PHP.
* No frameworks or libraries (e.g. Bootstrap, jQuery, Angular, React, CodeIgniter, Laravel...).
* Nav menu must be responsive.
* Items in nav menu should be load using javascript getting the json object in **"resources/data/menu.js"** via http request.
* An user can log in and log out using php sessions.

### Nice to haves
* Object-oriented programming (OOP)
* The code must be clear and legible.
* Documentation.

### Resources
You can find in **"resources"** folder all what you need to complete this test:
* **asssets**: All images what you need include in responsive site navigation.
* **data**: A json with nav menu items to be loaded via javascript.
* **typography**: Site fonts.
* **wireframes**: These will guide how the site should look like.


## Design Specifications
The site will have two main states, Desktop and Mobile; these will be shown in the folder **resources/wireframes**, any detail about measurements, colors or actions that no be especificate in wireframes or below, should be asumed.

##### General
* The background must be fixed in center of screen, cover all content, and it should not be deformed on screen resize.
* The background should have a slight translucent mask, that allow visualize better all texts.
* On hover, active or focus, all buttons or links in nav menu will change clearly his state.
* On click, if item menu contains a URL, the browser will navigate to a new page.
* Facebook & linkedIn buttons don't have events associated.
* If login form have errors, his fields state should change clearly .
* On click in nav item with sub-menu, sub-menu will appear below.
* Only one sub-menu will appear at time, if other sub-menu is active, should be hide.
* When a submenu is displayed or hidden, arrow icon should rotate with ease animation 180 degrees.

##### Desktop (> 768px)
* The nav menu will display as a horizontal nav. Nav items will display sub-nav items when clicked. No hamburger will be shown.
* If a sub-menu is active, on click outside should be hidden.

#### Mobile (<=767px)
* Nav menu will disappear and hamburger icon will display in the top-right of the page; clicking the hamburguer will cause appear a responsive nav menu.
* When responsive nav menu appear:
    * The menu should “pull” from right to left with ease animation all content.
    * Translucent mask appears over content.
    * On click in translucent mask or close button in responsive menu, should "pull" from left to right with ease animation all content, and the translucent mask should be hidden.
* Scroll bar should appear on responsive menu only when menu items exceed the height of the screen.


## PHP Tasks
* On submit login form, a php object will validate the fields values, if values are consistent (e.g the name is alphabet and password has caracters) then init a new php session and redirect to **internal view (take a look in wireframes)** in another case return to **home page view** with form errors.
* If you have an active session the index view should load **internal view**, in another case should load **home page view**.
