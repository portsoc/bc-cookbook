# The Bootcamp Cookbook

Welcome to the Bootcamp Cookbook! This repository serves as a workspace for us to learn Git flows, collaboration, and version control while building a collection of delicious recipes.


## Prerequisites

Before we start, ensure you have the following:
1. **Git** installed ([Download here](https://git-scm.com/downloads)).
2. A **Code Editor** (we recommend [VS Code](https://code.visualstudio.com/)).
3. A **GitHub Account**.

---

## Phase 1: Getting Set Up

If you haven't already, get this cookbook repo onto your local machine:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/portsoc/bc-cookbook.git
   ```
2. **Enter the folder:**
   ```bash
   cd bc-cookbook
   ```
3. **Open the project** in your code editor.

---

## Phase 2: The Sprint Cycle

We will be working in 15-minute sprints. Follow these steps for every single ticket you work on.

### 1. Sync Up (IMPORTANT)
Before starting **anything**, make sure your local computer has the latest version of the book.
```bash
git checkout main
git pull origin main
```

### 2. Pick an Issue
1. Go to the [Issues](https://github.com/portsoc/bc-cookbook/issues) tab in this repository.
2. Find an open task (e.g., "Add Pancake Recipe", "Ensure no recipes contain lead", `<strong\>` instead of `<b\>`).
3. **Assign yourself** to the issue so others know you are working on it.

### 3. Create a Branch
**Never work directly on the `main` branch.** Create a workspace for your specific task.
```bash
# Naming convention: feature/name-of-task
git checkout -b feature/add-pancakes
```

### 4. Sprint (Code & Commit)
Do the work required for the ticket (create the HTML file, fix the typo, remove poisonous heavy metals from ingredients). Once you are happy with your work:

```bash
git add .
git commit -m "Added basic HTML structure for pancakes"
```
*(You can do this multiple times during the sprint!)*

### 5. Test the code
Write some tests for the code in plain english.
Consider edge-cases for these tests (e.g. a person should not be able to add an empty recipe; a person should not be able to add a recipe over 100000 characters....etc.)
Verify that the code passes the tests by running the code.

### 6. Push & Pull Request
When your ticket is done:

1. **Push your branch to the cloud:**
   ```bash
   git push origin feature/add-pancakes
   ```
2. Go to the GitHub page for this repo.
3. You will see a yellow banner: **"Compare & pull request"**. Click it.
4. Write a brief description and click **Create Pull Request**.

---

## 🤝 Phase 3: Review & Stand-Up

1. **Stop Coding:** When the sprint timer ends, stop.
2. **Peer Review:** Ask another group to review your Pull Request on GitHub. They should check it is appropriate and look for things like correct HTML and typos in content.
3. **Merge:** Once approved, click **"Squash and Merge"** on GitHub.
4. **Stand-Up:** We will have a quick group sync to discuss blockers and show off new features.

---

## 🛑 Golden Rules

> **1. Never commit to `main`.** Always use a branch.
>
> **2. Always `git pull` before starting a new branch.**
>
> **3. Don't merge your own Pull Request.** Get a second pair of eyes on it.
