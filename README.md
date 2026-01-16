# Exploratory Data Analysis Project

This repository contains a Jupyter Notebook focused on exploratory data analysis using various SQLite databases for learning data science concepts.

## Project Overview

The project includes analysis of multiple datasets stored in SQLite databases, covering various topics such as:

- Anscombe's quartet
- Car crashes data
- Diamond dataset
- Flight information
- FMRI data
- Iris dataset
- MPG (Miles Per Gallon) data
- Planets data
- Tips dataset
- Titanic dataset

## Project Structure

- `Exploratory Data Analysis.ipynb`: Main Jupyter notebook containing the analysis
- `SQLite_databases_for_learning_data_science/`: Directory containing various SQLite databases used in the analysis
- `requirements.txt`: List of Python packages required for this project

## Tools and Technologies

- Python (3.x recommended)
- Jupyter Notebook
- SQLite
- Data Analysis libraries (Pandas, Plotly, etc.)

## Installation Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/jorgermzg15/exploratory-data-analysis.git
   cd exploratory-data-analysis
   ```

2. Create a virtual environment:
   ```bash
   # On macOS/Linux
   python -m venv .venv
   source .venv/bin/activate

   # On Windows
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

5. Open `Exploratory Data Analysis.ipynb` in your browser and start exploring!

## Troubleshooting

If you encounter any issues:

1. Make sure your virtual environment is activated (you should see `(.venv)` in your terminal)
2. Try upgrading pip before installing requirements:
   ```bash
   pip install --upgrade pip
   ```
3. If you have problems with any visualization, make sure Plotly is properly installed:
   ```bash
   pip install plotly --upgrade
   ```

## Database Credits

The SQLite databases used in this project are sourced from the [SQLite Databases for Learning Data Science](https://github.com/davidjamesknight/SQLite_databases_for_learning_data_science) repository by David James Knight.

## Using GitHub Codespaces (recommended for students)

This repository includes a `.devcontainer` configuration so Codespaces (or VS Code Remote - Containers) will automatically prepare a ready-to-use development environment.

How it works:

- When a student opens the repository in GitHub Codespaces, Codespaces will build the container using the provided `Dockerfile` and `devcontainer.json`.
- After the container is built, the `postCreateCommand` runs `pip install -r requirements.txt` to install all Python dependencies.
- The Codespace will have the Python and Jupyter extensions installed and port 8888 forwarded so students can run Jupyter Notebook or JupyterLab and open notebooks directly.

What students need to do:

1. Click the green "Code" button on the repository page and select "Open with Codespaces" -> "New codespace" (or use the Codespaces UI if provided by your organization).
2. Wait a few minutes for the container build and dependencies installation to complete. The first build may take longer.
3. Once the Codespace is ready, run the notebook server from the terminal:

```bash
# Start Jupyter Notebook
jupyter notebook --ip=0.0.0.0 --no-browser --port=8888
```

Or use the VS Code Command Palette: `> Jupyter: Create New Blank Notebook` and open `Exploratory Data Analysis.ipynb`.

Notes:

- If you update `requirements.txt`, Codespaces users can rebuild the container or re-run the `postCreateCommand` manually to pick up changes.
- For heavy packages you might want to pre-build a Codespaces image for your organization to speed up student start times (optional).

