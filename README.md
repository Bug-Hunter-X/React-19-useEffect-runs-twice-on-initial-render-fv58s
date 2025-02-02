# React 19 useEffect Runs Twice on Initial Render

This repository demonstrates a common issue in React 19 where the `useEffect` hook runs twice on the initial render when combined with `useState`.  The problem is analyzed, and a solution is provided.

## Problem
The `useEffect` hook, designed to perform side effects after render, unexpectedly runs twice during the initial render.  This can lead to unexpected behavior and performance issues.

## Solution
The solution involves carefully managing the dependencies array passed to `useEffect`. By ensuring that the dependencies array accurately reflects the values that trigger the effect, we can eliminate the redundant execution.