# React useState Unexpected Increment Bug

This repository demonstrates a subtle bug related to the React `useState` hook. When the `setCount` function is called multiple times within a single event handler, the updates may not behave as expected, leading to unexpected increments.

## Bug Description

The `MyComponent` component uses `useState` to manage a counter.  The `handleClick` function increments the counter by 1, but when called, it does so twice, resulting in the counter jumping by 2 instead of 1. This happens because of React's batching mechanism.