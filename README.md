# react-movies

A react-based app to store and fetch movies.

Usage:

User can add the movie info to database and fetch the data from the database.

Demo: [http://jordon-chen.github.io/react-movies](http://jordon-chen.github.io/react-movies)

### Installation

```
npm install
npm start
```

Learning: [firebase](https://firebase.google.com/), [useState](https://reactjs.org/docs/hooks-reference.html#usestate), [useEffect](https://reactjs.org/docs/hooks-reference.html#useeffect), [useCallback](https://reactjs.org/docs/hooks-reference.html#usecallback), [fetch()](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch), [async](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function), [await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await), [Try Catch Throw](https://www.w3schools.com/js/js_errors.asp), [response.josn()](https://developer.mozilla.org/en-US/docs/Web/API/Body/json), [JSON.stringify()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify)

Implementation:

- This app consists of 3 components: Movie, MoviesList, AddMovie.
- Set up `firebase` as a backend server.
- Post movie info to the backend server, and get data from backend server through JavaScript built in `fetch API`.
- Use `response.json()` to transform data into objects after fetching the json data.
- Use `JSON.stringify()` to convert a JavaScript object or value to a JSON string before posting data to the backend server.
- When fetching data from backend server, we need to deal with many conditions, such as isLoading, error, no data, got data.
- We can use `useEffect` to fetch data automatically at the beginning of components loaded.
- We can use `useCallback` to save the async fetch function to prevent unnecessary renders.
