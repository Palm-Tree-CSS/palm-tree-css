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

## Semantic Commits: A Complete Guide 📝

## What are semantic commits? 🤔

Semantic commits are a way of writing commit messages that follow a standardized structure, making them more readable and understandable for both humans and machines.

## Benefits of semantic commits 🚀

- Enhance communication and understanding of project history.
- Facilitate task automation, such as generating changelogs or version management.
- Enable more precise tracking of project progress.

## Structure of a semantic commit 🏗️

A semantic commit consists of three main parts:

1. **Commit type**: Indicates the type of change made. Common commit types include:
   - :sparkles: feat: Introduces a new feature.
   - :bug: fix: Fixes a bug.
   - :wrench: chore: Project maintenance tasks, such as dependency updates.
   - :page_facing_up: docs: Documentation changes.
   - :art: style: Code style changes, such as indentation or formatting.
   - :white_check_mark: test: Adds or modifies tests.
   - :recycle: refactor: Code structure changes without modifying its functionality.

2. **Scope (optional)**: Specifies the area of the project affected by the change. It is written in parentheses after the commit type.

3. **Description**: A brief description of the change made. It should be clear, concise, and understandable to anyone reading the project history.

## Example of a semantic commit 💡

```bash
feat(parser): add ability to parse arrays
fix(validation): Fixed validation issue with user input
chore(dependencies): Updated dependencies to latest versions
docs(readme): Updated README.md with new instructions
style(css): Adjusted indentation in stylesheet for consistency
test(unit): Added unit tests for authentication module
refactor(api): Restructured API endpoints for improved readability
build: Updated build configuration for better performance
ci: Updated continuous integration configuration for faster builds
perf(database): Optimized database queries for faster response times
revert: Reverted previous commit that introduced bug in authentication
security(auth): Fixed security vulnerability in authentication process
```

This commit introduces a new feature to the parser, which is the ability to parse arrays.


## Tools for semantic commits 🛠️

There are several tools that can assist you in writing semantic commits, such as:

- **Commitizen**: A CLI tool that helps you write interactive semantic commits.
- **Semantic-Release**: A tool that automates release generation and changelogs based on semantic commits.
- **Husky**: A tool that allows you to run scripts before making commits or pushes.

## Additional resources ℹ️

- [Complete guide to semantic commits](https://www.conventionalcommits.org/es/v1.0.0-beta.2/)
- [How to write commit messages](*URL removed as it is invalid*)
- [Best practices for writing commits in Git](*URL removed as it is invalid*)

## Conclusion 🎉

Semantic commits are a simple and effective way to improve the readability and understanding of your project's history. I recommend starting to use them in your projects to take advantage of all their benefits.
