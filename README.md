# flux_redux_mastering
Flux and Redux mastering course




## FLUX

### Concepts


* Actions 
    "Action have a message and payload"
        |-> Actions creator "Helper functions for actions"

* Dispatcher 
    "register listeners and dispatch an action to flux store"

* Flux store
    "Contains the app state, no api to change data, we can have more than one store"
        |-> Reduce store
            "Same as above but implements a reducer feature, flux store have [prev state] [action] [reducer] => [new state]"


### Flux Store Vs ReduceStore

Store | ReduceStore
---   | --- 
can mutate the state        | can't mutate the state
state before and after change can be same obj | new state has to be a copy of the state before the change
logic for responding to actions can be implemneted in any way | logic for responding to actions must be implemented as a reducer
logic does not need to be pure | logic must be pure


## Idempontence / idempotency !?

Given the same inputs, a pure [idempotent] function will always return the same output.

> Pure functions relationated...

> Used in reducers...



## Redux

- Manage app state
- works with any view engine
- Mandatory reducers
- Simgle store and dispatcher
- Dispatcher is part of the store


### Concepts

* State: App data and modify in response to actions 
* Actions: Describe modifications to state
* Reducers: Process actions returns a new state
* Store: Where state is accessed, receives actions


#### Redux and Immutability:
    Once the constructor for and [immutable] obj has completed execution that instance can't be altered.


### Middleware:
    Responde to actions in a unique way
    Use cases: 
        - Debug easily
        - Add support for promises
        - Analytics


