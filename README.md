## Next.js App

Basic dashboard application.

Created a database in the same region as your application code to reduce latency between your server and database.

Fetched data on the server with React Server Components. This allows you to keep expensive data fetches and logic on the server, reduces the client-side JavaScript bundle, and prevents your database secrets from being exposed to the client.

Used SQL to only fetch the data you needed, reducing the amount of data transferred for each request and the amount of JavaScript needed to transform the data in-memory.

Parallelize data fetching with JavaScript - where it made sense to do so.

Implemented Streaming to prevent slow data requests from blocking your whole page, and to allow the user to start interacting with the UI without waiting for everything to load.

Move data fetching down to the components that need it, thus isolating which parts of your routes should be dynamic.
