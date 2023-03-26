# drunkapi
Some funny questions for party people.

# Usage
Send a GET request to `https://rimezin.github.io/drunkapi/api.json`
Use the array that returns how you see fit. For example:
```js
  const getData = () => {
    const data = fetch('https://rimezin.github.io/drunkapi/api.json')
      .then((res) => {
        console.log('Returned:', res);
        return res;
      })
      .catch((err) => {
        console.error('There was an error:', err));
        return null;
      });
  }
```

# Example Response
```json
    [{
        "question": "If you could live in any fictional world, which one would it be?",
        "category": "fictional worlds"
    },
    {
        "question": "If you had to pick a new first name for yourself, what would it be?",
        "category": "names"
    }]
```
