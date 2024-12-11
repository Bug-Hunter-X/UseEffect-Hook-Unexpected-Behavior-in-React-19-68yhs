# React 19 useEffect Hook Unexpected Behavior

This repository demonstrates an unexpected behavior observed with the `useEffect` hook in React 19.  The `useEffect` hook, even with an empty dependency array, appears to be executing on every render instead of only once after the initial render.  This is counter to the expected behavior.

## Bug Description
The provided `MyComponent` uses `useEffect` with an empty dependency array (`[]`).  Logically, the effect should only run once after the initial render. However, in React 19, this example shows the effect logging 'Effect ran!' on every render. This causes unexpected side effects and performance issues.

## Solution
The issue likely arises from a misunderstanding of how `useEffect` works or a bug within a specific React version or related library.  The correct implementation ensures that the effect runs only once by using the empty dependency array correctly, and double-checking that other parts of the component aren't causing unintended re-renders.