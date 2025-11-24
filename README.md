# 🧪 GitHub 101: Version Control for Our Lab

Welcome to the lab's introductory session on GitHub! This guide will help you set up your environment and understand the basics of version control without getting technical.

## ✅ Prerequisites (Complete Before Session)

To make the most of our workshop, please complete these three steps before you arrive:

1.  **Create a GitHub Account:**
    * Go to [github.com](https://github.com/) and sign up (it's free).
    * *Tip: Use a professional username (like `firstname-lastname`) if possible.*
2.  **Install the Tools:**
    * **Download VS Code:** [code.visualstudio.com](https://code.visualstudio.com/). This will be our text editor.
    * **Important:** You also need to install **Git** (the engine that powers GitHub).
        * *Windows:* Download [Git for Windows](https://gitforwindows.org/).
        * *Mac:* Open your terminal and type `git --version`. If it's not installed, your Mac will prompt you to install it.
3.  **Bring your Laptop:** We will be doing live coding!

---

## Part 1: What is this and why do we need it?

Imagine if "Track Changes" in Word and "Dropbox" were combined, but specifically designed for research code and data.

* **Git:** A tool that sits on your computer and tracks changes to your files over time.
* **GitHub:** The website where we store these files to share them with the lab.

### The Core Workflow (The "Save" Cycle)

We don't just "save" files in Git; we take snapshots.

1.  **Work:** You edit your script or data file.
2.  **Stage:** You choose which files you want to include in the snapshot (like putting items in a shopping cart).
3.  **Commit:** You take the snapshot and label it (e.g., "Added new graph").
4.  **Push:** You upload that snapshot to the website (GitHub).

---

## Part 2: Let's Get Started

### Step 1: Create a Project Folder (Repository)
In GitHub terms, a project folder is called a **Repository** (or "repo").

1.  Log into GitHub.com.
2.  Click the **+** icon in the top right corner -> **New repository**.
3.  Name it: `lab-intro-demo`.
4.  Check the box: **Add a README file**.
5.  Click **Create repository**.

### Step 2: Copy to your Computer (Clone)
We need to get that folder from the internet down to your laptop.

1.  On your new GitHub page, click the green **<> Code** button.
2.  Copy the web address (URL).
3.  Open **VS Code**.
4.  Press `F1` (or `Cmd+Shift+P` on Mac) to open the command menu.
5.  Type: `Git: Clone` and press Enter.
6.  Paste the URL you copied and select a folder on your laptop to save it.
7.  Click **Open** when prompted.

---

## Part 3: Making Changes

Now that you have the project open on your computer, let's make a change.

### 1. Edit a File
Open the file named `README.md` and add a few lines: