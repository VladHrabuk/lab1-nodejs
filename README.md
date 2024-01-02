# Lab 1

## Task

Create project in GitHub with minimal code-quality checks and autodepoly.

### Requirements

- new repo in GitHub
- initial empty commit
- add ESlint
- add Sonar-Lint to ESLint
- add Prettier
- add check on pre-commit hooks
- add GitHub action to run checks\tests on commit or PR
- add AutoDeployment to any hosting provider
- add Editorconfig

## Answer on questions

- dev Deps vs Deps:
  - Dependencies are the packages that your project directly depends on for its normal operation.
  - DevDependencies are packages that are only needed during the development phase.
- Why we have separate tooling for formatting/linting:
  - Formatting is used to make the code look consistent and more readable.
  - Linting is used to analyze code for potential errors, bugs, and code quality issues.
- Difference with VPS/FaaS?
  - VPS is a virtualized server that acts as a dedicated server within a larger physical server. It provides users with more control and flexibility over their server environment.
    Users have root access, allowing them to install and configure software as needed.
  - FaaS is a serverless architecture. We don't have to configure anything, just write code and deploy it.
- Why we need peerDeps?
  - Peer Dependencies is a feature that allows a package to declare dependencies that are expected to be provided by the application using the package, rather than the package itself.
    It is used when a package expects the consumer to have a specific version of a dependency, and it doesn't want to include that dependency directly in its node_modules folder.
- `npm i` vs `npm ci`
  - `npm i` installs all dependencies and devDependencies, modifying package.json, package-lock.json, and node_modules folder.
  - `npm ci` ("clean install") deletes the node_modules folder and installs exactly what's in the package-lock.json for consistency.
