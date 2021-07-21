# Understanding Questions:
1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code excutes for each step.
* The user presses the 1 button.
* The button has an onClick function, so the code looks at this function
* The function tells us to dispatch our addOne() function which is located in the actions directory
* addOne() returns the type: ADD_ONE which the reducer takes in as an argument
* Because the case is ADD_ONE, the reducer returns a spread of the current state, but updates the total to the current state + 1
* TotalDisplay shows the total plus 1.
