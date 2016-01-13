# Polymer Paradox - Solution

## How this approach works

- when the delete button is pressed, `example-row` sets a `deleting` flag
- it will also set up a promise
- and fire an event, passing the item and the promise through the event
- the event is picked up by the index page
- and forwarded to the `example-data#delete`
- `example-data` method will handle the deletion and reject the promise
(passed through the event)
- the promise is caught by `example-row` and then the `deleting` flag is removed.


## What is this?

Demo application that highlights some open ended questions on who we can use in polymer to handle event/promise communication.

This project is aimed at finding out how other developers would approach this issue.
