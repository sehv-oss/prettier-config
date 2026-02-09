# @sehv-oss/prettier-config

Shared prettier configuration for JavaScript/TypeScript projects.

## Installation

```bash
# npm
npm install --save-dev @sehv-oss/prettier-config prettier

# pnpm
pnpm add --dev @sehv-oss/prettier-config prettier

# yarn
yarn add --dev @sehv-oss/prettier-config prettier
```

## Usage

Create a `.prettier.config.ts` file at the root of your project and [extend](https://prettier.io/docs/sharing-configurations) the configuration:

```ts
// .prettier.config.ts
import type { Config } from 'prettier';

import baseConfig from '@sehv-oss/prettier-config';

const config: Config = {
  ...baseConfig,
  // your customizations here
  printWidth: 100,
};

export default config;
```
