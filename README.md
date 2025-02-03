# React Native useRef Hook Returns Null

This repository demonstrates a common error encountered when using the `useRef` hook in React Native.  The problem arises because the ref object might be unexpectedly null even after the component has mounted. This can occur if you try to access the `current` property of the ref before React has fully initialized it.

## Problem
The issue is explained in detail in the `bug.js` file.  Accessing `animatedValue.current` before it's initialized throws an error. 

## Solution
The `bugSolution.js` file shows a robust solution. It utilizes a conditional check to ensure the ref is properly initialized before attempting to access its `current` property, preventing the runtime error.