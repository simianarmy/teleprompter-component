teleprompter-component
======================

A small Polymer component for displaying text kind of like a teleprompter.

Getting my hands dirty with Polymer and wanted to create a small component that I could use on one of my projects.

Usage:
```
  <head>
  ...
  <link rel="import" href="simian-teleprompter.html">
  ...
  </head>
  <body>
  ...
  <simian-teleprompter>
  Any text or HTML here
  </simian-teleprompter>`
  ...
  </body>
```
On page load, will display the text in teleprompter style within the tag. 

You can set some attributes on the element to control:
- delay between words: wordDelay - milliseconds
- total display time: displayTime - milliseconds
  
You can trigger a new prompt by changing the words property:
```
  var prompter = document.querySelector('simian-teleprompter');
  prompter.words = 'This will replace the existing text but will be displayed in the same fashion';
```

