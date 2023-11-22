# Class 06 (22/11/2023)

## Styling

- globals.css for style you want in all pages.

  - It supports importing other CSS files to let you organise your styles as you might have done on many projects in the past.
  - You can use this will any CSS naming scheme that you would like, eg. BEM.
  - The downside to this is Next won't be able to perform page route-level code splitting on your styles like it can with modules.

- CSS modules
- Tailwind

### CSS Modules

- Specify imports per component that only affect that component.
- It can be used for components and pages too.
- name.module.css

```
mypage.tsx
mypage.module.css

```
