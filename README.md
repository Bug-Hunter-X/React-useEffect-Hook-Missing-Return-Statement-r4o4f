# React useEffect Hook Missing Return Statement
This repository demonstrates a common but easily missed error in React: forgetting the cleanup function in `useEffect` hooks.  The example showcases a component that logs a message on mount but never cleans up, potentially causing memory leaks or unexpected behavior when the component unmounts.

The solution provides the correct implementation, including the cleanup function that prevents these issues.

## How to reproduce the bug
1. Clone this repository.
2. Navigate to the `bug` directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Open your browser and observe the console logs.
6. Notice that even after unmounting the component, there is no cleanup action, indicating a potential memory leak.

## How to fix the bug
The solution provided in the `bugSolution` directory addresses the issue by adding a return statement within the `useEffect` hook.