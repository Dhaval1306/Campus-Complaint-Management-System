# Team Contribution & Workflow Guide

Follow this guide to contribute to the **Campus-Complaint-Management-System**.

---

### Step 1: Fork the Main Repository
1. Visit the main project repository: [TakshChauhan/Campus-Complaint-Management-System](https://github.com/TakshChauhan/Campus-Complaint-Management-System).
2. Click the **Fork** button (top-right) to create your own copy under your GitHub account.

---

### Step 2: Clone Your Fork
Clone your personal fork to your local machine:
```bash
git clone https://github.com/<YOUR-USERNAME>/Campus-Complaint-Management-System.git
cd Campus-Complaint-Management-System
```

Configure upstream remote to stay in sync with the main project:
```bash
git remote add upstream https://github.com/TakshChauhan/Campus-Complaint-Management-System.git
```

---

### Step 3: Create a Working Branch
Always branch off the latest `main`:
```bash
# Sync local main with upstream
git checkout main
git pull upstream main

# Create and switch to your feature/task branch
git checkout -b feature/<task-name>
```
*(Example: `git checkout -b feature/auth-api` or `feature/login-ui`)*

---

### Step 4: Make Changes & Commit
Stage your files and write a clear, descriptive commit message:
```bash
git add .
git commit -m "Brief description of changes"
```

---

### Step 5: Push to Your Fork
Push your branch to your GitHub fork (`origin`):
```bash
git push -u origin feature/<task-name>
```

---

### Step 6: Create a Pull Request (PR)
1. Go to your fork on GitHub or the main repository: [TakshChauhan/Campus-Complaint-Management-System](https://github.com/TakshChauhan/Campus-Complaint-Management-System).
2. Click **Compare & pull request**.
3. Verify the branches:
   - **Base repository**: `TakshChauhan/Campus-Complaint-Management-System` (`main`)
   - **Head repository**: `<YOUR-USERNAME>/Campus-Complaint-Management-System` (`feature/<task-name>`)
4. Add a title and description summarizing your work.
5. Click **Create pull request** and notify the team lead.

---

### 💡 Quick Syncing Tip
Before starting new work, always pull latest changes from upstream:
```bash
git checkout main
git pull upstream main
git push origin main
```
