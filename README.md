# 🚀 Automated Commit

This repository contains a **GitHub Actions workflow** that automatically updates a file named `TIMESTAMP.txt` with the current date and time every 12 hours.  
It’s a simple example of using GitHub Actions to automate routine repository tasks.

---

## 🧭 Overview

The **Automated Commit** workflow demonstrates how to use **GitHub Actions** to keep a repository active or log automated updates.  
Specifically, this workflow:

- 🗂 Checks out the latest code from the `main` branch.  
- 🕒 Updates the `TIMESTAMP.txt` file with the current date and time.  
- 🧩 Commits the change if modifications are detected.  
- 🚀 Pushes the new commit back to the repository.

---

## ⚙️ Workflow Structure

The workflow file is defined at:

[`.github/workflows/auto-commit.yml`](.github/workflows/auto-commit.yml)

### 🔁 Triggers
- Runs automatically **every 12 hours** (`cron` schedule).  
- Can also be **manually triggered** from the GitHub Actions UI (`workflow_dispatch` event).  
- Runs **on every push** to the `main` branch.

### 🧱 Jobs and Steps
The workflow includes one main job: `update_commit`, which:
- Runs on the latest Ubuntu runner (`ubuntu-latest`).
- Sets up Git configuration.
- Updates and commits the `TIMESTAMP.txt` file.
- Pushes changes to the repository.

### 🔒 Permissions
The workflow grants `contents: write` permission so it can make commits to the repo.

---

## 🛠 Using This Workflow

### 🧩 Creating Your Own Version
To create your own copy of this automation:
1. Click **“Use this template”** on the GitHub repository page.  
2. Choose a name for your new repository.  
3. Click **“Create repository from template.”**  
4. Clone your repository locally if you want to make custom edits.

### ✏️ Customizing the Workflow
Before using, replace the Git configuration with your details:

1. Open the file `.github/workflows/auto-commit.yml`.  
2. Find this section:
   ```yaml
   git config user.email "your-email@gmail.com"
   git config user.name "your-gihub-usename"
3. Update these values with your own GitHub account details (if you forked it).
4. Commit and push your changes.

## 📊 Viewing Workflow Runs

To view the workflow history:
1. Navigate to the **Actions** tab on your repository.  
2. Select the **Automated Commit** workflow.  
3. Click any run to view details, logs, and timestamps.

---

## ▶️ Manually Triggering the Workflow

You can run the workflow manually anytime:

1. Go to the **Actions** tab.  
2. Select **Automated Commit**.  
3. Click **“Run workflow”**, choose the `main` branch, and confirm.

This is useful for testing or when you want to trigger an immediate commit instead of waiting for the next 12-hour schedule.

---

## 🤝 Contributing

Contributions are always welcome!  
To contribute:

1. **Fork** this repository.  
2. Make your changes or improvements.  
3. Submit a **Pull Request** describing your updates.

## ☕ Support & Donations

If you find this project helpful and want to support my work, you can send a small donation 🙏  
Your support helps me keep building more open-source automations like this.

💰 **EVM Address:** [**cruzl.eth**](https://etherscan.io/address/0x5629AEA7C12097bB4aF9920577Dcd5fC33D3f77e)



