---
name: "🐛 Bug Report"
description: "File a bug report. Something isn't working as expected."
title: "[BUG]: "
labels: ["bug", "triage"]
body:
  - type: markdown
    attributes:
      value: "Thank you for taking the time to file a bug report! This helps us make A.R.C. better."
  - type: dropdown
    id: component
    attributes:
      label: "Component"
      description: "Which part of A.R.C. is affected?"
      options:
        - "cli"
        - "gateway"
        - "engine"
        - "processor"
        - "docs"
        - "Other / Unsure"
      default: 5
    validations:
      required: true
  - type: textarea
    id: description
    attributes:
      label: "Bug Description"
      description: "A clear and concise description of what the bug is."
      placeholder: "When I run `arc run`, the `gateway` service fails to connect to the `engine`..."
    validations:
      required: true
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: "Steps to Reproduce"
      description: "How can we make this bug happen on our end?"
      placeholder: |
        1. Run `arc new my-app`
        2. Add the `...` service
        3. Run `arc run`
        4. See error in logs...
    validations:
      required: true
  - type: textarea
    id: expected-behavior
    attributes:
      label: "Expected Behavior"
      description: "A clear description of what you expected to happen."
      placeholder: "I expected the `gateway` to start and connect to the `engine`."
    validations:
      required: true
  - type: textarea
    id: environment
    attributes:
      label: "Your Environment"
      description: "Please provide any relevant details about your environment."
      placeholder: |
        - OS: [e.g., macOS Sonoma, Windows 11, Ubuntu 22.04]
        - A.R.C. Version: [e.g., v0.1.0]
        - Docker Version: [e.g., 20.10.17]
---
