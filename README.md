# CODE100 Final Berlin Challenge Solution

Welcome to my solution for the CODE100 final challenge! I am excited to apply as a challenger for the WeAreDevelopers World Congress in Berlin on July 17-19, 2024. This repository contains my solution to determine how many points from a given dataset fall within the black regions of the "100" logo.

## Challenge Overview

To qualify for the CODE100 final, we are required to solve a puzzle that involves analyzing a dataset containing a coordinate system and numerous points. The objective is to identify which of these points lie within the black regions of the "100" logo, as illustrated below:

[Logo Illustration](https://puzzles.code100.dev/puzzles/100hits/) 

## Project Structure

- `main.py`: The main script that processes the dataset and identifies the points within the black regions.
- `requirements.txt`: The dependencies required for the project.

## How It Works

### 1. Vertical Bar of "1"

The vertical bar is defined by the following ranges:
- **Horizontal range**: `145 <= x <= 165`
- **Vertical range**: `75 <= y <= 225`

### 2. First "0"

The first "0" is a ring centered at `(250, 150)` with:
- **Inner radius**: `55 units`
- **Outer radius**: `75 units`

### 3. Second "0"

The second "0" is a ring centered at `(410, 150)` with:
- **Inner radius**: `55 units`
- **Outer radius**: `75 units`

### Algorithm

1. **Load Data**: The coordinates are loaded from `dataset.csv`or I loaded directly.
2. **Define Regions**: The function `bpixels` determines if a point lies within any of the black regions.
3. **Apply Function**: The function is applied to each point in the dataset.
4. **Filter and Count**: Points meeting the criteria are filtered, and their count is reported.

## Dependencies

The project requires the following Python library:
- `pandas`

Install the dependencies using:
```bash
pip install -r requirements.txt
