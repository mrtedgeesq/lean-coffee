Resources
https://codelabs.developers.google.com/codelabs/polymer-firebase-pwa/

Steps

Project Tools
npm install -g bower
npm install -g firebase-Tools
firebase version //Check the version is >= 3.0.0
firebase login //Log in to firebase

Setup the project

firebase init //Use default settings apart from the re-write urls to index.html, whihc should be no
polymer init //Choose polymer-starter-kit

Check what we've got

polymer serve --open //Uses dev server to show the sample app

Create our new element

create a file src/lean-coffee.html

setup as new element:

<link rel="import" href="../bower_components/polymer/polymer.html">
<dom-module id="coffee-app">
  <template>
    <style>
    :host {
        display: block;
    }
    </style>
    Hello
  </template>
  <script>
    Polymer({
      is: 'coffee-app',
      properties: {

      },
    });
  </script>
</dom-module>

add to index.html + change import
<coffee-app></coffee-app>

demo again

Add ui

Add paper-elements and iron-icons
bower install --save iron-icons
bower install --save paper-elements

coffee-app.html
<link rel="import" href="../bower_components/paper-elements/paper-elements.html">
<link rel="import" href="../bower_components/iron-icons/iron-icons.html">

//create topic-editor.html
//add boilerplate
//add controls + code 
//add layout

//coffee-app
//handle save event


//DON'T forget to set <body class="fullbleed vertical layout"> and <coffee-app class="flex"> in index.htmls