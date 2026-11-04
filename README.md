# Video Game Sales Data Analysis

## Project Overview

This project focuses on analyzing video game sales data using Python and data analytics libraries. The objective is to explore global video game sales, identify popular gaming genres and platforms, analyze regional sales performance, and understand publisher market share.

The project uses data analysis and visualization techniques to extract meaningful insights from video game sales records.

## Objectives

- Perform data cleaning and preprocessing.
- Explore and understand the video game sales dataset.
- Analyze sales performance across different gaming genres.
- Compare sales across North America, Europe, Japan, and other regions.
- Identify the top-performing video games.
- Calculate the market share of leading game publishers.
- Visualize sales trends and patterns using graphs and charts.

## Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook / Google Colab | Development environment |

## Dataset Description

The dataset contains 25 video game records and 11 columns.

| Column | Description |
|---|---|
| Rank | Global sales ranking |
| Name | Video game title |
| Platform | Gaming platform |
| Year | Release year |
| Genre | Game category |
| Publisher | Game publishing company |
| NA_Sales | Sales in North America |
| EU_Sales | Sales in Europe |
| JP_Sales | Sales in Japan |
| Other_Sales | Sales in other regions |
| Global_Sales | Total worldwide sales |

**Sales units:** Millions of copies.

## Project Workflow

### 1. Data Loading and Exploration
- Imported the required Python libraries.
- Loaded the video game sales dataset.
- Examined the first and last five records.
- Checked dataset dimensions, column names, and data types.
- Generated descriptive statistics for numerical and categorical columns.

### 2. Data Cleaning and Preprocessing
- Checked for missing values.
- Removed rows containing missing values, where applicable.
- Verified and corrected data types.
- Checked the consistency between regional sales and global sales.

### 3. Exploratory Data Analysis (EDA)

Performed analysis on:

- Video game sales by genre.
- Regional sales distribution.
- Top-selling video games.
- Publisher market share.
- Platform distribution.
- Sales comparisons across different geographical regions.

### 4. Data Visualization

Used Matplotlib and Seaborn to create visual representations, including:

- Bar charts for genre-wise sales.
- Regional sales comparison charts.
- Top-selling video game charts.
- Publisher market share visualizations.
- Comparative sales analysis.

## Key Findings

### 1. Total Sales by Genre

Based on the selected dataset:

| Genre | Global Sales (Millions) |
|---|---:|
| Sports | 160.46 |
| Platform | 119.48 |
| Misc | 76.70 |
| Role-Playing | 72.45 |
| Racing | 59.24 |
| Shooter | 43.07 |
| Action | 42.21 |
| Puzzle | 30.26 |
| Simulation | 24.77 |

**Insight:** Sports is the highest-performing genre, followed by Platform and Misc.

### 2. Regional Market Analysis

| Region | Top Genre | Sales (Millions) |
|---|---|---:|
| North America | Sports | 75.27 |
| Europe | Sports | 56.65 |
| Japan | Platform | 21.55 |

**Insight:** Sports games lead in North America and Europe, whereas Platform games have the highest sales in Japan.

### 3. Publisher Market Share

Top five publishers based on the calculated market share:

| Publisher | Market Share |
|---|---:|
| Nintendo | 83.71% |
| Take-Two Interactive | 6.71% |
| Microsoft Game Studios | 3.47% |
| Activision | 2.35% |
| Blizzard Entertainment | 1.45% |

**Insight:** Nintendo has the largest share of global sales within this selected dataset.

### 4. Dataset Statistics

- Total records: 25
- Total columns: 11
- Unique game titles: 25
- Unique platforms: 10
- Unique genres: 9
- Unique publishers: 8
- Missing values: 0 after cleaning

## Project Structure

```text
Video-Game-Sales-Analysis/
│
├── Video_Game_Sales_Analysis.ipynb
├── README.md
└── dataset.csv
```

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/your-
