---
id: bit-tools
title: Bit and Other Tools
---

## Git and Bit

Git is a distributed version-control system for tracking changes in source code during software development. Git manages changes in files' contents without any reference to their structure or semantics. Bit adds a layer on top of Git that understands the internal structure of the code as components and managing their internal relationships.  

Bit augments Git to:  

- Bundle files into components so they become granular shareable components.
- Add an automatic layer for versioning components (creates package.json)
- Mock building and testing in components as if they are outside of the repository while still in the repository

Bit does not require Git to exist in the project, but it can use Git's functionality to perform actions such as code merging. Bit should not replace Git in project development. The project's code should remain in Git.  

## NPM / Yarn and Bit

A component packaged with Bit is a valid NPM package and can be installed using NPM or Yarn.  

Package registries and tools like NPM and Yarn help to manage distributable artifacts. NPM and Yarn manage the dependencies for each package, according to the explicit definition in the package.json files.

- Bit automates code packaging based on code analysis.  
- Bit provides access to package code with a single command without leaving the project context.
- Bit manages dependencies between packages and automatic versioning based on dependencies

## Storybook and Bit

Storybook is a fantastic aid tool for visually developing components in simulated isolation and creating visual documentation for components based on their stories.

Bit facilitates a full lifecycle of components development. Bit tracks changes to the components, package them for distribution, merge code changes, track versions, and showcase them on a cloud hub.  

Through bit.dev, the components are not only put on display but can also be directly consumed.  

Storybook and Bit can live separately or side by side. For example, Bit can be used to isolate, build, test, and publish multiple components from a repository. Storybook can provide the visual development environment for the component prototyping to create examples that leverage the component discovery experience in bit.dev.
