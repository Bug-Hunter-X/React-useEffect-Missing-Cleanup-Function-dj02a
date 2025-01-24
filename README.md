# React useEffect Hook Missing Cleanup

This repository demonstrates a common error in React applications: forgetting to include a cleanup function within the `useEffect` hook.  When a component unmounts, resources allocated by the effect should be released to prevent memory leaks and other issues.  This example showcases the problem and its solution.

## Bug

The `bug.js` file contains a React component that uses the `useEffect` hook to log a message to the console when the component mounts. However, it omits the cleanup function, resulting in potential resource leaks if the component is unmounted before the effect's completion.

## Solution

The `bugSolution.js` file provides the corrected implementation of the component, including a cleanup function that logs a message when the component unmounts. This ensures that any necessary resources are properly released.
