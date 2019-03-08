### 1.  Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?

Mutable Array methods: 
- `.filter()`
- `.map()`
- `.assign()`

For creating a new object using an existing object as a prototype we use `Object.create()`

### 2.  Describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

#### Actions

Actions send data from your application to your store. 

#### Reducers

Reducers specify how application state changes in response to actions sent to the store.

#### Store

Contains redux state for the application.

### 3.  What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application state is a sort of global state, held in stores.
Component state is contained inside a component. Component state is used for epheremral state information or as an intermediary to be put into application state.

### 4.  What is middleware?

Middleware is code you put between the framework.

### 5.  Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

Redux Thunk is middleware for Redux. Makes it a lot easier to do async requests, promises, etc using the thunk pattern. We can have action-creators return functions with direct access to the dispatch method.

### 6.  Which `react-redux` method links up our `components` with our `redux store`?

.connect()