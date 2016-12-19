Wayne State Style Guide
=========

Wayne State University global header/footer and other general styles. Build on [Zurb Foundation 6](http://foundation.zurb.com/).

## Desktop
![desktop](http://waynestate.github.io/styleguide/images/header-fd5-desktop.png "Header on the desktop")

## Tablet
![tablet](http://waynestate.github.io/styleguide/images/header-fd5-tablet.png "Header on the tablet")

## Mobile
![mobile](http://waynestate.github.io/styleguide/images/header-fd5-mobile.png "Header on the mobile")

## University Mission
1. Add Fjalla One to the master layout header <pre>&lt;link href="https://fonts.googleapis.com/css?family=Fjalla+One" rel="stylesheet"&gt;</pre>
2. Include mission.tpl or mission.blade.php in the master layout
    * Blade <pre>@include('partials.mission')</pre>
    * Smarty <pre>{include "partials/mission.tpl"}</pre>
3. Edit the gulp file to move the mission template AND the background image from node modules into the project
    * Search for 'styleguide' and add a line to move 'mission-bg.jpg' and 'mission.blade.php' or 'mission.tpl'
