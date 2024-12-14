# Next.js 15 Data Fetching Error Handling

This repository demonstrates a common error in Next.js 15 applications related to data fetching within `getStaticProps`.  Specifically, it highlights the need for robust error handling when fetching data, preventing runtime errors when the data fetch fails.

## The Problem

The `bug.js` file showcases code that fails to adequately handle potential errors during data fetching. If the API request in `getStaticProps` fails, the component attempts to render `data`, which is `undefined` or `null`, causing a runtime error.

## The Solution

The `bugSolution.js` file demonstrates a correct approach.  It includes a `try...catch` block to handle potential errors and returns a default value (e.g., `null` or an empty object) if an error occurs. This prevents the runtime error and provides a graceful fallback.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npm run dev` to start the development server.