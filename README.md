# React Native FlatList: Duplicate Key Handling

This repository demonstrates a common error in React Native's FlatList component: using duplicate or invalid keys in the `keyExtractor` prop.  This can lead to unpredictable rendering behavior and crashes.

The `bug.js` file shows the problematic code with duplicate keys.  The `bugSolution.js` file demonstrates the correct implementation with unique keys, ensuring proper FlatList functionality.

## Problem

When keys are not unique, FlatList's internal mechanisms for managing item updates and rendering become unreliable, resulting in incorrect display or even app crashes.

## Solution

Always provide a unique key for each item in your data array using the `keyExtractor` prop.  Common strategies include using UUIDs, unique database IDs, or generating keys based on a combination of unique item properties. 