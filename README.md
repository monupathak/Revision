# Revision

A structured collection of revision notebooks for **Artificial Intelligence (AI)**,
**Machine Learning (ML)**, **Natural Language Processing (NLP)**, and
**Reinforcement Learning (RL)**.

The repository is intended for learning, reviewing concepts, and keeping small
implementations and experiments in one place. Each notebook should focus on one
idea and should be easy to run, read, and revisit.

## Repository Structure

```text
Revision/
├── AI/                 # Search, representation, reasoning, and planning
├── ML/                 # Core machine learning algorithms and evaluation
├── NLP/                # Text processing, embeddings, sequence models, and transformers
├── RL/                 # Reinforcement learning algorithms and deep RL
├── common/
│   ├── datasets/       # Small shared datasets or dataset notes
│   ├── utilities/      # Reusable helper code
│   └── references/     # Papers, links, books, and reference notes
├── README.md
└── requirements.txt
```

Each subject is divided into numbered folders. The numbers show a suggested
learning and revision order. Project folders contain larger demonstrations that
combine multiple concepts.

See the README in each subject folder for its topic map:

- [AI](AI/README.md)
- [ML](ML/README.md)
- [NLP](NLP/README.md)
- [RL](RL/README.md)

## Notebook Naming

Use a number, a short topic name, and the `.ipynb` extension:

```text
01_linear_regression.ipynb
02_decision_trees.ipynb
03_attention_mechanism.ipynb
```

Use lowercase `snake_case` names. Keep one primary topic per notebook and place
related notebooks in the appropriate numbered folder.

## Recommended Notebook Format

Each notebook should generally include:

1. A short explanation of the concept
2. Imports and setup
3. A small, reproducible example
4. The implementation or experiment
5. Results and interpretation
6. A brief summary of key points

Prefer small datasets or documented public datasets. Avoid committing secrets,
large generated files, model checkpoints, or duplicate datasets.

## Setup

Create and activate a virtual environment, then install the shared dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Open the repository in VS Code or start Jupyter:

```bash
jupyter lab
```

Add a dependency to `requirements.txt` only when it is used by multiple
notebooks or is part of the repository's shared setup. Notebook-specific
dependencies should be documented in that notebook.

## Contribution Guidelines

- Keep notebooks focused and runnable from top to bottom.
- Add explanatory markdown around non-obvious code.
- Use deterministic seeds where reproducibility matters.
- Keep generated outputs and large artifacts out of version control.
- Place new material in the correct subject and numbered topic folder.
