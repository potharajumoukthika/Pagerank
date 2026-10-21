# CS50 AI – PageRank

This project implements Google's PageRank algorithm to rank web pages by importance, as part of Harvard's CS50's Introduction to Artificial Intelligence with Python course.

## Features

- **Random Surfer Model:** Estimates PageRank by sampling pages using a Markov chain.
- **Transition Model:** Calculates the probability of visiting each page.
- **Iterative Algorithm:** Computes PageRank by repeatedly updating page scores until convergence.
- **Multiple Corpora:** Tests the implementation on three collections of HTML pages.

## Technologies

- Python 3
- Python standard library

## Project Structure

- `pagerank.py` – PageRank implementation.
- `corpus0/` – Small test corpus.
- `corpus1/` – Medium test corpus.
- `corpus2/` – Larger test corpus.

## How to Run

Run the following command from the project directory:

```bash
python pagerank.py corpus0
```

Replace `corpus0` with `corpus1` or `corpus2` to test another corpus.

## Algorithms

**Sampling:** Estimates each page's rank from the proportion of visits during random surfing.

**Iteration:** Repeatedly applies the PageRank formula until successive ranks differ by no more than 0.001.

The damping factor is 0.85, and the sampling method uses 10,000 samples by default.

## Learning Outcomes

- Understanding Markov chains and probability distributions.
- Implementing iterative algorithms and convergence.
- Working with HTML files, dictionaries, and sets in Python.
