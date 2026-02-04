# @repo/types

Shared TypeScript type definitions used across all applications and packages.

## Purpose

Provide consistent type definitions to ensure type safety across the monorepo:

- Common data models
- API request/response types
- Shared interfaces
- Utility types
- Domain-specific types

## Structure

```
types/
├── src/
│   ├── common/        # Common types (User, Response, etc.)
│   ├── api/           # API-related types
│   ├── domain/        # Domain models
│   └── utils/         # Utility types
├── package.json
└── tsconfig.json
```

## Usage

```typescript
import type { User, ApiResponse, Revenue } from '@repo/types';

function fetchUser(): ApiResponse<User> {
  // Implementation
}

const revenue: Revenue = {
  amount: 1000,
  currency: 'USD',
  date: new Date(),
};
```

## Example Types

### Common Types

```typescript
export interface User {
  id: string;
  name: string;
  email: string;
  role: UserRole;
}

export type UserRole = 'admin' | 'user' | 'viewer';
```

### API Types

```typescript
export interface ApiResponse<T> {
  data: T;
  status: number;
  message?: string;
}

export interface ApiError {
  error: string;
  code: string;
  details?: unknown;
}
```

## Benefits

- ✅ Type safety across packages
- ✅ Autocomplete in IDEs
- ✅ Catch errors at compile time
- ✅ Self-documenting code
- ✅ Easier refactoring
