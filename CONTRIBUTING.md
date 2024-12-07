# Contribution Guide

Welcome to the **Field Day Project**! This guide will walk you through the process of contributing to our repositories, ensuring a smooth and efficient workflow.

## Overview

The **2024 Capstone team** will be working on these repositories:

- [Desktop Data Manager](https://github.com/Field-Day-2022/desktop-data-manager)
- [Mobile Data Collector](https://github.com/Field-Day-2022/mobile-data-collector)

### Key Issue

The team has forked the main repositories and tweaked the backend values to utilize their own test environment. The goal is to smooth out that part of the process, but for now, this process is designed to prevent accidental overwrites and ensure meaningful contribution chunks. Although the team has already forked the repositories, it is recommended to fork a fresh copy to make polished contributions. You can give this fork a different name to avoid confusion (e.g., `ddm-contributions`). You can replace local-folder-name with the name of your choice.

## Contribution Workflow

### 1. Fork the Repository
- Navigate to the main repository you want to contribute to.
- Click the **Fork** button to create your own copy of the repository.

### 2. Clone the Forked Repository
~~~
git clone <your-forked-repo-url> <local-folder-name>
cd <local-folder-name>
~~~

### 3. Create a Feature Branch
- Ensure you're on the `dev` branch of your forked repository:
~~~
git checkout dev
~~~
- Pull the latest changes from the original repository to stay up-to-date:
~~~
git remote add upstream <original-repo-url>
git pull upstream dev
~~~
- Create a new branch for your feature or fix:
~~~
git checkout -b feature/<short-description>
~~~

### 4. Apply Your Changes
- Manually apply your changes to a copy of the main branch from the original repository.
- Follow these guidelines:
  - Focus on one feature or fix per branch.
  - Avoid bundling multiple changes in a single branch.

### 5. Test Your Changes
- Ensure your changes work as expected.
- Run any tests available to verify functionality.

### 6. Commit Your Changes
- Use meaningful commit messages. For example:
~~~
git add .
git commit -m "Refactor: Replace hardcoded backend with dynamic config"
~~~

### 7. Push Your Feature Branch
~~~
git push origin feature/<short-description>
~~~

### 8. Create a Pull Request (PR)
- Navigate to your forked repository on GitHub.
- Click on **Compare & pull request**.
- Choose the appropriate base repository and branch (main repository's `dev` branch).
- Provide a clear title and description for the PR, including:
  - A brief summary of the changes.
  - Any related issue numbers (if applicable).

## PR Best Practices

- Keep PRs small and focused (one feature or fix per PR).
- Clearly explain why the change is necessary.
- Request reviews from other team members for feedback.

## Additional Notes

1. **Branch Naming Convention**
   - Use descriptive and consistent branch names:
     - Example: `feature/dynamic-backend-config`, `fix/login-bug`.

2. **Code Style**
   - Follow the existing coding style in the repository.
   - Use linters or formatters if available.

3. **Review and Respond**
   - Address all feedback in the PR review process promptly.
   - Ensure all requested changes are implemented before merging.

## Support

If you have any questions or encounter issues during the contribution process, feel free to reach out to [Ian Skelskey](https://www.github.com/IanSkelskey).

By following this guide, you'll help maintain a clean and collaborative workflow. We look forward to your contributions!