# itemlabs

List of core edits.

In meanjs its fine to edit the core module, however I'm trying to avoid this as much as possible to keep upgrades as seamless as I can. Below are things I changed within core or outside of my module that need to be done for the functionality to work properly:

Remove header within core/server/views/layout.server.view.html

Add font markup to core/server/views/layout.server.view.html
  - < link href="https://fonts.googleapis.com/css?family=Orbitron" rel="stylesheet">

Remove 'home' state from core/client/config/core.client.routes.js

Add angucomplete js and css files in config/assets/default.js
  - 'public/lib/angucomplete-alt/dist/angucomplete-alt.min.js'
  - 'public/lib/angucomplete-alt/angucomplete-alt.css'


### I only have my module included in the repo, these are dependencies for the install
Modules to install:
npm install && npm install lolapi && bower install angucomplete-alt --save



Purpose:
Create and compare itemsets on your favorite champions.

Currently working on search. Have champion names pulled from api creating an auto-complete search field.
When a champion is selected, data is returned for that champion from mongo.
