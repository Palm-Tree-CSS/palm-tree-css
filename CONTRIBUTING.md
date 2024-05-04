# How to contribute

We welcome contributions from the community to help improve our project. This document provides guidelines on how to contribute to the project, including reporting bugs, suggesting features, and submitting pull requests.

## Report an bug

If you encounter a problem with the project, please follow these steps to report the issue:

1. **Check for existing issues**: Before creating a new issue, check if the problem has already been reported by searching the [existing bug issue](https://github.com/adonyssantos/palm-tree-css/issues?q=is%3Aopen+is%3Aissue+label%3Abug).
2. **Create a new issue**: If the problem has not been reported, create a new issue by clicking on the [Bug report](https://github.com/adonyssantos/palm-tree-css/issues/new?assignees=&labels=&projects=&template=bug_report.md&title=) button. Fill in the required fields, including a clear title and description of the issue, and any relevant information that will help us understand and reproduce the problem.
3. **Provide context**: Include any relevant information that will help us understand the problem, such as the browser and version you are using, the operating system, and any steps to reproduce the issue.
4. **Submit the issue**: Once you have completed the issue template, submit the issue by clicking on the "Submit new issue" button.

After creating a new bug issue, we will start a discussion about the issue and evaluate if it is a bug or a feature request.

## Suggest a feature

If you have an idea for a new feature or enhancement, please follow these steps to suggest the feature:

1. **Check for existing suggestions**: Before creating a new suggestion, check if the feature has already been suggested by searching the [existing feature issue](https://github.com/adonyssantos/palm-tree-css/issues?q=is%3Aopen+is%3Aissue+label%3Afeature).
2. **Create a new suggestion**: If the feature has not been suggested, create a new suggestion by clicking on the [Feature request](https://github.com/adonyssantos/palm-tree-css/issues/new?assignees=&labels=&projects=&template=feature_request.md&title=) button. Fill in the required fields, including a clear title and description of the feature, and any relevant information that will help us understand and evaluate the suggestion.
3. **Provide context**: Include any relevant information that will help us understand the feature, such as the use case, the expected behavior, and any additional information that will help us evaluate the suggestion.
4. **Submit the suggestion**: Once you have completed the suggestion template, submit the suggestion by clicking on the "Submit new issue" button.

After create a new feature issue, we will start a discussion about the feature and evaluate if it fits the project's goals and roadmap.

## Submit a pull request

1. **Fork the repository**: Start by forking the project repository to your GitHub account. You can do this by clicking on the "Fork" button on the top right corner of the repository page.
2. **Clone the repository**: Clone the forked repository to your local machine using the `git clone` command. 
3. **Create a new branch**: Create a new branch for your changes using the `git checkout -b` command. The branch name should be descriptive of the changes you are making, but is not required to follow a specific format.
4. **Make your changes**: Make the necessary changes to the project to implement the feature or fix the bug. Ensure that your changes follow the all the [standards, conventions and guidelines](#standards-conventions-and-guidelines) defined in the project.
5. **Commit your changes**: Once you have made your changes, commit them to the branch using the `git commit` command. Ensure that your commit messages follow the [commit standards](#commits-standards) defined in the project. Try to keep your commits focused on a single change to make the review process easier.
6. **Push your changes**: Push your changes to the forked repository using the `git push` command.
7. **Create a pull request**: Once your changes have been pushed to the forked repository, create a new pull request by clicking on the "New pull request" button on the repository page. Ensure that the pull request is made against the `release/*` branch of the project repository.
8. **Fill in the pull request template**: Fill in the required fields in the pull request template, including a clear title and description of the changes you are making. Ensure that you have followed the [pull request checklist](#for-the-reviewer) before submitting the pull request.
9. **Submit the pull request**: Once you have completed the pull request template, submit the pull request by clicking on the "Create pull request" button.

## For the reviewer

If you are reviewing a pull request, please follow these guidelines to ensure a smooth review process:

1. **Check the commit message**: Verify that the commit message follows the [commit standards](#commits-standards) defined in the project.
2. **Check the code style**: Ensure that the code follows the [code standards](#code-standards) and [naming conventions](#naming-conventions) defined in the project.
3. **Check the code quality**: Verify that the code additions do not introduce any linting errors or unit test failures.
4. **Provide constructive feedback**: If you have suggestions for improvement, provide clear and constructive feedback to help the contributor make the necessary changes.
5. **Approve the pull request**: If the pull request meets the project's standards and the changes are significant, approve it and merge it into the `release/*` branch.
6. **Consider creating an issue for minor changes**: If the pull request contains minor or insignificant changes, consider creating a new issue with the label `cr-improve`. This will allow for discussion on whether these changes are necessary and can be worked on in a separate branch. Since we are working with release branches, there is no concern about these changes reaching production, and in the worst case, they can be reverted before reaching production. The goal is to avoid demotivating contributors by requesting numerous insignificant or less relevant changes that could be worked on in a separate branch or by another contributor.
7. **Use common sense**: It's important to use common sense when reviewing pull requests. If a pull request was created with malicious intent or introduces intentional bugs, it's important to communicate with the author and provide constructive feedback. If the author refuses to address the issues, the pull request should be closed.

## Standards, conventions and guidelines

### Naming conventions

#### Variables, functions, mixins, and placeholders

- Use lowercase letters.
- Use hyphens to separate words.

**Examples**

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

##### File Naming

- Use lowercase letters.
- Use hyphens to separate words.
- Use `_` at the beginning of any `.scss` file so it won't compile (except for the `main.scss` file).
- The style file extensions will be `.scss` (not `.sass`).
- Don't repeat the module name in the file name.

**Examples**

```bash
❌ px-to-rem.scss           # Not using `_` at the beginning
❌ _px-to-rem.sass          # Using `.sass` instead of `.scss`
❌ _px-to-rem-module.scss   # Repeating the module name
❌ _pxToRem.scss            # Using camelCase

✅ _px-to-rem.scss          # Correct
```

### Code standards

- Use 2 spaces for indentation.
- Use a new line after the closing brace `}` of a rule declaration.
- Use a new line at the end of the file.
- Use a new line between rules.
- Use a one declaration per line in rule declarations.
- Use a space after the colon `:` in rule declarations.
- Use a space after the comma `,` in rule declarations.
- Use a space before the opening brace `{` in rule declarations.
- Use double quotes for strings.
- Use hyphens to separate words in class names.

### Commits standards

Semantic commits are a way of writing commit messages that follow a standardized structure, making them more readable and understandable for both humans and machines. We base our commit messages on the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification.

**🚀 Some benefits of semantic commits are:**

- Enhance communication and understanding of project history.
- Facilitate task automation, such as generating changelogs or version management.
- Enable more precise tracking of project progress.

#### Structure of a semantic commit 🏗️

A semantic commit consists of three main parts:

1. **Commit type**: Indicates the type of change made. In this project, we use the following commit types:
   - `build` Changes related to the build system or external dependencies.
   - `chore` Project maintenance tasks, such as dependency updates.
   - `ci` Changes related to the continuous integration system.
   - `docs` Documentation changes.
   - `feat` Introduces a new feature.
   - `fix` Fixes a bug.
   - `perf` Improves performance.
   - `refactor` Code structure changes without modifying its functionality.
   - `release` Changes related to the release process.
   - `revert` Reverts a previous commit.
   - `security` Improves security.
   - `style` Code style changes, such as indentation or formatting (Don't to be confused with `css` or `scss` changes).
   - `temp` Temporary commit that will be removed later.
   - `test` Adds or modifies tests.
   - `wip` Work in progress.   

2. **Scope (optional)**: Specifies the area of the project affected by the change. It is written in parentheses after the commit type. If the commit affects the entire project, the scope can be omitted. In this project, we use the following scopes:
   - `core` Changes related to the core functionality of the project.
   - `docs` Changes related to the project documentation.
   - `styles` Changes related to the project styles.
   - `tests` Changes related to the project tests.
   - `utils` Changes related to the project utilities.

3. **Description**: A brief description of the change made. It should be clear, concise, and understandable to anyone reading the project history.

