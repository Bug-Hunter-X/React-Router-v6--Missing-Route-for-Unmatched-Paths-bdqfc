# React Router v6 - Handling Unmatched Routes

This repository demonstrates a common issue in React Router v6:  the lack of a catch-all route to handle unmatched paths. Without such a route, navigating to a non-existent path results in a blank screen, a poor user experience.

The `App.js` file shows the problem - a missing route for unmatched paths. The solution is provided in `AppSolution.js`

## How to Reproduce the Bug

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Navigate to a URL that does not match any of the defined routes (e.g., `/invalid-path`).  Observe a blank screen.

## Solution

The solution adds a catch-all `Route` with `path="*"` to handle any unmatched paths, displaying a custom 404 page.
