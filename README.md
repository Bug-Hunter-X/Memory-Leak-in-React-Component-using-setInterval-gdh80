# React setInterval Memory Leak

This repository demonstrates a common mistake when using `setInterval` within a React component's `useEffect` hook: forgetting to clear the interval when the component unmounts. This leads to a memory leak, as the interval continues to run even after the component is no longer needed.

The `bug.js` file contains the faulty code.  The `bugSolution.js` file provides the corrected version.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the continuously increasing counter even after unmounting the component.  The memory leak is evident via the browser's developer tools.