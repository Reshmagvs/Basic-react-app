## Basic-React-App
1. Create a React app using these commands in VS Code terminal :

```
npx create-react-app my-app
cd my-app
```
2. To create a counter app
Replace the code to the below one , inside App.js which will be in src folder :

```
import { useState } from "react";

function CounterApp() {
  const [count, setCount] = useState(0);

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gray-100">
      <h1 className="text-3xl font-bold mb-4">Counter: {count}</h1>
      <div className="flex gap-4">
        <button
          onClick={() => setCount(count - 1)}
          className="px-4 py-2 bg-red-500 text-white rounded-lg"
        >
          Decrease
        </button>
        <button
          onClick={() => setCount(count + 1)}
          className="px-4 py-2 bg-green-500 text-white rounded-lg"
        >
          Increase
        </button>
      </div>
    </div>
  );
}

export default CounterApp;
```
3. Start the React app using this command in terminal :

```
npm start

```

