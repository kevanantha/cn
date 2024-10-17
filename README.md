# Tailwind CSS Class Merging Utility

Utility function for merging Tailwind CSS class names efficiently.

## Installation

To install this package, run:

```bash
# deno
deno add jsr:@vyn/cn
# or import directly with a jsr specifier
import * as mod from "jsr:@vyn/cn";

# npm
npx jsr add @vyn/cn
```

## Usage

The package exports a single function `cn` which can be used to merge Tailwind CSS class names:

```typescript
import { cn } from '@vyn/cn';

const className = cn('text-red-500', 'bg-blue-200', 'p-4');
const classNames = cn(['text-red-500', 'bg-blue-200', 'p-4']);
```

## API

### `cn(...inputs: ClassValue[]): string`

Merges the provided class names, resolving conflicts and duplicates efficiently.

- `inputs`: An array of class names or objects representing class names.
- Returns: A string of merged class names.

## Dependencies

This package depends on:

- [clsx](https://github.com/lukeed/clsx): A tiny utility for constructing `className` strings conditionally.
- [tailwind-merge](https://github.com/dcastil/tailwind-merge): A utility function to efficiently merge Tailwind CSS classes without style conflicts.

## License

[MIT License](LICENSE)

<!-- ## Contributing -->
<!---->
<!-- Contributions are welcome! Please feel free to submit a Pull Request. -->
<!---->
<!-- ## Support -->
<!---->
<!-- If you encounter any problems or have any questions, please open an issue in the GitHub repository. -->
