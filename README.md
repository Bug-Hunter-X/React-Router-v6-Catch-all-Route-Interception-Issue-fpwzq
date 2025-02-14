# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6.  The catch-all route unexpectedly intercepts all other routes, making it impossible to navigate to pages defined before it.

## Problem

The primary issue is that the `/*` route in `Routes` is too broad and matches every possible path, overshadowing other more specific routes.

## Solution

The problem is solved by reordering the routes, moving the catch-all route to the end of the routes list. This ensures that more specific routes are matched before the catch-all route.