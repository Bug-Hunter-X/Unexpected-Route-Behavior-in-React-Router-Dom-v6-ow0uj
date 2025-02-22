# React Router Dom v6 Unexpected Route Behavior

This repository demonstrates an uncommon bug encountered when using React Router Dom v6.  The issue involves unexpected behavior when navigating to a route that doesn't exist.  The provided solution demonstrates a way to handle this gracefully and prevent unexpected rendering issues.

## Bug Description

When navigating to a route that is not defined in the `Routes` component, the application may behave unexpectedly.  This might manifest as an empty screen or a different component rendering instead of a 404 or similar error handling page.

## Solution

The solution implements an error boundary using a `Route` with `path="*"` to catch all undefined routes and display a custom 404 page.