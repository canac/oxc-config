# oxc-config

Shared [oxlint](https://oxc.rs/docs/guide/usage/linter) and [oxfmt](https://oxc.rs/docs/guide/usage/formatter) config.

## Install

```sh
pnpm add -D @canac/oxc-config oxlint oxlint-tsgolint oxfmt
```

## Usage

`oxlint.config.ts`:

```ts
import base from "@canac/oxc-config/oxlint";
import { defineConfig } from "oxlint";

export default defineConfig({
  extends: [base],
});
```

`oxfmt.config.ts`:

```ts
import base from "@canac/oxc-config/oxfmt";
import { defineConfig } from "oxfmt";

export default defineConfig({
  ...base,
});
```
