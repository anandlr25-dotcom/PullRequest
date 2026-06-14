# GitHub Pull Request (PR)

## Introduction

A **Pull Request (PR)** is a GitHub feature that allows developers to propose changes to a repository. It enables team members to review, discuss, and approve code before it is merged into the main branch.

A Pull Request helps maintain code quality by providing a structured review process and encouraging collaboration among developers.

---

## What is a Pull Request?

A Pull Request is a request to merge changes from one branch into another branch.

For example:

```text
feature/login-page → main
```

This means the changes made in the `feature/login-page` branch are being requested to merge into the `main` branch.

---

## Why Pull Requests Are Important

Pull Requests provide several benefits:

- Code review before merging
- Better collaboration among team members
- Discussion and feedback on code changes
- Automated testing and validation
- Improved code quality
- Better project management
- Reduced risk of bugs in production

---

## Pull Request Workflow

### Step 1: Create a New Branch

Create a separate branch for your feature or bug fix.

```bash
git checkout -b feature/new-feature
```

---

### Step 2: Make Changes

Implement the required feature, enhancement, or bug fix in your branch.

---

### Step 3: Stage Changes

Add modified files to the staging area.

```bash
git add .
```

---

### Step 4: Commit Changes

Create a commit with a meaningful message.

```bash
git commit -m "Add new feature"
```

---

### Step 5: Push Changes to GitHub

Push the branch to the remote repository.

```bash
git push origin feature/new-feature
```

---

### Step 6: Create a Pull Request

1. Open the repository on GitHub.
2. Navigate to the Pull Requests tab.
3. Click **New Pull Request**.
4. Select:
   - Base Branch: `main`
   - Compare Branch: `feature/new-feature`
5. Add a title and description.
6. Click **Create Pull Request**.

---

### Step 7: Code Review

Team members review the code and may:

- Approve the changes
- Request modifications
- Leave comments and suggestions

---

### Step 8: Address Feedback

Make the requested changes and push additional commits.

```bash
git add .
git commit -m "Fix review comments"
git push origin feature/new-feature
```

The Pull Request updates automatically.

---

### Step 9: Merge the Pull Request

Once approved:

1. Click **Merge Pull Request**
2. Confirm the merge
3. Delete the feature branch if no longer needed

---

## Pull Request Lifecycle

```text
Create Branch
      ↓
Make Changes
      ↓
Commit Changes
      ↓
Push Branch
      ↓
Create Pull Request
      ↓
Code Review
      ↓
Approval
      ↓
Merge
      ↓
Delete Branch
```

---

## Example Pull Request

### Branch

```text
feature/user-authentication
```

### Commit

```text
Implement user login functionality
```

### Pull Request

```text
feature/user-authentication → main
```

### Pull Request Title

```text
Add User Authentication Module
```

### Pull Request Description

```text
This PR adds user authentication functionality including:

- Login page
- Password validation
- Session management
- Logout functionality

Testing:
- Login tested successfully
- Logout tested successfully
- Invalid credentials handled properly
- Currrent update
```

---

## Best Practices

### Write Clear Titles

Good:

```text
Add password reset functionality
```

Bad:

```text
Changes
```

---

### Keep Pull Requests Small

Smaller Pull Requests are:

- Easier to review
- Easier to test
- Less likely to introduce bugs

---

### Write Meaningful Descriptions

Include:

- What was changed
- Why it was changed
- How it was tested

---

### Link Related Issues

Example:

```text
Closes #25
Fixes #42
```

---

### Request Reviews

Ask team members to review before merging.

---

### Ensure Tests Pass

Run tests before creating a Pull Request.

```bash
npm test
```

or

```bash
pytest
```

---

## Pull Request vs Merge Request

| Pull Request | Merge Request |
|-------------|--------------|
| Used by GitHub | Used by GitLab |
| Same purpose | Same purpose |
| Review and merge code | Review and merge code |

Both terms refer to the same concept.

---

## Common Pull Request Terms

### Base Branch

The branch receiving the changes.

Example:

```text
main
```

---

### Compare Branch

The branch containing the new changes.

Example:

```text
feature/login-page
```

---

### Reviewer

A person responsible for reviewing the Pull Request.

---

### Approval

Confirmation that the code is ready to merge.

---

### Merge

Combining changes from one branch into another.

---

## Sample Pull Request Template

```markdown
## Description

Briefly describe the changes made.

## Type of Change

- [ ] Bug Fix
- [ ] New Feature
- [ ] Documentation Update
- [ ] Refactoring

## Testing

Describe how the changes were tested.

## Screenshots

Add screenshots if applicable.

## Related Issue

Closes #123

## Checklist

- [ ] Code follows project standards
- [ ] Tests pass successfully
- [ ] Documentation updated
- [ ] Ready for review
```

---

## Advantages of Pull Requests

- Improved code quality
- Knowledge sharing
- Better collaboration
- Easier maintenance
- Safer deployments
- Clear project history
- Automated quality checks

---

## Conclusion

A Pull Request (PR) is a GitHub feature used to propose, review, discuss, and merge code changes from one branch into another. It is a critical part of modern software development workflows and helps teams maintain high-quality, reliable code through collaboration and structured code reviews.


## Updated by yashvanthbalaji
