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




