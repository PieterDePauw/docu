# Documentation Repository

This repository hosts the documentation for our project, which is generated and maintained using a combination of Markdown and MDX files. Additionally, we have implemented the [Supabase Embeddings Generator GitHub Action](https://github.com/supabase/embeddings-generator) to improve searchability and enhance the documentation experience for users.

[![generate_embeddings](https://github.com/PieterDePauw/documentation-vector-search/actions/workflows/generate_embeddings.yml/badge.svg)](https://github.com/PieterDePauw/documentation-vector-search/actions/workflows/generate_embeddings.yml)

## Table of Contents

- [Overview](#overview)
- [Structure](#structure)
- [Documentation Organization](#documentation-organization)
- [Documentation Maintenance](#documentation-maintenance)
- [Search Optimization](#search-optimization)
- [Contributing](#contributing)

## Overview

This repository contains all the documentation required for our project. The documentation is stored in a `docs` directory and is written in Markdown (`.md`) and MDX (`.mdx`) formats. The primary goal of this repository is to provide clear, comprehensive, and easily navigable documentation for all users.

## Structure

The repository is structured as follows:

```
.
├── .github
│   └── workflows
│       └── embeddings-generator.yml  # GitHub Action configuration
├── docs
│   ├── index.md                      # Entry point for documentation
│   ├── getting-started.md            # Basic introduction and setup guide
│   ├── guides
│   │   ├── guide1.md                 # Guide 1 documentation
│   │   ├── guide2.md                 # Guide 2 documentation
│   │   └── ...
│   ├── reference
│   │   ├── api-reference.md          # API reference documentation
│   │   └── ...
│   ├── tutorials
│   │   ├── tutorial1.mdx             # Tutorial 1 with interactive components
│   │   └── ...
│   └── ...
├── README.md                         # This file
└── ...
```

## Documentation Organization

To ensure consistency and ease of navigation, the documentation should be organized as follows:

1. **Home Page (`index.md`)**: This should serve as the main entry point and provide an overview of the documentation structure.

2. **Getting Started**: Include a `getting-started.md` that provides an introduction to the project, installation instructions, and a quick start guide.

3. **Guides**: The `guides/` directory should contain detailed guides on various topics. Each guide should be a self-contained document that covers a specific aspect of the project.

4. **Reference**: The `reference/` directory should hold all reference materials, such as API documentation, command references, and configuration details.

5. **Tutorials**: The `tutorials/` directory is for step-by-step tutorials, preferably written in MDX to include interactive components where necessary.

## Documentation Maintenance

### Writing and Updating Documentation

- **Consistency**: Ensure that the tone, style, and structure of the documentation are consistent across all files. Follow a unified style guide for Markdown and MDX.

- **Version Control**: When updating documentation, clearly indicate which version of the software it pertains to. Use versioned directories or tags if necessary.

- **Links**: Use relative links for referencing other documentation files within the `docs` directory to ensure that the documentation remains portable.

### Search Optimization

The Supabase Embeddings Generator GitHub Action is configured to automatically generate embeddings for your documentation, improving its searchability.

- **Triggering the Action**: The action is triggered automatically on each commit to the `main` branch or on demand by manually dispatching the workflow.

- **Embedding Updates**: After every significant update to the documentation, the embeddings should be regenerated to ensure that search results remain relevant.

- **Monitoring**: Regularly monitor the action’s output to ensure that embeddings are generated correctly and search results are effective.

## Contributing

Contributions to the documentation are welcome. Please follow these steps when contributing:

1. **Fork the Repository**: Create a fork of the repository to your GitHub account.

2. **Create a New Branch**: Make your changes in a new branch, ideally with a descriptive name.

3. **Write/Update Documentation**: Add or update the relevant Markdown or MDX files in the `docs/` directory.

4. **Commit and Push**: Commit your changes with a descriptive message and push them to your fork.

5. **Create a Pull Request**: Open a pull request against the `main` branch of this repository. Provide a clear description of what your changes do and why they are necessary.

6. **Review Process**: Your pull request will be reviewed by maintainers. Please be responsive to any feedback provided.

This README provides an overview of how to navigate, organize, and maintain the documentation within this repository. Following these guidelines will ensure that our documentation remains high-quality, easy to use, and effective in helping users understand and engage with our project.
