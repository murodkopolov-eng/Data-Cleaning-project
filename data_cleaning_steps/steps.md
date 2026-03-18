# Data Cleaning Project

This project focuses on cleaning and preprocessing a messy student dataset.

---

## Step 1: Data Understanding
- Load CSV file and preview first 10 rows
- Check column names and total number of columns
- Identify missing values in each column
- Understand data types (string, numeric, date, JSON)

---

## Step 2: String Cleaning
- Remove leading and trailing spaces using strip()
- Replace empty strings with NaN / Null values

---

## Step 3: Numeric and Date Cleaning
- Clean and convert numeric columns (Age, Score, GPA, Attendance, Money_Spent)
- Convert columns to appropriate types (int, float)
- Convert date columns to pandas datetime format

---

## Step 4: Email and Phone Validation
- Convert emails to lowercase
- Detect invalid email formats
- Standardize phone numbers (e.g., +998 format)

---

## Step 5: JSON Parsing
- Parse JSON column (profile_json)
- Extract fields into separate columns:
  - hobbies
  - skills
  - family
  - devices
- Flatten nested structures if necessary

---

## Step 6: Address Parsing
- Split address into structured fields:
  - city
  - district
  - postal code
- Preserve original raw address column

---

## Step 7: Handling Duplicates and Missing Data
- Identify and remove duplicate rows
- Handle missing values:
  - Fill (fillna)
  - Drop (dropna)

---

## Step 8: Data Normalization
- Standardize gender values (Male / Female / Unknown)
- Normalize course names (Data Science / Python / Other)
- Standardize status values (lowercase or consistent format)

---

## Step 9: Final Type Conversion and Export
- Ensure correct data types (string, int, float, datetime)
- Standardize date format (YYYY-MM-DD HH:MM:SS)
- Export cleaned dataset:
  - `super_dirty_students_cleaned.csv`

---

## Step 10: Quality Assurance (QA Checks)
- Compare row counts (original vs cleaned)
- Check missing email and phone counts
- Validate numeric ranges (GPA, attendance, score)
- Ensure no duplicate rows remain
