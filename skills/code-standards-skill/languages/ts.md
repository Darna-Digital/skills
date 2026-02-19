# TypeScript / TSX

## Control Flow

- Prefer early return. No nested if statements. No if/else.

## Naming

- Make variable and function names self-explanatory. Don't add unnecessary comments. 
- Use `camelCase` for variables and functions, `PascalCase` for types and interfaces.
- Prefix interfaces with purpose, not `I` (e.g., `UserProfile` not `IUserProfile`). 
- Use descriptive boolean names: `isLoading`, `hasError`, `canSubmit`.
- File names should be kebab-case.

## Functions

- Pass parameters as objects if there are more than 2. 
- Keep functions small and single-purpose.
- Prefer `function` declarations over `const` declarations.

## Types

- Prefer `type` over `interface` unless declaration merging is needed.
- Avoid `any`. Use `unknown` when the type is truly unknown, then narrow. 
- Avoid type assertions (`as`). Prefer type guards or narrowing.
- Use discriminated unions over optional fields when variants are mutually exclusive.
- Prefer inferred types over explicit types.

## Imports

- Prefer named exports over default exports.

## Error Handling

- Never silently swallow errors. Always handle or propagate.
- Use typed errors or error result patterns over throwing when possible.
