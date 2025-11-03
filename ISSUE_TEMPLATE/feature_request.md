---
name: "✨ Feature Request"
description: "Suggest an idea for a new feature or an enhancement."
title: "[FEAT]: "
labels: ["enhancement"]
body:
  - type: markdown
    attributes:
      value: "Thank you for suggesting an idea! We appreciate your feedback."
  - type: textarea
    id: related-problem
    attributes:
      label: "Is your feature request related to a problem?"
      description: "A clear description of what the problem is. Ex. I'm always frustrated when..."
      placeholder: "It's difficult to manage... because..."
  - type: textarea
    id: solution
    attributes:
      label: "What is your suggested solution?"
      description: "A clear and concise description of what you want to happen."
      placeholder: "I propose we add a new command `arc logs` that automatically...`"
    validations:
      required: true
  - type: textarea
    id: alternatives
    attributes:
      label: "Alternatives you've considered"
      description: "A clear description of any alternative solutions or features you've considered."
  - type: textarea
    id: context
    attributes:
      label: "Additional Context"
      description: "Add any other context, mockups, or screenshots about the feature request here."
---
