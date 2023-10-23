# 19 Progressive Web Applications (PWA): Text Editor (Teditor)

## My Task

I set up a new project directory and initializing it with npm.
I installed the necessary dependencies, including idb and any other libraries I need.
I created the Text Editor UI:

I designed the user interface for my text editor using HTML and CSS.
I implemented a textarea or contenteditable element for text input.
Implement IndexedDB:

I used the idb package to create and manage an IndexedDB database.
I defined a schema for my database, specifying the structure of my data.
Add Data Persistence:

I implemented methods to save, update, and retrieve text data from the IndexedDB database.
I handled online and offline scenarios by checking the browser's online status.
Offline Support:

I implemented a service worker to cache my application and enable offline access.
I used the service worker to handle offline data synchronization.

## User Story

```md
AS A developer
I wanted to create notes or code snippets with or without an internet connection
so that I can reliably retrieve them for later use
```

## Acceptance Criteria

```md
GIVEN a text editor web application
WHEN I open my application in my editor
THEN I should see a client server folder structure
WHEN I run `npm run start` from the root directory
THEN I find that my application should start up the backend and serve the client
WHEN I run the text editor application from my terminal
THEN I find that my JavaScript files have been bundled using webpack
WHEN I run my webpack plugins
THEN I find that I have a generated HTML file, service worker, and a manifest file
WHEN I use next-gen JavaScript in my application
THEN I find that the text editor still functions in the browser without errors
WHEN I open the text editor
THEN I find that IndexedDB has immediately created a database storage
WHEN I enter content and subsequently click off of the DOM window
THEN I find that the content in the text editor has been saved with IndexedDB
WHEN I reopen the text editor after closing it
THEN I find that the content in the text editor has been retrieved from our IndexedDB
WHEN I click on the Install button
THEN I download my web application as an icon on my desktop
WHEN I load my web application
THEN I should have a registered service worker using workbox
WHEN I register a service worker
THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets
WHEN I deploy to Heroku
THEN I should have proper build scripts for a webpack application
```

## My site

### Technical Acceptance Criteria: 40%

* Satisfies all of the above acceptance criteria plus the following:

  * Uses IndexedDB to create an object store and includes both GET and PUT methods

  * The application works without an internet connection

  * Automatically saves content inside the text editor when the DOM window is unfocused

  * Bundled with webpack

  * Create a service worker with workbox that Caches static assets

  * The application should use babel in order to use async / await

  * Application must have a generated `manifest.json` using the `WebpackPwaManifest` plug-in

  * Can be installed as a Progressive Web Application


## Screenshots
![initial](https://github.com/eecmanny/Teditor/assets/130661353/5b274425-e79e-4d93-ac6c-60a2ceaefac7)

![typed](https://github.com/eecmanny/Teditor/assets/130661353/983a8f93-56a2-47fb-b862-fb18e257718d)

![download](https://github.com/eecmanny/Teditor/assets/130661353/de30aaa9-c9a1-4306-aa6f-3419e88c4214)

![offline app](https://github.com/eecmanny/Teditor/assets/130661353/eb0f9c29-5129-4776-b9fa-4511d232fab8)



## Review

https://stormy-sea-35497-abd9bb5b28ec.herokuapp.com/

https://github.com/eecmanny/Teditor

- - -
© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
