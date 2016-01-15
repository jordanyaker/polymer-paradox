# Polymer Paradox - Solution

## How this approach works

- a publish and subscribe method is added to Polymer.Base
- each data model has a `deleting` state
- the data model subscribes to the `delete` event
- when the delete button is pressed, the `delete` event is publish passing the model
- `example-data` reacts to the publish and sets deleting on that model to true


## What is this?

Demo application that highlights some open ended questions on who we can use in polymer to handle event/promise communication.

This project is aimed at finding out how other developers would approach this issue.


## Solution & Explanations

- [Api-like Data](https://github.com/filaraujo/polymer-paradox/tree/solution/api-like-data) - Adding methods to data to reduce round trip communication
- [Event+Promise](https://github.com/filaraujo/polymer-paradox/tree/solution/event%2Bpromise) - Combining events and promises
- [Stateful Data](https://github.com/filaraujo/polymer-paradox/tree/solution/stateful-data) - Data that defines the state of the application
