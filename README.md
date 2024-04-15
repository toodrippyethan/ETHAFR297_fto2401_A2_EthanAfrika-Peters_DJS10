## Project Brief: DJS10 - Asynchrony

#### Objective
Dive into the asynchronous world of React by creating an application that fetches and displays blog posts from an API. You'll practice handling API calls with the Fetch API, managing application state, and gracefully handling errors.

#### Project Description
Your task is to build a React application that makes HTTP GET requests to the JSONPlaceholder API to retrieve a list of dummy blog posts. The application should render the titles and bodies of these posts on the screen. You'll also implement error handling to manage unsuccessful API calls.

- Create a React App that uses the Fetch API to fetch dummy blog posts from this API: https://jsonplaceholder.typicode.com/posts
- Check if the response from the API is "ok", if not throw an error.
- Catch the error by chaining the catch() method to the fetch API per hint below, however save the error in the state instead of console logging it:
  ```js
  fetch('https://api.example.com/data')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));

  ```
- If the API call is succesful, display the title and body of the post in your application as shown below (Don't worry about CSS styling) 
![alt text](<images/blog-posts.png>)
- If the API call was **NOT** succesful, diplay a message to the user notifying them of the error. YOur application should not crash but display a message such a below:
![alt text](<images/error-message.png>)

  ***Hint:** Break the API URL (https://jsonplaceholder.typicode.com/posts) by mistyping it to simulate an error state.
#### Requirements

1. **API Integration**: Use the Fetch API to asynchronously fetch blog posts from `https://jsonplaceholder.typicode.com/posts`. Ensure the API response is checked—if it's not "ok", throw an error.
2. **State Management**: Store the fetched posts in the application's state. Use React hooks like `useState` and `useEffect` to manage state and side effects.
3. **Error Handling**: Implement error handling using the `.catch()` method of the Fetch API. If an error occurs, catch it and store the error message in the state instead of logging it to the console.
4. **UI Rendering**:
   - If the API call is successful, display each post's title and body in your application.
   - If the API call fails, display a user-friendly error message. Ensure your application does not crash.
5. **Testing Error States**: Simulate an error state by modifying the API URL to an incorrect address, and observe if the application correctly handles the error by displaying the appropriate message.

#### Additional Guidelines

- Prioritize clean, readable code. Make sure to separate concerns by keeping your fetching logic and UI rendering distinct.
- Comment your code where necessary to explain why certain decisions were made, especially around error handling.
- No styling is required.


#### Evaluation Criteria

- Correct implementation of asynchronous data fetching.
- Effective state management and error handling.
- Code readability and structure.
- Handling of edge cases and potential errors.







