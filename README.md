# Student Management System - MongoDB Dataset

This project contains a dataset and basic scripts for managing student records, originally structured for **MongoDB** and exported to **CSV** format for analysis and migration purposes.

## Overview

The repository features a collection of student data, including unique identifiers, names, ages, and their respective academic programs. This is a typical example used for practicing **NoSQL database operations**, data cleaning, and exploratory data analysis (EDA).

## Dataset Structure

The primary data is stored in `BD_CursoMongo.Estudiantes.csv`. The schema includes:

| Column | Description |
| :--- | :--- |
| `_id` | Unique MongoDB Hexadecimal Identifier |
| `nombre` | Full name of the student |
| `edad` | Student's age |
| `carrera` | Academic major / Program |

## Key Features

* **Data Cleaning:** Handles inconsistencies in naming conventions (e.g., "Ciencia de datos" vs "Ciencia de Datos").
* **Schema Validation:** Example of how MongoDB documents are structured before being flattened into CSV.
* **Query Practice:** Ideal for practicing **SQL** (via SQLite/PostgreSQL) or **NoSQL** (via MongoDB Compass/Shell) queries.

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. **Import to MongoDB:**
   You can import the CSV file directly using `mongoimport`:
   ```bash
   mongoimport --db SchoolDB --collection Students --type csv --headerline --file BD_CursoMongo.Estudiantes.csv
   ```
3. **Data Analysis:**
   Load the file in Python using **Pandas** for quick insights:
   ```python
   import pandas as pd
   df = pd.read_csv('BD_CursoMongo.Estudiantes.csv')
   print(df.head())
   ```

## Author

David Ricardo Castro Gonzalez
