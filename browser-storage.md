### Browser storage cheat sheet

Browser storage is an essential feature for web developers, allowing them to store data locally on a user's browser to enhance the functionality and user experience of web applications. The following cheat sheet provides an overview of the different types of browser storage, their limitations, and how to use them effectively.

### Type of Storage

| Storage Type | Storage Limit | Expiration | Typical Use Cases |
| --- | --- | --- | --- |
| Cookies | 4 kilobytes | Can set an expiration | Storing user login information, tracking user preferences and behavior, storing session IDs for server-side session management, saving the state of a web application between page refreshes or browser restarts |
| Local Storage | 10 megabytes | Data never expires | Saving user preferences (e.g. color scheme), caching data for offline use, storing form data to be auto-filled, saving the state of a web application between page refreshes or browser restarts |
| Session Storage | 5 megabytes | Expires when the user closes the browser | Storing temporary data for a single session, storing temporary data for a single tab, storing data for an authenticated user session |

### Methods

| Method | Description |
| --- | --- |
| `localStorage.setItem(key, value)` | Sets a key-value pair in local storage |
| `localStorage.getItem(key)` | Retrieves a value from local storage with the given key |
| `localStorage.removeItem(key)` | Removes an item from local storage with the given key |
| `localStorage.clear()` | Removes all items from local storage |
| `localStorage.length` | Returns the number of items in local storage |
| `sessionStorage.setItem(key, value)` | Sets a key-value pair in session storage |
| `sessionStorage.getItem(key)` | Retrieves a value from session storage with the given key |
| `sessionStorage.removeItem(key)` | Removes an item from session storage with the given key |
| `sessionStorage.clear()` | Removes all items from session storage |
| `sessionStorage.length` | Returns the number of items in session storage |

### Using JSON with Browser Storage

- JSON is a lightweight data interchange format for storing structured data
- Use `JSON.stringify()` to convert data to a JSON string before storing in browser storage
- Use `JSON.parse()` to convert JSON data back to its original format when retrieving from browser storage

Remember that browser storage is only available in the user's current browser, and users can easily clear their browser storage or switch to a different browser/device. Use browser storage appropriately and always ask for user permission when storing sensitive information.
