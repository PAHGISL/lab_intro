# 🌿 GitHub 102: Working Together (Branches)

Now that you know how to save your own work, how do we work on the same project without overwriting each other's code?

We use **Branches**.

## What is a Branch?

Think of the `main` branch as the **Published Final Report**. It should always be clean and working.

When you want to work on something new, you don't touch the Final Report directly. You create a **Duplicate Copy** (a Branch) to work on safely.
* If you make a mistake in your branch, the main project is safe.
* If two people work on different branches, they won't block each other.

---

## The Task: Create Your Own Workspace

We are going to create a branch using your **UniKey** so we can identify who is working on what.

### Step 1: Create your Branch
1.  Open our `lab-intro` project in VS Code.
2.  Look at the very **bottom-left corner** of the VS Code blue bar. You should see the word `main` (or `master`) next to a little graph icon.
3.  Click on `main`. A menu will pop up at the top.
4.  Select **+ Create new branch...**
5.  **Name it:** Type your **UniKey** (e.g., `yiyu0116`) and press Enter.

*Result:* Look at the bottom-left corner again. It should now show your UniKey. You are now working in your own parallel universe!

### Step 2: Make a Change "Safely"
Now that you are in your own branch, you can do anything you want without breaking the main code.

1.  Create a new file named `[your_uni_id].txt` (e.g., `yiyu0116.txt`).
2.  Inside, write one sentence about your current research focus.
3.  Save the file.

### Step 3: Save your Snapshot (Commit)
Just like before:
1.  Go to the **Source Control** tab (left sidebar).
2.  Click the **+** to stage the changes.
3.  Type a message: `Created my personal text file`.
4.  Click **Commit**.

### Step 4: Publish your Branch (Push)
Your branch currently only exists on your laptop. We need to send it to GitHub so the team can see it.

1.  Click the blue button that says **Publish Branch** (usually where the Sync button was).
2.  If asked, select "origin" (this just means the cloud version).

---

## Part 4: Bringing it all together (Pull Requests)

Now your work is on GitHub, but it's still separate from the "Final Report" (`main`). To combine them, we use a **Pull Request (PR)**.

*Plain English translation: "I have finished my draft. Please pull my changes into the main folder."*

1.  Go to the GitHub website for our repository.
2.  You should see a yellow banner saying **"Compare & pull request"**. Click it.
    * *(If you don't see it, click the "Pull requests" tab -> "New pull request" -> select your branch).*
3.  Give it a title (e.g., "Adding Jdoe's research summary").
4.  Click **Create pull request**.

🎉 **Success!** You have now formally requested to merge your work into the lab's main project. In a real scenario, I (or a colleague) would review your code here before accepting it.

---

## Summary Checklist
* [ ] Created a branch with my UniKey.
* [ ] Made changes safely in that branch.
* [ ] Published (Pushed) the branch to GitHub.
* [ ] Opened a Pull Request on the website.