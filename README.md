# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The bug is caused by improperly setting a state variable inside the `useEffect` callback function without correct dependency management leading to an infinite loop. The solution involves correctly managing dependencies using the dependency array.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the error in your browser's console, and the rapidly increasing counter.

## Solution
The solution is provided in `bugSolution.js` and addresses the issue by removing unnecessary state updates in the `useEffect` hook.  The updated code prevents the infinite loop and ensures the counter updates only when needed. 