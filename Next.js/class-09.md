# Class 09 (23/11/2023)

## Build Time and Request Time

(https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)
(https://nextjs.org/docs/app/building-your-application/rendering/server-components#server-rendering-strategies)

- Build time renders static data once and sends it to the server as HTML.
  - Static data does not need to be rendered every time we run the app, so it's rendered once and then retrieved as static HTML.
  - Satic routes are prerendered at build time (when Vervel builds the whole app).
- Request time renders dynamic data every time is accessed by the user because it doesn't know ahead of time what the data will be.
  - We use request time to render dynamic routes (server-side rendering).
