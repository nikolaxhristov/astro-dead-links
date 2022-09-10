# [astro-dead-links] 🪦

This **[Astro integration][astro-integration]** will automatically remove all
the dead links in your website.

## Installation

There are two ways to add integrations to your project. Let's try the most
convenient option first!

### `astro add` command

Astro includes a CLI tool for adding first party integrations: `astro add`. This
command will:

1. (Optionally) Install all necessary dependencies and peer dependencies
2. (Also optionally) Update your `astro.config.*` file to apply this integration

To install `astro-dead-links`, run the following from your project directory and
follow the prompts:

```sh
# Using NPM
npx astro add astro-dead-links
# Using Yarn
yarn astro add astro-dead-links
# Using PNPM
pnpx astro add astro-dead-links
```

### Install dependencies manually

First, install the `astro-dead-links` integration like so:

```
npm install -D -E astro-dead-links
```

Then, apply this integration to your `astro.config.*` file using the
`integrations` property:

**astro.config.ts**

```ts
import type { AstroUserConfig } from "astro";
import deadLinks from "astro-dead-links";

export default (): AstroUserConfig => ({
	integrations: [deadLinks()],
});
```

## Getting started

The utility should now automatically remove all the deadlinks from your website
and point to their origin.

[astro-dead-links]: https://npmjs.org/astro-dead-links
[astro-integration]: https://docs.astro.build/en/guides/integrations-guide/

[![Built with nikolarhristov/npm](https://raw.githubusercontent.com/nikolarhristov/npm/main/.github/img/favicon-16x16.png)](https://github.com/NikolaRHristov/npm)
