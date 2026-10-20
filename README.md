# Smart-City-Traffic-Flow-Simulator

Smart City Traffic Flow Simulator 🚦

A beginner-friendly NumPy project that simulates 30 days of hourly vehicle counts for 10 junctions, highlights rush-hour patterns, finds high-traffic periods, and compares loop-based and vectorized calculations.

Important: All data is synthetic and generated for learning purposes. It does not represent real-world traffic data.

🌟 Project Features

Reproducible Synthetic Data: Uses np.random.seed(42) to ensure identical outputs on every run.

Dataset Size: 30 days × 10 junctions × 24 hours = 7,200 junction-hour records.

Rush-Hour Modeling: Simulates realistic morning (08:00) and evening (18:00) peak patterns.

Axis-wise Aggregation: Demonstrates sum and mean calculations along specific axes, using np.argmax() for peak detection.

Data Visualizations: Includes bar charts for total junction traffic, average hourly traffic line plots, and a junction-vs-hour heatmap.

Performance Benchmarking: Quantifies performance differences between standard Python loops and NumPy vectorization.

High-Traffic Analysis: Simple automatic reporting of high-density traffic junctions.

💡 How It Works

Rush-Hour Curve: Creates a base traffic intensity distribution peaking near 08:00 and 18:00.

Poisson Data Generation: Uses a Poisson distribution (np.random.poisson) to generate realistic, non-negative integer vehicle counts.

Array Analysis: Computes totals and averages by junction and hour; utilizes np.argmax() to locate maximum traffic occurrences.

Data Visualization: Generates plots using Matplotlib to visualize patterns and traffic density heatmaps.

Runtime Benchmarking: Compares execution times of nested Python loops against vectorized np.sum() operations.

📂 File Structure

Smart_City_Traffic_Flow_Simulator.ipynb — Complete, runnable Jupyter/Google Colab notebook.

README.md — Project documentation and setup guide.

🚀 Getting Started

Option 1: Run in Google Colab

Download Smart_City_Traffic_Flow_Simulator.ipynb.

Open Google Colab.

Navigate to File → Upload notebook and upload the .ipynb file.

Go to Runtime → Restart session and run all (or Runtime → Run all).

View charts, summaries, and benchmarking timing results.

(Optional) Save a copy to your Google Drive or export to GitHub.

Option 2: Run Locally

Install required libraries:

python -m pip install numpy matplotlib jupyter


Launch Jupyter Notebook:

jupyter notebook Smart_City_Traffic_Flow_Simulator.ipynb


🧠 Concepts Practiced

NumPy Core: Multi-dimensional arrays, np.random.poisson, array reshaping, and broadcasting.

Aggregations: np.sum(axis=...), np.mean(), and index-location via np.argmax().

Data Visualization: Matplotlib (bar plots, line charts, and heatmaps).

Optimization: Python loops vs. NumPy vectorization and execution time measurement.

📝 Resume Bullet Point

Built a reproducible NumPy traffic simulator generating 7,200 synthetic junction-hour records with morning and evening rush-hour peaks; identified high-traffic junctions and peak hours using axis-wise aggregation and argmax(), and benchmarked loop-based versus vectorized calculations.


📌 Checklist Before Sharing

[ ] Execute all cells in the notebook so outputs, graphs, and execution times are saved.

[ ] Push the updated .ipynb and README.md to GitHub.

[ ] Replace YOUR_USERNAME and YOUR_REPOSITORY in the Open in Colab badge link above.

[ ] Update any placeholders in your documentation with measured runtime values (e.g., speedup factor).
