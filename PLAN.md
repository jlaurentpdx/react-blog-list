Use an existing repo
Remove .example from file names
Use useEffect hook with a 'dependency array' to retrieve data from a database
Use the Supabase JS client to retrieve data from a db
Use useState to manage component state
Use the network tab to examine and debug the request being sent to a server and the response received from a server
Use the async/await pattern to make our asychronous code easier to read

Use Supabase to rerieve a list of blogs from an existing database

- [x] User should see a list of blog posts when the load the page
- [x] App component should have a state variable called `blogs` that defaults to an empty array
- [x] App component should use a useEffect hook to call `getBlogs` from the services layer asynchronously and then set the returned data in state
- [x] There should be a function called `getBlogs` in the services layer which calls Supabase and returns all the columns from the `blogs` table
- [x] App component should map through each item in `blogs` and create a `<BlogCard>` component for each blog item
- [x] All existing Snapshot tests should pass without needing to update the snapshot

## Hookup Supabase

- [x] Add `blog.js` in services/
- [x] Export `getBlogs` function which calls Supabase

## Hookup Supabase call to Component

- [x] Create `blogs` state using `useState`
- [x] Use `useEffect` to call `getBlogs` when the page initially renders
- [x] Set the response from `getBlogs` as the `blogs` state
- [x] `console.log` to make sure this is all working
