# NPM Library Template

This repo is a template for creating CommonJS and ESM packages using Typescript to release on NPM.

- It uses `tsc` to transpile to CommonJS and `rollup` to build the ESM packages.
- Has a default MIT license
- Eslint rules from [https://github.com/blb-ventures/eslint-config](@blb-ventures/eslint-config)
- Prettier and EditorConfig
- Github Actions with:
  - Release: using [https://github.com/googleapis/release-please](release-please) that automates CHANGELOG generation
  - Testing: as a default it just run eslint

## Before Publish Checklist

- [ ] Update the license
- [ ] Update `rollup.config.js` external packages
- [ ] Update `src/external.ts` to include all the lib files
- [ ] Update `src/index.ts` line 4 to export a named module (optional)
- [ ] Update package.json
  - [ ] Set the package name
  - [ ] Set the package version
  - [ ] Set the homepage
  - [ ] Set the repository
  - [ ] Set the bugs url
  - [ ] Set the author
  - [ ] Set the license
  - [ ] Set the contributors
