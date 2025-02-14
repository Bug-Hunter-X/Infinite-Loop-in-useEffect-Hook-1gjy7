# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The example shows how omitting the dependency array in `useEffect` can lead to an infinite render loop.  The solution provides the correct way to use `useEffect` to prevent this problem. 

## Bug Description

The `useEffect` hook is used to perform side effects after rendering a component.  However, if the dependency array is omitted or incorrect, the effect will run after every render, potentially causing an infinite loop.

## Bug Solution

The solution demonstrates the correct use of dependency arrays in the `useEffect` hook. By specifying the dependency `count`, the effect only runs when `count` changes, preventing the infinite loop.
