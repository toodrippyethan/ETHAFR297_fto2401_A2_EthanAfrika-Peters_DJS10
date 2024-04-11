# DJS09 - Asychrony Challenge

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


