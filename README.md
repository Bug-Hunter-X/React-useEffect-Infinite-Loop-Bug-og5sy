# React useEffect Infinite Loop Bug

This repository demonstrates a common mistake when using the `useEffect` hook in React, leading to an infinite loop.  The problem arises from an incorrectly specified dependency array, causing the effect to re-run on every render.

## Bug Description
The provided `MyComponent` utilizes `useEffect` without correctly specifying the dependency array. This results in the effect running after every render, including renders caused by the `setCount` function, creating a continuous loop and potentially crashing the application.