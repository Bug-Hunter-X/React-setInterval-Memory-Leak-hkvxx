# React setInterval Memory Leak

This repository demonstrates a common error in React applications: memory leaks caused by the improper use of `setInterval` within a `useEffect` hook.  The example showcases a component that updates a counter every second. Without proper cleanup, the interval continues running even after the component unmounts, resulting in memory leaks.

The solution provided addresses this issue by incorporating a cleanup function within the `useEffect` hook to clear the interval when the component unmounts.