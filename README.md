# React Native FlatList Rendering Error: Missing or Duplicated Items

This repository demonstrates a common error in React Native when using FlatList, where items are missing, duplicated, or rendered out of order due to missing or non-unique keys.  The solution shows how to correctly implement unique keys to resolve the issue.

## Bug Description
The FlatList component requires a unique `key` prop for each item in its data array.  Without unique keys, FlatList cannot efficiently track changes, leading to incorrect rendering.

## Bug Reproduction
1. Clone this repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
4. Observe the incorrect rendering of the FlatList in the app.

## Solution
The solution involves adding a unique `key` prop to each item in the FlatList data array. This key should be unique across all items and ideally should be based on data that identifies each item uniquely.

## Lessons Learned
Always ensure each item in a FlatList has a unique key prop. This is crucial for correct rendering and performance.  Use data identifiers or generate unique IDs when appropriate.

## Additional Resources
* [React Native FlatList Documentation](https://reactnative.dev/docs/flatlist)