# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook.  The bug is caused by an incorrect dependency array, leading to an infinite render loop. The solution demonstrates how to correctly specify dependencies to avoid this issue.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. If the dependency array is missing necessary dependencies, or if it contains unnecessary dependencies, it can lead to unexpected behavior, such as infinite loops.  This example illustrates a scenario where omitting `count` from the dependency array causes an infinite loop, as the effect triggers continuously.

## Solution
The solution file correctly includes `count` in the dependency array. This ensures that the effect only runs when the `count` value changes.