# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a problem with catch-all routes (`/*`) in React Router Dom v6 when nested within other routes.  The catch-all route fails to match any unmatched paths resulting in unexpected behavior.

The issue occurs when a catch-all route is used as a child route and other routes are defined above it within the same Routes component.  The catch-all route should ideally always be the last route defined to function as intended. However, this can cause other problems if used in nested routes.

## Solution

The solution provided addresses this issue by reorganizing the routes structure.

## How to reproduce

1. Clone this repository.
2. Run `npm install`
3. Run `npm start`
4. Navigate to a non-existent route. You will observe that the catch-all route fails to be triggered even with wrong url.
5. Use the solution file to see the working example.