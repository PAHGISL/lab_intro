# 💬 Q&A: Lab GitHub Discussion

We gathered some great questions and insights from the team. Here are the detailed responses to help clarify our workflow.

---

## 🏗️ Topic 1: Structure & Organization

**Q: What do you think is most important for the lab-wise GitHub repository site?**

> • Good folder structure with easily interpretable names – e.g. project (for deliverable grant outputs), data (code/guides to access data), functions (split further into more specific topics e.g. modelling), packages or pipelines (if complete)

**Response:**
Agreed. A consistent folder structure is critical so anyone can open a project and know where to look. We recommend the following standard "Tiered" structure for our repositories:

- `project-name/`
  - `data/` (🛑 RAW data - Read-only, never edit manually)
  - `output/` (📉 Graphs and processed tables)
  - `src/` (🐍 Scripts and source code - Python/R)
    - `processing/` (Scripts to clean data)
    - `analysis/` (Scripts to model/graph data)
  - `docs/` (📄 Manuscripts or detailed guides)
  - `.gitignore` (🙈 Tells Git what to ignore)
  - `README.md` (📖 The "Landing Page" explaining the project)

> • Consistent file names (e.g. underscore, capitals, upper/lower camel case, how many words allowed etc.)

**Response:**
We should adopt a **"snake_case"** rule (lowercase with underscores) for all file names.
- **Why?** Windows is case-insensitive, but Linux/Mac are not. Using mixed cases (like `DataProcessing.R` vs `dataprocessing.R`) often causes code to crash when moving between computers.
- **Rule:** `my_script_name.py` (✅) vs `My Script Name.py` (❌).

> • Clear distinctions for scripts/code files which are designed to be used

**Response:**
We can handle this by using a numbering system in the filename or a specific folder.
- Example: `01_clean_data.py` implies it is the first step.
- Example: `dev_testing.py` implies it is just for testing.

---

## 🤯 Topic 2: "It feels overwhelming!"

**Q: What part have you been most confused with GitHub?**

> • how to access the lab GitHub, how to upload files in the right structure (file vs page??), best way to access files (fork/pull?) and share files (keep a master file in personal repository and fork into lab repository?)

**Response:**
- **File vs Page:** In GitHub, everything is stored as a file. However, if you name a file `.md` (Markdown), GitHub renders it to look like a webpage.
- **Fork vs Branch:**
    - **Forking:** Copying a project to your *personal* account. (Good for open source, distinct separation).
    - **Branching:** Creating a workspace *inside* the lab's repository. (Better for close collaboration).
    - **Recommendation:** We will start with **Branching**. It keeps everything in one place and is easier to manage.

> • It appears very overwhelming for a complete novice – what does push, pull, commit, forking etc. mean? How do we use this day-to-day? Or should we only be using GitHub to publish ready-to-use code to share with others? 

**Response:**
- **Day-to-day:** Please do **not** wait for code to be perfect! Use GitHub as a daily "Save" button. If you mess up your code on Tuesday, you can revert to Monday's version instantly.
- **Simple Dictionary:**
    - **Clone:** Download to laptop.
    - **Commit:** Save snapshot.
    - **Push:** Upload to cloud.
    - **Pull:** Download updates from cloud.

---

## 🛡️ Topic 3: Insights & Experience

**Q: Any other thoughts?**

> • I have no idea how to GitHub but many are experts, so perhaps a beginners meeting first so time is not wasted

**Response:**
That is exactly the purpose of this upcoming session! We assume zero prior knowledge.

> • I’d like to learn something about the unit test, how it works, and how to implement it. Anyone can share? (Yuxi)

**Response:**
Unit testing is excellent for reproducibility (ensuring your function always gives the correct answer).
- **Plan:** Since this is an intermediate/advanced topic, we will schedule a specific "Level 2" session on `pytest` (Python) and `testthat` (R) once everyone is comfortable with the basics of pushing/pulling code.

> • I used it for a while but not an expert. My experience is never putting any confidential information on your repository. Once it is committed and pushed, it can never be removed safely even if you delete the entire repository. There might be some solutions to remove a few files completely from the repository history. That was very complex, and I tried but didn’t success. That is why the `.gitignore` file is so useful - it can hide files you specify from being committed. Anyway, always check to ensure the files you committed do not contain any confidential information. (Yuxi)

**Response:**
**This is the most important security rule.**
- If you accidentally upload a password or API key, it stays in the history *forever* (even if you delete the file later).
- **Solution:** We will cover how to use `.gitignore` in the first 10 minutes of the workshop. This file acts as a "bouncer" that stops passwords and large data files from ever entering the repository.

> • As for user interfaces, I used SourceTree and GitHub Desktop. Both are good, but there might be new tools in recent years. (Yuxi)

**Response:**
Those are both great tools. For this workshop, we will use **Visual Studio Code (VS Code)**.
- **Reason:** VS Code has the Git buttons built directly into the editor. This means you don't have to switch windows to save your work, making the workflow much simpler for beginners.