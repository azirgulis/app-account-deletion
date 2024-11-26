---
name: Account Deletion Requests
about: Use this form to request deletion of your account
title: ''
labels: ''
assignees: ''

---

title: "Account Deletion Request"
labels: ["account-deletion"]
body:
  - type: markdown
    attributes:
      value: |
        # Account Deletion Request Form
        Please fill out this form to request deletion of your account.
  - type: input
    id: email
    attributes:
      label: Email Address
      description: Enter the email address associated with your account
      placeholder: example@email.com
    validations:
      required: true
  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      description: Please confirm the following
      options:
        - label: I want to permanently delete my account and all associated data
          required: true
        - label: I understand this action cannot be undone
          required: true
        - label: I am the owner of this account
          required: true
  - type: markdown
    attributes:
      value: |
        Note: Your request will be processed within 30 days. You will receive a confirmation email once your account has been deleted.
