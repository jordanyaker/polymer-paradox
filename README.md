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


## Solution & Explanations

- [Api-like Data](https://github.com/filaraujo/polymer-paradox/tree/solution/api-like-data) - Adding methods to data to reduce round trip communication
- [Event+Promise](https://github.com/filaraujo/polymer-paradox/tree/solution/event%2Bpromise) - Combining events and promises
- [Stateful Data](https://github.com/filaraujo/polymer-paradox/tree/solution/stateful-data) - Data that defines the state of the application
