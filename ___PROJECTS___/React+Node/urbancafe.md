# urbancafe

* find nearby cafe's with a social component
* mobile-first
* v1 in React, Node and Express, testing, ci-cd
* v2 migration to Next

<hr>
<br>

[mvp features](#mvp)  |  [stretch features ](#stretch)  |  [techstack](#tech)  |  [api's](#apis)  |  [task list](#tasks)  |  [approach notes](#approach)

<br>
<hr>

<h2 id="mvp">

  ## MVP features
</h2>

<hr>

    ui
      [] 3 pages: title, search, detail
      [] client side routing
      [] title page = splash with button entry (v2 conversion to login)
      [] search bar w. search by zip logic
      [] results list with click through to detail view
      [] create a detail page displaying returned data
        [] install thoughtboard variation for member reviews and comments => commentboard
    api
      [] geocoder places
        [] obtain google lat-long object by zip code
        [] GET nearby businesses(lat-long object)
        [] GET individual business

<br>
<hr>

<h2 id="stretch">
  
  ## Stretch Features
</h2>
<hr>
<br>

> auth
> fav tagging
> social component: utilize thoughtboard with login
> ecommerce: coffee + brew lifestyle selections
> add filtering
> add mapView of search results
> develop/implement a suggestion algorithm
> add testing

    [] init userbase API (from thoughtboard - add favs)
    [] init cafebase API (newBuild - init with data from google business... piggyback with internal commenting, reviewbase, etc )
      [] CRUD internal cafebase (persists cafe profile on first user  interaction - i.e. comment, like, tagged)
      [] 

> byobrews: checkbox to include waterfronts, park spaces, other public areas
> deploy vanilla react, node, express app
> migrate to Next


<br>
<hr>
<h2 id="tech">

  ## Tech Stack
</h2>
<hr>
<br>

- react
- react-router-dom

- node
- nodemon
- express
- mongoose


<br>
<hr>
<h2 id="apis">

  ## APIs
</h2>
<hr>
<br>

- geocoder.goecode (lat-long object)
- places.searchNearby(lat-long, dist)
- place_id // [] review this

<br>
<hr>
<h2 id="tasks">

  ## Tasklist
</h2>
<hr>
<br>

    [] build search component
    [] build list components
    [] business
      [] model
      [] api
      [] condensed/list card
      [] exapnded modal/page

    [] search functionality
    [] place id to its own variable
    [] ?(start from detailed and work outwards w/ data)
    [] title block
    [] details block
    [] reviews list
    [] review form
    [] photos fetch
    [] wire data into components
    [] add mobile responsiveness

    [] implement context || redux
      [] dark / light mode
      [] user role / profile
    
    [] init a server
      [] install CRUD db service 
      [] install geocoder service
      [] install auth<>userbase service
      [] install userProfileDB service
      [] install businessProfileDB service (mvp: [comments, likes, self-contained])


<hr>

    [] review and refine init scope 
    [] add typescript handling
    [] framework social component v1 
      [] install thoughtboard API
        [] inject auth
        [] inject ci/cd
        [] inject testing
      [] ideate and build out thoughtboard 
        [] iterate with reply to thought feature
        [] add likes/rating system
        [] v1 main ui: refactor giphy gallery into display board
    [] implement graphql??

<hr>

    [] NextMigration
      [] rebuild+finetune API in Node Mastery
        [] typeScript conversion
        [] build in TDD (use testing framework from thoughtboard)
      [] targeted knowledge grab
        [] concurrent rendering
        [] ssg-ssr-cdn deployment
        [] ci-cd pipeline in Next/Vercel
      [] gut reno frontend to layout with standard styling
        [] build layout (snag from astaiglesia)
        [] implement a header_minimal_thin
        [] implement a sidebar_minimal_thin, extends from thin
        [] implement a footer_minimal_thin
        [] rework the main
          [] ideate 3 concepts
          [] build one 
        [] install fira code font
        [] add mobile responsiveness 
        [] iterate for accessibility

 
<br>
<hr> 
<a id="approach">

  ## Approach Notes
</a>
<hr> 
<br>

  - flexbox pages w router
  - review schemas
    - define endpoints
    - create seed data

  - search page inputs ( zip + distance ) ----> geocode for lat + long at a specific point -----> Places API to search nearby businesses, filtering for restaurants, cafes
    - search bar
    
  - map fetch data to a list component
    -  clickable list items
      - on clickthru (or prefetch in next) GET request to places API for business details by id
      - redirect to product detail page 
  - on detail page/modal/view : 
    - post reviews