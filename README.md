# sales-data-raw

## Overview

This repository contains a sample sales dataset (`Book1.xlsx`) that demonstrates a range of common data quality issues typically encountered in real-world business data. The purpose of this dataset is to provide a realistic starting point for practicing and demonstrating data cleaning and preprocessing techniques.

## Dataset Description

The dataset includes the following columns:
- **OrderID:** Unique identifier for each sales transaction (non-unique in this raw version).
- **Date:** The date of each transaction, in various inconsistent formats.
- **SalesPerson:** Name of the sales agent involved in the sale.
- **Amount:** The sales amount, often including currency symbols and thousands separators.
- **Product:** The product sold.
- **Region:** The geographical region of the sale.
- **Column1:** A blank column present due to mistaken export or data entry.

## Data Issues Included

This raw data file was intentionally created to simulate messy, real-world data by including the following issues:

- **Missing Values:**  
  Some records are missing values for key fields such as `SalesPerson`, `Amount`, and others.

- **Duplicate Rows:**  
  Certain rows are exact duplicates (same OrderID and all other fields), causing data redundancy.

- **Inconsistent Text Formats:**  
  - Variations in capitalization and spelling for values in fields like `Region` (e.g., "North", "north", "NORTH", "SouTH").
  - Salesperson names appear in different letter cases and sometimes with extra spaces.

- **Inconsistent Date Formats:**  
  Multiple date formats are used, including `2023-01-05`, `07-01-2023`, `20230112`, `1/6/2023`, and `8-Jan-2023`.

- **Currency and Number Formatting Issues:**  
  The `Amount` field contains mixed formatting: with and without currency symbols (`$`), commas as thousands separators, numbers as text, and sometimes as missing values.

- **Extraneous/Empty Columns:**  
  The raw data includes a completely empty column (`Column1`) resulting from a faulty export.

## Usage

This dataset can be used for:

- Practicing data cleaning and preprocessing
- Demo for data wrangling scripts or courses
- Benchmarking data preparation tools

**WARNING:** Do not use this file for reporting or analytics until it has been thoroughly cleaned!

---

## Files

- `sales-data-raw.xlsx` — Original, uncleaned sales dataset

