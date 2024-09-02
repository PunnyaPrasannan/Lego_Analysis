# LEGO Parts Analysis

## Overview

This project analyzes LEGO sets and their parts to identify unique parts that appear in only one set. The analysis focuses on identifying these unique parts and categorizing them by theme, set, and year. The data is visualized in Tableau to provide a clear and interactive understanding of the distribution of parts across different LEGO sets. 

## Database Setup

To replicate this analysis, you will need a PostgreSQL database with the following tables:

1.COLORS
2.INVENTORIES
3.INVENTORY_PARTS
4.INVENTORY_SETS
5.PARTS
6.PART_CATEGORIES
7.SETS
8.THEMES

Ensure you have these tables properly set up in your PostgreSQL database.

## SQL Scripts

The SQL script provided in this repository performs the following tasks:

1. **Create a View (`unique_parts_analysis`)**: This view is created to identify unique LEGO parts that appear in only one set. It categorizes each part by theme, set name, year, and whether it is unique or not. 


2. **Query Results**: After creating the view, you can run the final `SELECT` statement to view the results of the analysis, which includes data on unique and non-unique parts by set and theme.

## Visualization

The data from the SQL analysis is visualized using Tableau to provide an interactive exploration of the unique parts across LEGO sets and themes. The Tableau dashboard includes:

- **Theme Distribution**: Visual representation of how unique and non-unique parts are distributed among different LEGO themes.
- **Set Analysis**: Detailed breakdown of unique parts by set and year, allowing users to explore specific sets and their composition.

## Results

The view `unique_parts_analysis` provides the following columns:

- `theme_name`: The name of the LEGO theme.
- `set_name`: The name of the LEGO set.
- `set_year`: The year the LEGO set was released.
- `unique_part`: Indicates whether the part is unique ('Unique') or not ('Not Unique').
- `parts`: The count of parts for each set/theme combination.

This data helps in identifying unique parts and understanding their distribution across various sets and themes.
