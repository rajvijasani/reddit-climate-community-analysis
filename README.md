# Reddit Climate Community Analysis

A framework for detecting and tracking micro-communities in the r/climatechange subreddit using NLP, graph construction, and temporal analysis.

## Overview
Even within a single subreddit, users form smaller groups with distinct language patterns and thematic focus. This project identifies those micro-communities by analyzing one year of Reddit data (2023) and tracks how they evolve month by month.

## Methods
1. **Data collection** — Posts and comments from r/climatechange collected via Reddit API; users connected based on co-appearance within the same thread
2. **Text embeddings** — OpenAI text embedding large model to encode semantic and tonal information from each user's posts
3. **Clustering** — K-means clustering into 3 micro-communities per month; embeddings aggregated at the monthly level
4. **Keyword extraction** — TF-IDF and KeyBERT used to profile each cluster's thematic focus
5. **Temporal analysis** — Sankey diagram and monthly network graphs to track community movement and membership shifts over 12 months

## Language
Python (Jupyter Notebook)

## Files
- `Microcommunities_final.ipynb` — main analysis notebook
- `A Framework for Detecting Micro-communities on Popular Subreddits.pdf` — full writeup
- `Outputs/` — generated network graphs and visualizations

## Data
Collected via Reddit API (not included due to terms of service restrictions).
