# Unnecessary Re-renders and Console Logging in React useEffect Hook

This repository demonstrates a common issue in React applications: unnecessary re-renders and excessive console logging within the `useEffect` hook.  The example shows how improper dependency management leads to inefficient updates and cluttered console output.

## Problem:

The initial code logs to the console on every state change, even when the logged value hasn't changed. This is inefficient because it causes unnecessary re-renders, and it clutters the browser's console, making it difficult to debug actual problems.

## Solution:

The solution uses dependency arrays to control when `useEffect` runs more efficiently. It only logs when the count changes to a new value, significantly improving performance and reducing console clutter.

## How to run the code

1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.