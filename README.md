# Next.js Links Not Working in Production

This repository demonstrates a common issue in Next.js where links work perfectly in development but fail to function correctly in production.  The problem stems from a mismatch in the base URL used by Next.js's `Link` component. 

## Problem:

In the `bug.js` file, you'll find a simple component with Next.js links. While these links function flawlessly in development, they fail in production.  Clicking them doesn't navigate to the target pages.

## Solution:

The `bugSolution.js` file presents the solution. It addresses the base URL issue using the `basePath` option in `next.config.js` (or by making sure your production environment is properly configured with the correct base URL).