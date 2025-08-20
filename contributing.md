# 🤝 Contributing Guidelines

Welcome! 👋  
Thank you for considering contributing to this project. To keep our workflow consistent and our codebase clean, please follow these guidelines.  

---

## 1️⃣ Branch Naming Convention
Branches must follow this format:  

- **Feature development** → `feature/<ticket-id>-<short-description>`  
  Example: `feature/123-add-user-login`  

- **Bug fix** → `bugfix/<ticket-id>-<short-description>`  
  Example: `bugfix/321-fix-login-crash`  

- **Hotfix (urgent production fix)** → `hotfix/<short-description>`  
  Example: `hotfix-critical-payment-bug`  

- **Chore/maintenance** → `chore/<short-description>`  
  Example: `chore/update-dependencies`  

✅ This ensures clarity and easy tracking of branches.

---

## 2️⃣ Commit Message Convention
We follow a structured commit format:  

```
<type>(<scope>): <short summary>
```

**Types:**  
- `feat` → new feature  
- `fix` → bug fix  
- `chore` → build/CI/dependencies/maintenance  
- `docs` → documentation changes  
- `style` → code style changes (no logic changes)  
- `refactor` → code restructure without changing functionality  
- `test` → adding/updating tests  

**Examples:**  
- `feat(auth): add JWT authentication`  
- `fix(user-profile): resolve avatar upload bug`  
- `chore(deps): bump React to 18.0.0`  

✅ Helps maintain a clean commit history and enables auto-generated changelogs.

---

## 3️⃣ Pull Requests (PRs)
- Use the [PR Template](.github/pull_request_template.md) when creating a PR.  
- **One PR = One task/feature/fix** → keep them small and focused.  
- Always link issues → e.g., `Closes #123`.  
- Rebase before opening PRs to avoid unnecessary merge commits.  
- Ensure CI/CD checks pass before requesting a review.  

---

## 4️⃣ Deployment Checklist
If your PR requires deployment actions, document them in the **🚀 Deployment Notes** section of the PR.  

Examples include:  
- Running database migrations  
- Installing new dependencies  
- Clearing cache  
- Restarting services  
- Running additional scripts  

---

## 5️⃣ Code Review Guidelines
- Be respectful and constructive in feedback.  
- Request changes only if they affect correctness, security, or maintainability.  
- Optional suggestions should be marked as such.  
- Approve only when:  
  - Code works as expected  
  - No unnecessary complexity is introduced  
  - Tests & documentation are updated  

---

## 6️⃣ Testing Requirements
- All new features must include relevant unit/integration tests.  
- Run tests locally before pushing:  
  ```bash
  npm test
  # or
  pytest
  ```
- CI/CD must pass before merging.  

---

## 7️⃣ Protected Branches
- `main` → Always production-ready.  
- `develop` (if used) → Stable staging branch.  

🚫 Direct commits are **not allowed**. All changes go through PRs.  

---

## ✅ Quick Checklist Before Submitting PR
- [ ] Correct branch name used  
- [ ] Commit messages follow convention  
- [ ] Code linted and formatted  
- [ ] Tests added/updated and passing  
- [ ] Documentation updated (if needed)  
- [ ] PR template filled properly  
- [ ] Deployment notes added (if applicable)  

---

By following these guidelines, we ensure a clean, consistent, and reliable workflow across the team 🚀.  