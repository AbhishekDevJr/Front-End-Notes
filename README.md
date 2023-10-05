# Front-End-Notes


Redux Fundamentals:-<br><br>
--> Action Objects:- Action Objects are simple JS Objects with 'Type', 'Payload' key value pairs.<br><br>
--> Actions Object Creators :- These are functions that return an action object when called.<br><br>
--> Reducers :- Reducers are functions that accept State & Action object as arguments and based on the type of object update the Application State.<br><br>
--> Store :- Store in a central Application state container that manages the state and makes it available throughout the Application.<br><br>
--> Dispatch, getState :- Dispatch method is called on store and passed an Action object, getState method is called on store to retrieve the current state of the App.<br><br>
--> Data Flow in Redux-React App :- An event occurs that is handled by an Event Handler, inside Event Hanlder dispatch method on store is called and an action object is passed with it.<br><br>
The Action object is then received by the store inside which the Reducer function takes the current State and Action Object and updates State accordingly.<br><br>


React Advanced Concepts:-<br><br>
--> 1. React Code should make WebApps highly Accessible/Accessiblity should be great.
--> 2. Lazy Loading:- Using Lazy Loading to only Render Components when they are required on the UI.
            const MyComp = lazy(() => import('./MyComp.js'));
            function ParentComp(){
              return(
                <Suspense fallback = {<Loading />}>
                  <MyComp />
                </Suspense>
              );
            }

  Suspense Boundary provides a FallBack UI during rendering of a component when Code Splitting
--> 3. ErrorBoundary :- Can be used to fallback to a UI Component that gets rendered when some error occurs on the FrontEnd Side of the Code.
