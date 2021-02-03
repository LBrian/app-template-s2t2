# Snowpack + Svelte + Tailwind + Typescript template
A GitHub and `csa-teamplate` tempalte to start developing SSTT in seconds.

![svelte](https://img.shields.io/badge/svelte-3.32.1-blue)
![tailwindcss](https://img.shields.io/badge/tailwindcss-2.0.2-blue)
![Typescript](https://img.shields.io/badge/typescript-4.1.3-blue)
![snowpack](https://img.shields.io/badge/snowpack-3.0.11-blue)

<span><img src="https://github.com/LBrian/app-template-svelte-typescript-tailwind/blob/main/public/logo.svg?raw=true" width="40px" alt="svelte"></span>
<span><img src="https://github.com/LBrian/app-template-svelte-typescript-tailwind/blob/main/public/tailwindcss.svg?raw=true" width="70px" alt="tailwindcss"></span>
<span><img src="https://github.com/LBrian/app-template-svelte-typescript-tailwind/blob/main/public/typescript.png?raw=true" width="40px" alt="typescript"></span>
<span><img src="https://github.com/LBrian/app-template-svelte-typescript-tailwind/blob/main/public/snowpack.png?raw=true" width="50px" alt="snowpack"></span>

## Why this template
[See more](https://ralphbliu.medium.com/s2t2-snowpack-svelte-tailwindcss-typescript-8928caa5af6c)
* Purge unused TailwindCSS untilities
* No unnecessary messy `postcss` dependencies

## Create a new app
`npx create-snowpack-app my-app --template app-template-svelte-typescript-tailwind`

### npm start

Runs the app in the development mode.
Open http://localhost:8080 to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console.

### npm test

Launches the test runner in the interactive watch mode.
See the section about running tests for more information.

### npm run build

Builds a static copy of your site to the `build/` folder.
Your app is ready to be deployed!

**For the best production performance:** Add a build bundler plugin like [@snowpack/plugin-webpack](https://github.com/snowpackjs/snowpack/tree/main/plugins/plugin-webpack) or [snowpack-plugin-rollup-bundle](https://github.com/ParamagicDev/snowpack-plugin-rollup-bundle) to your `snowpack.config.json` config file.

### Q: What about Eject?

No eject needed! Snowpack guarantees zero lock-in, and CSA strives for the same.
