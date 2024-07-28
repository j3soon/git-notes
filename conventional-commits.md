# Conventional Commits

For small projects, single-line commit messages with optional descriptions may suffice. However, for larger projects, a consistent approach to writing commit messages enhances readability and facilitates the use of parsing tools. This is why the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification was developed.

## Commit Message Format

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

If the commit is a breaking change, use `<type>[optional scope]!` instead:

```
<type>[optional scope]!: <description>

[optional body]

[optional footer(s)]
```

## Commit Types

Commit types and descriptions specified in the [Angular convention](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format), with some minor modifications:

- `fix`: A bug fix.
- `feat`: A new feature. Note that the term "feature" represents any code change, [excluding bug fixes](https://stackoverflow.com/a/64297032), that alters the program's behavior or functionality, including removal of features.
- `docs`: Documentation only changes, including [code comments](https://www.reddit.com/r/git/comments/12560kf/comment/je2tf76).
- `perf`: A code change that improves performance, without introducing new features.
- `refactor`: A code change that neither fixes a bug nor adds a feature. i.e., code refactoring.
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc). i.e., code formatting changes.
- `test`: Adding missing tests or correcting existing tests.
- `revert`: Reverts a previous commit, where the commit hash [should be provided](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#revert-commits) in the body.
- `build`: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm), which is irrelevant to the code itself.
- `ci`: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs), which is irrelevant to the code itself.
- `chore`: Changes to other configuration files (example scopes: [gitignore](https://stackoverflow.com/a/26944812)), which is irrelevant to the code itself.

For more examples, refer to the [examples section](https://www.conventionalcommits.org/en/v1.0.0/#examples) in the Conventional Commits specification.
