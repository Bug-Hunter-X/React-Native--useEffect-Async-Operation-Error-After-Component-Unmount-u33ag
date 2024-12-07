# React Native useEffect Async Operation Error

This repository demonstrates a common error in React Native when using the `useEffect` hook with asynchronous operations.  The issue occurs when the component unmounts before the asynchronous operation completes, resulting in a warning about updating an unmounted component. This can lead to memory leaks.

The `bug.js` file shows the problematic code, while `bugSolution.js` provides a solution using cleanup functions and the `useRef` hook to prevent state updates after unmounting.  The solution ensures that asynchronous operations are cancelled if the component unmounts before they complete.