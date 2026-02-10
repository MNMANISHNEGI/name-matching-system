# Name Matching System (Task-1)

## Overview

This project implements a **name matching system** that finds the most similar names from a dataset when a user inputs a name.

It uses **RapidFuzz**, a fast and accurate fuzzy matching library, to compute similarity scores and return ranked matches.

This system simulates real-world use cases such as:

* KYC verification
* Customer search
* Autocomplete systems
* Record matching

---

## Features

* Dataset with 30+ similar names
* Finds best match for user input
* Returns ranked list of similar names
* Displays similarity scores
* Fast and lightweight
* Runs locally on any Windows/Linux laptop

---

## Technology Used

* Python 3.8+
* RapidFuzz
* Jupyter Notebook

---

## Project Structure

```
name-matching-system/
│
├── name_matching.ipynb
├── requirements.txt
└── README.md
```

---

## Installation

Install dependencies:

```
pip install -r requirements.txt
```

Or install directly:

```
pip install rapidfuzz
```

---

## How to Run

Open the notebook:

```
jupyter notebook name_matching.ipynb
```

Run all cells.

Enter a name when prompted.

---

## Example Input

```
gi
```

---

## Example Output

```
Best Match:
Gita -> 100

Ranked Matches:
Gita -> 100
Gitu -> 100
Gitika -> 100
Gitanshi -> 100
Gitanjali -> 100
```

---

## How It Works

The system:

1. Stores a dataset of names
2. Accepts user input
3. Computes similarity score using RapidFuzz
4. Ranks names by similarity
5. Returns best match and top results

---

## Similarity Method

Uses hybrid matching strategy:

* Prefix matching (highest priority)
* Substring matching
* Fuzzy similarity scoring

This improves accuracy, especially for short inputs.

---

## Verification Steps

To verify locally:

1. Install Python
2. Install RapidFuzz
3. Run notebook
4. Enter test input like:

```
Geeta
```

5. Verify correct match is returned

---

## Sample Dataset

Example names:

```
Geetha
Gita
Gitu
Geeta
Gitika
Gitanshi
Gitanjali
Geetanjali
```

---

## Use Cases

* Banking KYC name matching
* Customer database search
* Identity verification
* Autocomplete systems

---

## Runs Fully Locally

This project runs completely locally and does not require internet or external APIs.
