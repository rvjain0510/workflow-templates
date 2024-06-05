---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

name: Create Release Branch
description: Use this template to create a release branch from a different repository.
title: "[Release Branch Request] - "
labels: ["release", "workflow"]
assignees: ["username"]

body:
  - type: markdown
    attributes:
      value: |
        ## Create Release Branch

        Please fill in the details below to create a release branch.

  - type: input
    attributes:
      label: Source Repository
      description: The repository from which to create the release branch (e.g., `organization/repo-name`).
      placeholder: "organization/repo-name"
      required: true
      render: bash

  - type: input
    attributes:
      label: Branch Name
      description: The name of the new release branch.
      placeholder: "release/v1.0.0"
      required: true

  - type: input
    attributes:
      label: Source Branch
      description: The branch to create the release branch from (e.g., `main` or `develop`).
      placeholder: "main"
      required: true
