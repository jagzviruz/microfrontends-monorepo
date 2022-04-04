### What does this project use ?

#### Yarn workspaces

Yarn workspaces are used to optimize dependency management. When we use yarn workspaces, all project dependencies are installed in one go. Tools like Lerna make use of Yarn workspaces' low-level primitives.

#### Lerna

Lerna is a tool used to manage monorepos. The repositories are structured into sub repositories. It is typically used in large codebases for shared dependency management and code deployment. Lerna has two major features, namely bootstrap and publish.

lerna bootstrap
This is a command provided by Lerna that does the following:

It installs the dependencies of all the packages within the monorepo.
It creates links between shared dependencies so that the same package is not installed twice.

```
lerna publish
```

The publish command publishes the package updated since the last version release.

#### Webpack - Module federation

This is the magic sauce for implementing Microfrontends.

#### Typescript
