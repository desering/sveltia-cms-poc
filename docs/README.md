# sveltia-cms-poc

A poc/template for multilingual static sites built with
[Astro](https://astro.build) and [Sveltia](https://github.com/sveltia/sveltia-cms).

It only supports the subdirectory URL format. Each language is managed with a
URL like the following. The root URL will redirect to the specified default
language.

- example.com/en/
- example.com/es/

## Features

- [x] Support for Astro's official i18n functionality
- [x] Various methods for managing multilingual pages
- [x] Vanilla CSS
- [x] SEO-friendly

## Getting started

Install dependencies:

```shell
bun i
```

Run dev server:
```shell
bun run --bun dev
```

Run tests with vitest (`vi.mock` depends on Node.js behavior for module
interception and is not compatible with the `--bun` runtime):
```shell
bun run test
```

## Deployment

GHA workflow builds static site and pushes it to GitHub Pages.

Sveltia CMS requires an Oauth client to allow users to authenticate to GitHub.
See https://github.com/desering/sveltia-cms-auth.
