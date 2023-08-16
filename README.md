# NPM Library Template

This repo is a template for creating CommonJS and ESM packages using Typescript to release on NPM.

- It uses `tsc` to transpile to CommonJS and `rollup` to build the ESM packages.
- Has a default MIT license
- Eslint rules from [@blb-ventures/eslint-config](https://github.com/blb-ventures/eslint-config)
- Prettier and EditorConfig
- Github Actions with:
  - Release: using [release-please](https://github.com/googleapis/release-please) that automates CHANGELOG generation
  - Testing: as a default it just run eslint

## Before Publish Checklist

- [ ] Update the license
- [ ] Update `rollup.config.js` external packages
- [ ] Update `src/external.ts` to include all the lib files
- [ ] Update `src/index.ts` line 4 to export a named module (optional)
- [ ] Update package.json
  - [ ] Package name
  - [ ] Package version
  - [ ] Homepage
  - [ ] Repository
  - [ ] Bugs url
  - [ ] Author
  - [ ] License
  - [ ] Contributors
