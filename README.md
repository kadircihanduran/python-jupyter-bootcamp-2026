# Introduction to Python & Jupyter Notebooks
### 2026 Open Scholarship Bootcamp · One-hour hands-on workshop

Welcome! This repository contains all the materials for the **Introduction to Python and Jupyter Notebooks** session at the 2026 Open Scholarship Bootcamp. It's designed for absolute beginners — no prior coding experience required.

You will leave the session knowing how to run code in Jupyter, work with variables, lists, loops, and `if`-statements, and you'll have a small library of curated notebooks to keep exploring on your own.

---

## What's in this repo

| File | What it is |
|---|---|
| `01_live_session_intro.ipynb` | The notebook we work through together during the one-hour session. Covers all the core Python building blocks. |
| `02_madlibs_story_generator.ipynb` | After-session notebook #1 — playful. Build a Mad Libs game and a tiny choose-your-own-adventure. Introduces functions and randomness. |
| `03_data_detective.ipynb` | After-session notebook #2 — analytical. Investigate a (made-up) coffee shop's sales data and make your first charts. Includes a peek at `pandas`. |
| `CHEATSHEET.md` | A one-page reference for everything covered in the live session. Print it, save it, scribble on it. |

---

## How to run the notebooks

### Recommended: Google Colab (no installation needed)

[Google Colab](https://colab.research.google.com/) runs Jupyter notebooks for free in your browser. It is the fastest way to get started.

1. Open <https://colab.research.google.com/>.
2. Click **File → New notebook**.
3. Open the `.ipynb` file you want to work with (here on GitHub) and **copy each section into a new Colab cell**. The `# %%` lines in the file mark where one cell ends and the next begins — everything between two `# %%` markers belongs in a single Colab cell.
4. Press **Shift + Enter** to run a cell.

> *Tip:* Colab also lets you upload files directly. Click the folder icon in the left sidebar of any notebook to upload data files for the **Data Detective** notebook.

### Alternative: JupyterLab on your own computer

If you'd rather run things locally:

1. Install Python from <https://www.python.org/downloads/> (3.10 or newer).
2. Install JupyterLab and the libraries used here:
   ```bash
   pip install jupyterlab matplotlib pandas jupytext
   ```
3. Launch JupyterLab from a terminal:
   ```bash
   jupyter lab
   ```
4. In JupyterLab, **right-click** any `.ipynb` file in this repo and choose **Open With → Jupytext Notebook**. Cells will appear ready to run.

---

## What you'll learn during the session

- Navigating JupyterLab and running code cells
- Variables and the four basic data types (string, int, float, bool)
- Doing math with Python
- Working with text using strings and f-strings
- Storing collections of items in lists
- Making decisions with `if` / `elif` / `else`
- Repeating work with `for` loops
- A taste of data visualization with `matplotlib`

---

## After the session

Pick one of the follow-up notebooks based on what excited you most:

- **Liked the language part?** → `02_madlibs_story_generator.ipynb`
- **Liked the chart at the end?** → `03_data_detective.ipynb`

Each follow-up notebook is fully commented and includes practice challenges at the end. You can work through them on your own time — no instructor required.

---

## Need help?

If something doesn't make sense, that's normal. Three good first moves:

1. **Read the last line of any error message** — it usually tells you exactly what's wrong. The cheat sheet has a section on this.
2. **Restart the kernel** (Kernel → Restart Kernel) if a notebook is misbehaving.
3. **Google your error message verbatim.** Whatever's gone wrong has happened to thousands of others before you.

---

*Created for the 2026 Open Scholarship Bootcamp. Happy coding!*
