# `@chakra-ui/icons` compat for easier migration to `@chakra-ui/react` v3

This package is a compatibility layer for the `@chakra-ui/icons` package to make it easier to migrate to `@chakra-ui/react` v3 as it is no longer available for V3 release and using the existing `@chakra-ui/icons` package breaks the build.

## Installation

For the most drop-in replacement that does not require any code changes, you can install this package and as an alias for `@chakra-ui/icons` which is supported by most package managers.

### npm

```sh
npm install @chakra-ui/icons@npm:chakra-ui-icons-compat
```

### yarn

```sh
yarn add @chakra-ui/icons@npm:chakra-ui-icons-compat
```

### pnpm

```sh
pnpm add @chakra-ui/icons@npm:chakra-ui-icons-compat
```

## Usage

If you installed this package as an alias for `@chakra-ui/icons`, you can continue using it as you would normally.

```jsx
import { AddIcon } from "@chakra-ui/icons";

function MyComponent() {
  return (
    <div>
      <AddIcon />
    </div>
  );
}
```

Otherwise, you need to update your imports to use the new package name.

```diff
- import { AddIcon } from "@chakra-ui/icons";
+ import { AddIcon } from "chakra-ui-icons-compat";
```

## Disclaimer

This package is a temporary solution to help with the migration to `@chakra-ui/react` v3. It is not a long-term solution, and you should update your code to use icons in the recommended way as described in the [Chakra UI documentation](https://www.chakra-ui.com/docs/get-started/migration#icons).

## License

MIT
