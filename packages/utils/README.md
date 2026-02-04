# @repo/utils

Shared utility functions and helpers used across all applications.

## Purpose

Provide reusable utility functions to avoid code duplication:

- Date and time formatting
- String manipulation
- Number formatting (currency, percentages)
- Validation helpers
- Array and object utilities
- Async helpers

## Structure

```
utils/
├── src/
│   ├── date/          # Date utilities
│   ├── format/        # Formatting functions
│   ├── validation/    # Validation helpers
│   ├── async/         # Async utilities
│   └── index.ts       # Public exports
├── package.json
└── tsconfig.json
```

## Usage

```typescript
import { 
  formatCurrency, 
  formatDate, 
  debounce,
  validateEmail 
} from '@repo/utils';

// Currency formatting
const price = formatCurrency(1234.56, 'USD'); // "$1,234.56"

// Date formatting
const date = formatDate(new Date(), 'MMM DD, YYYY'); // "Feb 03, 2026"

// Debounce function
const debouncedSearch = debounce((query: string) => {
  // Search logic
}, 300);

// Email validation
const isValid = validateEmail('user@example.com'); // true
```

## Utility Categories

### Date Utilities

```typescript
export function formatDate(date: Date, format: string): string;
export function getDateRange(days: number): [Date, Date];
export function isToday(date: Date): boolean;
```

### Format Utilities

```typescript
export function formatCurrency(amount: number, currency: string): string;
export function formatPercentage(value: number, decimals?: number): string;
export function formatNumber(value: number, options?: FormatOptions): string;
```

### Validation Utilities

```typescript
export function validateEmail(email: string): boolean;
export function validateUrl(url: string): boolean;
export function validateRequired(value: unknown): boolean;
```

### Async Utilities

```typescript
export function debounce<T>(fn: Function, delay: number): Function;
export function throttle<T>(fn: Function, limit: number): Function;
export function retry<T>(fn: () => Promise<T>, attempts: number): Promise<T>;
```

## Testing

All utilities include comprehensive unit tests:

```bash
pnpm test --filter=@repo/utils
```

## Benefits

- ✅ DRY (Don't Repeat Yourself)
- ✅ Well-tested functions
- ✅ Type-safe utilities
- ✅ Performance optimized
- ✅ Tree-shakeable exports
