# @repo/config

Shared configuration files for ESLint, TypeScript, and other tools.

## Purpose

Centralize configuration to ensure consistency across all packages and applications.

## Included Configurations

### ESLint

- `eslint-config.js` - Shared ESLint rules
- `eslint-react.js` - React-specific rules
- `eslint-next.js` - Next.js-specific rules

### TypeScript

- `tsconfig.base.json` - Base TypeScript configuration
- `tsconfig.react.json` - React-specific settings
- `tsconfig.node.json` - Node.js-specific settings

### Prettier

- `.prettierrc.js` - Code formatting rules

## Usage

### ESLint

```json
{
  "extends": ["@repo/config/eslint-react"]
}
```

### TypeScript

```json
{
  "extends": "@repo/config/tsconfig.base.json",
  "compilerOptions": {
    // App-specific overrides
  }
}
```

## Benefits

- ✅ Consistent code style
- ✅ Single source of truth
- ✅ Easy updates across all packages
- ✅ Reduced configuration duplication
