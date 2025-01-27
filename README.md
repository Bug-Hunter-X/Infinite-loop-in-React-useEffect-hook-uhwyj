# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug stems from an improperly defined dependency array, leading to an infinite loop. The solution shows how to correct this by specifying the correct dependencies.

## Bug
The `bug.js` file contains a component that uses `useEffect` to log the current count.  However, the dependency array is missing, causing the effect to run on every render, leading to an infinite loop of logging and re-renders.

## Solution
The `bugSolution.js` file shows the corrected code.  The dependency array `[count]` ensures that the effect only runs when the value of `count` changes.