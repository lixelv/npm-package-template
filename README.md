# npm package template

[![GitHub Workflow Status](https://img.shields.io/badge/CI/CD-Automated-success?style=flat-square&logo=github)](https://github.com/features/actions)
[![Svelte](https://img.shields.io/badge/Svelte-Ready-FF3E00?style=flat-square&logo=svelte&logoColor=white)](https://svelte.dev/)
[![npm](https://img.shields.io/badge/npm-package-CB3837?style=flat-square&logo=npm)](https://www.npmjs.com/)

A streamlined template for creating npm packages with automated CI/CD pipeline. Built with Svelte but can be used for any JavaScript/TypeScript package.

## Features

- Automated publishing to npm on GitHub releases
- TypeScript support out of the box
- Svelte integration (optional for your package consumers)
- Pre-configured testing with Vitest
- TailwindCSS for styling development environment

## Setup Guide

1. **Create a new repository** from this template

2. **Configure your package**
   - Update `package.json` with your package name
   - Version is automatically set from GitHub release tags
   - Modify dependencies as needed for your project

3. **Set up CI/CD**
   - Generate an npm token: [Get npm token](https://www.npmjs.com/settings/<YOUR_NPM_USERNAME>/tokens)
   - Add token as `NPM_TOKEN` in GitHub secrets: [Create GitHub secret](https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_GITHUB_REPOSITORY>/settings/secrets/actions)
   - Replace `<YOUR_NPM_USERNAME>`, `<YOUR_GITHUB_USERNAME>`, and `<YOUR_GITHUB_REPOSITORY>` with your actual values

4. **Release your package**
   - Create a GitHub release with a semantic version tag (e.g., `v1.0.0`)
   - The workflow automatically builds and publishes your package to npm

---

<div align="center">
  <code>npm install your-package-name</code>
</div>