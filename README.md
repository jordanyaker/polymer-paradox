# Polymer Paradox - Solution

## How this approach works

- each data model has a `deleting` state
- when the delete button is pressed and event is fired
- the event is picked up by the index page
- and forwarded to the `example-data#delete`
- `example-data` will set `deleting` on that model to true
- `example-data` method will handle the deletion and set the `deleting` flag to flag


## What is this?

Demo application that highlights some open ended questions on who we can use in polymer to handle event/promise communication.

This project is aimed at finding out how other developers would approach this issue.
