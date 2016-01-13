# Polymer Paradox - Solution

## How this approach works
- data.splices change handler is added to `example-data` so whenever the number of items changes
the component will attach a `delete` method to that data object
- when the delete button is pressed, `example-row` sets a `deleting` flag and
calls `this.model.delete` method (previously exposed)
- `example-data#delete` method will handle the deletion and returns the promise
- the promise is caught by `example-row` and then the `deleting` flag is removed.


## What is this?

Demo application that highlights some open ended questions on who we can use in polymer to handle event/promise communication.

This project is aimed at finding out how other developers would approach this issue.
