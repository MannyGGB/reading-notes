# Class 15 (10/11/2023)

## Manifest

- We use manifest to turn a website app into a progressive web app (PWA).
  (https://dev.to/bhendi/turn-your-react-vite-app-into-a-pwa-3lpg)

- npm install -D workbox-window vite-plugin-pwa
- Import the plugin we have installed using at the top of your vite.config.ts file.
  - import { VitePWA } from "vite-plugin-pwa";
- // https://vitejs.dev/config/

```

export default defineConfig({
    base: "./",
    plugins: [react(), VitePWA(manifestForPlugin)],
});


```

- manifest key must be identical to your manifest.json
- PWA Asset Generator https://www.npmjs.com/package/pwa-asset-generator

## Final Project Guidelines

(https://github.com/Tech-Educators/sept-2023-bootcamp/tree/main/301/final-project)

(https://github.com/elsewhencode/project-guidelines)
