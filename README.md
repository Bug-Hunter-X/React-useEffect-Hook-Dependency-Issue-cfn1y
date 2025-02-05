# React useEffect Hook Dependency Issue

This repository demonstrates a common error in React applications related to the `useEffect` hook and its dependency array.

## The Problem

The `useEffect` hook in the `bug.js` file is missing a crucial dependency. This leads to the effect running after every render, potentially causing performance problems or infinite loops.

## The Solution

The `bugSolution.js` file shows the corrected code. By including the `count` state variable in the dependency array, the effect only runs when `count` changes, solving the issue.

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console logs and the behavior of the component in both versions of the code.