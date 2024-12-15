# React Router Dom Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom. The catch-all route, intended to handle 404 errors, is unexpectedly overriding other defined routes.

## Problem

The provided `App.js` file includes a catch-all route that is incorrectly intercepting all other routes, regardless of their validity.  This often happens silently after an upgrade to newer versions of `react-router-dom`.

## Solution

The `AppSolution.js` file presents a correct implementation. The key is to ensure the catch-all route is placed correctly within your route structure. It should be the last route defined.