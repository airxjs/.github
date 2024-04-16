# Airx

☁️ Airx is a lightweight JSX web application framework.

Airx is a front-end framework based on JSX, designed to provide a simple and straightforward solution for building web applications. While it does not include hooks like React, it offers a range of features to manage state and handle user interactions efficiently.

## Features

- Create reaction values for managing dynamic data
- Define components using JSX syntax
- Lightweight and easy to learn

## Getting Started

To get started with Airx, follow these steps:

1. Install Airx using npm or yarn:

   ```shell
   npm install airx
   ```

2. Import the necessary functions and components in your project:

   ```javascript
   import * as airx from 'airx';

   // Your code here
   ```

3. Start building your web application using Airx's API and features.

## Examples

Here's a simple example demonstrating the usage of Airx:

```javascript
import * as airx from 'airx';

// Create a reaction value
const count = airx.createSignal(0);

// Define a component
function App() {
  const handleClick = () => {
    count.value += 1;
  };

  // Return a render function
  return () => (
    <div>
      <h1>Counter: {count.value}</h1>
      <button onClick={handleClick}>Increment</button>
    </div>
  );
}

// Mount the app to the DOM
airx.createApp(<App />).mount(document.getElementById('app'));
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.

## Acknowledgments

We would like to thank all the contributors and supporters of the Airx project.

---

For more information, check out the [official documentation](https://github.com/airxjs/airx).
