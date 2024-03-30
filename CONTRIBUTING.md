# Code Standards

## Naming Conventions

### Variables, functions, mixins, and placeholders

- Use lowercase letters.
- Use hyphens to separate words.

#### Examples

```scss
# Variables
❌ $pxToRem           # Using camelCase
❌ $px_to_rem         # Using underscores
❌ $PxToRem           # Using camelCase with the first letter capitalized

✅ $px-to-rem         # Correct

# Functions
❌ pxToRem()          # Using camelCase
❌ px_to_rem()        # Using underscores
❌ PxToRem()          # Using camelCase with the first letter capitalized

✅ px-to-rem()        # Correct

# Mixins
❌ pxToRem()          # Using camelCase
❌ px_to_rem()        # Using underscores
❌ PxToRem()          # Using camelCase with the first letter capitalized

✅ px-to-rem()        # Correct

# Placeholders
❌ %pxToRem           # Using camelCase
❌ %px_to_rem         # Using underscores
❌ %PxToRem           # Using camelCase with the first letter capitalized

✅ %px-to-rem         # Correct
```

**Note:** The `$` symbol is used to indicate a variable, and the `%` symbol is used to indicate a placeholder. This is a convention used in Sass and we should follow it.

### File Naming

- Use lowercase letters.
- Use hyphens to separate words.
- Use `_` at the beginning of any `.scss` file so it won't compile (except for the `main.scss` file).
- The style file extensions will be `.scss` (not `.sass`).
- Don't repeat the module name in the file name.

#### Examples

```bash
❌ px-to-rem.scss           # Not using `_` at the beginning
❌ _px-to-rem.sass          # Using `.sass` instead of `.scss`
❌ _px-to-rem-module.scss   # Repeating the module name
❌ _pxToRem.scss            # Using camelCase

✅ _px-to-rem.scss          # Correct
```
