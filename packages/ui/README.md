# @repo/ui

Shared UI component library for all applications in the monorepo.

## Purpose

Provide consistent, reusable UI components across all demo applications:

- Buttons, inputs, and form elements
- Cards and containers
- Navigation components
- Charts and data visualization
- Loading states and skeletons
- Modals and dialogs
- Toast notifications

## Tech Stack

- React 18+
- TypeScript
- Tailwind CSS
- Radix UI for accessible primitives
- Class Variance Authority (CVA) for component variants

## Usage

In any app or package:

```typescript
import { Button, Card, Input } from '@repo/ui';

export default function MyComponent() {
  return (
    <Card>
      <Input placeholder="Enter text" />
      <Button variant="primary">Submit</Button>
    </Card>
  );
}
```

## Development

```bash
# Build the package
pnpm build --filter=@repo/ui

# Watch mode for development
pnpm dev --filter=@repo/ui
```

## Component Structure

```
ui/
├── src/
│   ├── components/     # React components
│   ├── styles/        # Shared styles
│   └── index.ts       # Public exports
├── package.json
└── tsconfig.json
```

## Design System

Follows a consistent design system with:
- Color palette
- Typography scale
- Spacing system
- Component variants
- Accessibility standards
