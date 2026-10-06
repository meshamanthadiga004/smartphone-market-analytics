# Data dictionary

The dataset (`cellphone_data.csv`) was provided as part of MBA coursework and is not included in this repository. This file documents its structure so the analysis can be followed or reproduced with a dataset of the same shape.

- **Rows:** 990
- **Columns:** 22
- **Grain:** one row per customer rating of a phone model, joined with device specifications and buyer demographics.

## Columns

| Column | Type | Description |
|---|---|---|
| `user_id` | integer | Customer identifier |
| `cellphone_id` | integer | Phone model identifier |
| `rating` | integer | Customer's rating of the phone |
| `brand` | text | Phone brand (10 brands, e.g. Apple, Samsung, Xiaomi) |
| `model` | text | Phone model name |
| `operating system` | text | Android or iOS |
| `internal memory` | integer | Storage in GB |
| `RAM` | integer | RAM in GB |
| `performance` | decimal | Performance score of the device |
| `main camera` | integer | Rear camera resolution in MP |
| `selfie camera` | integer | Front camera resolution in MP |
| `battery size` | integer | Battery capacity in mAh |
| `screen size` | decimal | Screen size in inches |
| `weight` | integer | Weight in grams |
| `price(INR)` | decimal | Phone price in Indian rupees |
| `release date` | text (DD/MM/YYYY) | Model release date |
| `user_name` | text | Customer first name |
| `Region(City)` | text | Customer's city (8 cities) |
| `Salary_in_INR` | integer | Customer's annual salary in Indian rupees |
| `age` | integer | Customer's age in years |
| `gender` | text | Male or Female |
| `occupation` | text | Customer's occupation |
