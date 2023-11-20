# Class 01 (20/11/2023)

1. **What is Next.js?** A framework/library for React, which is server-side render.

- Main features:

  - No more react-router-dom or libraries to do basic web app features.
  - Allows SSR and SGG.
  - Automatic code splitting.
  - Fas, efficient.
  - Distinct API routes.
  - Simplified data fetching with async await in server components.
  - Data caching and revalidation APIs.

- Benefits:
  - Quickly build complext web apps.
  - Vercel implementation.
  - Much shorter JS bundles with SSR.
  - Hot module replacement: Next.js supports hot module replacement, which allows for instant code changes without requiring a full page reload.

2. **Single Page App (SPA)**

- It runs in the client.
- The client makesa request for the web app --> it downloads everything for the app and then browser takes it from there.
- It takes a bit of time to render --> it takes a while to get to the "First Constentful Paint" and webcrawlers struggle to see the actual content of the site (not great for SEO).

3. **Dynamic rendering: Server-Side Rendering (SSR)**

- The process of rendering React components on the server and sending the pre-rendered HTML to the client.
- The web server figures out our HTML page on the server and sending that back to the client.
- First Contentful Paint (FCP) is faster, and webcrawler situation is improved.
- We still need to download the js for interactivity to happen.

---

### React server components

- Because our server streams only the HTML for the server components and only the JS for any client components, our initial js bundle is much smaller.

- We can have both server components rendered on the server and streamed to the client, and client component rendered on the browser.

4. **Static rendering: Static Site Generation (SSG)**

- We can speed up our apps by only fetching my non-dynamic data only once at build time, so our server is not making requests to get the saem data.
- If we know the data in the DB is not going to change often, it is faster to generate the HTML

5. **Other competing frameworks are available**

- Remix (https://remix.run/)
- SvelteKit (https://kit.svelte.dev/)
