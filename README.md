# Polymer Paradox - Solution


## How this approach works
- when the delete button is pressed, `example-row` fires an event
- the event is picked up by the index page
- and deletion request is forwarded to the `example-data#delete`
- and `state.page.isDeleting` property of within `example-app-state` is set to the id of the item
- `example-data` method will handle the deletion
- when the request fails, `example-data` will fire a `delete-failed` event
- and that event is picked up by the index page
- and `state.page.isDeleting` state is set to false


## What is this?

Demo application that highlights some open ended questions on who we can use in polymer to handle event/promise communication.

This project is aimed at finding out how other developers would approach this issue.


## Solution & Explanations

- [Api-like Data](https://github.com/filaraujo/polymer-paradox/tree/solution/api-like-data) - Adding methods to data to reduce round trip communication
- [Event+Promise](https://github.com/filaraujo/polymer-paradox/tree/solution/event%2Bpromise) - Combining events and promises
- [Stateful Data](https://github.com/filaraujo/polymer-paradox/tree/solution/stateful-data) - Data that defines the state of the application
