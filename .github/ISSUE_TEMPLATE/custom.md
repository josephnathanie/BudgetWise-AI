---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

name: 🐛 Bug Report & Troubleshooting
description: File a bug report if the Wiki couldn't solve your issue.
title: "[BUG]: "
labels: [bug]
body:
  - type: checkboxes
    id: docs-check
    attributes:
      label: 🔍 Pre-Check Requirement
      description: Please check the documentation before submitting.
      options:
        - label: I have checked the [Official BudgetWise AI Wiki](https://github.com) and my issue or error code is not listed there.
          required: true
  - type: textarea
    id: bug-description
    attributes:
      label: Describe the bug
      placeholder: What is going wrong with the app?
    validations:
      required: true
