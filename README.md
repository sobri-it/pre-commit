# Sobr-IT Pre-commit

Define all useful pre-commit hooks for Sobr-IT project (that is not already defined and maintained).

## Hooks

This project define following hooks:
- **rust-fmt**: Format rust files with cargo fmt.
- **rust-cargo-check**: Check the rust package for errors.
- **rust-build**: Build the rust package.
- **rust-no-warnings**: Build the rust package and error on warnings.
- **rust-clippy**: Lint rust source files.
- **bicep-fmt**: Format bicep files, requires az bicep command installed.

## Example

Below a how those hooks could be used:

```yaml
repos:
- hooks:
  - id: rust-fmt
  - id: rust-clippy
  - id: rust-cargo-check
  - id: bicep-fmt
  repo: https://github.com/sobri-it/pre-commit
  rev: <tag>
```
