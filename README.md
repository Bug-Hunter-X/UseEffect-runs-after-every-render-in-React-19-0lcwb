# React 19 useEffect infinite loop bug

This repository demonstrates a common issue in React 19 where `useEffect` hooks run after every render, leading to unintended behavior. The example showcases a simple counter component where the `useEffect` hook logs the current count. However, because it's not properly optimized to only run when the count changes, it runs infinitely. This results in an excessive amount of logs to the console and the app potentially crashing.

The solution involves using the correct dependency array within the `useEffect` hook to ensure that it only runs when necessary.