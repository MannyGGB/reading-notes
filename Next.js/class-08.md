# Class 08 (23/11/2023)

## Deployment, automatic deployments, pull requests and branch previews

- When deploying from main, the environment is production.
- When deploying from a branch, environment is preview.
  - After a pull request and merge is done, the branch environment will be pushed to production.
- GitHub and Vercel are integrated, so both have to merge and deploy without errors for the app to work.
- In the Deployment tab, you can check all previous deployments, and you can navigate through the links to see previous versions of the app.
- Everytime you acp, Vercel will start a new deployment automatically.
