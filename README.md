# Front-End-Notes


Redux Fundamentals:-
--> Action Objects:- Action Objects are simple JS Objects with 'Type', 'Payload' key value pairs.
--> Actions Object Creators :- These are functions that return an action object when called.
--> Reducers :- Reducers are functions that accept State & Action object as arguments and based on the type of object update the Application State.
--> Store :- Store in a central Application state container that manages the state and makes it available throughout the Application.
--> Dispatch, getState :- Dispatch method is called on store and passed an Action object, getState method is called on store to retrieve the current state of the App.
--> Data Flow in Redux-React App :- An event occurs that is handled by an Event Handler, inside Event Hanlder dispatch method on store is called and an action object is passed with it.
The Action object is then received by the store inside which the Reducer function takes the current State and Action Object and updates State accordingly.
