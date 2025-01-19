# React Router DOM v6 - Unexpected Route Behavior with Missing Parameters

This repository demonstrates a subtle bug in React Router DOM v6 related to routes with parameters where those parameters might be missing from the URL.  The issue involves the route failing to render correctly when the expected parameters are absent.

## Bug Description
The provided `bug.js` file shows a simple React app using React Router DOM v6. The `/users/:id` route is supposed to display user information.  However, if a user navigates directly to `/users` (without specifying an `id`), the component associated with that route does not render as expected.

## Solution
The `bugSolution.js` file offers a solution using the `useParams` hook to gracefully handle the case where the parameter is missing.