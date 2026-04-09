# DSF-PT15 Student Materials

Class notebooks and datasets for the **Data Science Foundations — Part-Time 15** cohort at Moringa School.

---

## Prerequisites

Before you begin, make sure you have the following installed:

- A [GitHub account](https://github.com/signup)
- [Git](https://git-scm.com/downloads) installed on your computer
- [VS Code](https://code.visualstudio.com/download) and/or [Jupyter Notebook](https://jupyter.org/install)

---

## Step 1: Fork the Repository

Forking creates **your own personal copy** of the repo under your GitHub account. This lets you work freely without affecting the original.

1. Visit the original repo:
   **https://github.com/ds-moringa-datanerds/dsf-pt15-student-materials**

2. Look at the **top-right corner** of the page. You'll see a row of buttons:
   `Watch` | `Fork` | `Star`

3. Click the **`Fork`** button

4. On the "Create a new fork" page:
   - **Owner:** Select your GitHub username
   - **Repository name:** Keep as `dsf-pt15-student-materials`
   - Click the green **"Create fork"** button

5. Done! You now have your own copy at:
   `https://github.com/YOUR-USERNAME/dsf-pt15-student-materials`

---

## Step 2: Clone Your Fork to Your Computer

Cloning downloads the repo to your local machine so you can work offline.

1. Go to **YOUR fork** on GitHub (not the original repo!)
   `https://github.com/YOUR-USERNAME/dsf-pt15-student-materials`

2. Click the green **`<> Code`** button

3. In the dropdown that appears:
   - Make sure the **`HTTPS`** tab is selected
   - You'll see a URL like: `https://github.com/YOUR-USERNAME/dsf-pt15-student-materials.git`
   - Click the **copy icon** (clipboard) next to the URL

4. Open your terminal:
   - **Windows:** Open **Git Bash** or **Command Prompt**
   - **Mac:** Open **Terminal**

5. Navigate to where you want the folder, then clone:

   ```bash
   cd Desktop
   git clone https://github.com/YOUR-USERNAME/dsf-pt15-student-materials.git
   ```

   > Replace `YOUR-USERNAME` with your actual GitHub username

6. Enter the project folder:

   ```bash
   cd dsf-pt15-student-materials
   ```

You should now have all the files on your computer!

---

## Step 3: Open in VS Code

### Option A: From the Terminal (Recommended)

```bash
cd Desktop/dsf-pt15-student-materials
code .
```

This opens the **entire project folder** in VS Code.

### Option B: From VS Code Directly

1. Open **VS Code**
2. Go to **File** > **Open Folder...** (or press `Ctrl+K Ctrl+O`)
3. Navigate to the `dsf-pt15-student-materials` folder on your Desktop
4. Click **"Select Folder"**

### Installing the Jupyter Extension (Required for Notebooks)

To run `.ipynb` notebook files inside VS Code:

1. Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on Mac) to open the **Extensions** panel
2. In the search bar, type **`Jupyter`**
3. Find the one published by **Microsoft** and click **Install**
4. Now you can open any `.ipynb` file and run it directly in VS Code!

---

## Step 4: Open in Jupyter Notebook

1. Open your terminal (**Git Bash**, **Command Prompt**, or **Terminal**)

2. Navigate to the project folder:

   ```bash
   cd Desktop/dsf-pt15-student-materials
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Your **default browser** will open automatically showing all the files in the repo

5. Click on any `.ipynb` file to open and run the notebook

> **If Jupyter is not installed**, run this first:
> ```bash
> pip install notebook
> ```

---

## Step 5: Keep Your Fork Updated

When new class materials are added to the original repo, you'll want to sync your fork to get them.

### Option A: From GitHub (Easiest)

1. Go to **your fork** on GitHub
2. If you see a banner that says *"This branch is X commits behind"*, click **"Sync fork"**
3. Click **"Update branch"**
4. Then pull the changes to your local computer:

   ```bash
   cd Desktop/dsf-pt15-student-materials
   git pull
   ```

### Option B: From the Terminal

```bash
# Navigate to your project folder
cd Desktop/dsf-pt15-student-materials

# Add the original repo as "upstream" (only needed once)
git remote add upstream https://github.com/ds-moringa-datanerds/dsf-pt15-student-materials.git

# Fetch and merge the latest updates
git fetch upstream
git merge upstream/main
```

---

## Repository Structure

```
dsf-pt15-student-materials/
├── Week3/
│   └── W3D2_TypesOfData_Student.ipynb
├── Financial_inclusion_dataset.csv
├── W3D2_TypesOfData_Student.ipynb
└── README.md
```

> More folders will be added as the course progresses.

---

## Troubleshooting

| Problem | Solution |
|---|---|
| `git` is not recognized | [Install Git](https://git-scm.com/downloads) and restart your terminal |
| `code` is not recognized | Open VS Code > Press `Ctrl+Shift+P` > Type "shell command" > Select **"Install 'code' command in PATH"** |
| `jupyter` is not recognized | Run `pip install notebook` in your terminal |
| Permission denied when cloning | Make sure you're cloning **your fork**, not the original repo |
| Can't see new class materials | Follow **Step 5** above to sync your fork |

---

## Need Help?

- **Git reference:** [git-scm.com/doc](https://git-scm.com/doc)
- **VS Code docs:** [code.visualstudio.com/docs](https://code.visualstudio.com/docs)
- **Jupyter docs:** [jupyter-notebook.readthedocs.io](https://jupyter-notebook.readthedocs.io/)
- **Still stuck?** Reach out to your facilitator or classmates!

---

**Course Website:** [ds-moringa-datanerds.github.io](https://ds-moringa-datanerds.github.io)
