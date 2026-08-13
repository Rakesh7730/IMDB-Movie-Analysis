# IMDB Movie Analysis - Data Cleaning Rules

## 1. Movie Dataset

### Duplicate Movies

- A movie is considered a duplicate when `title` and `release_year` are repeated.
- Do not remove duplicates randomly.
- Sort duplicate records by `rating` in descending order.
- Keep the record with the highest rating.
- If ratings are equal, keep the record with the highest `gross_million`.
- Remove the remaining duplicate records.

### Missing Values

- Identify missing values in all relevant columns.
- Apply column-specific business rules for handling missing values.
- Do not blindly replace missing values without understanding the column.

### Movie Title

- `title` should not be NULL or empty.
- Movie titles should be preserved without changing the original meaning.

### Release Year

- `release_year` should be numeric.
- Invalid or missing release years should be investigated.
- Do not guess missing release years.

### Rating

- `rating` should be numeric.
- Ratings should be within the expected IMDB rating range.
- Missing ratings should be investigated before removal or replacement.

### Genre

- Preserve available genre information.
- Missing genre values should not be replaced with guessed values.

### Director

- Preserve director information.
- Missing director values should be handled according to the project's missing-value rule.

### Actors

- Preserve actor information.
- Missing actor values should be handled according to the project's missing-value rule.

### Budget

- Convert budget values into a consistent numeric format where required.
- Invalid values should be investigated before removal.

### Gross Income

- Convert gross income into a consistent numeric format.
- Invalid or missing gross values should be handled according to the project's business rules.

---

## 2. Data Validation

### Duplicate Validation

- Verify that no duplicate `title + release_year` combinations remain after cleaning.

### Missing Value Validation

- Check the number of missing values after cleaning.
- Confirm that missing values were handled according to the defined business rules.

### Data Type Validation

- Verify that numeric columns have appropriate numeric data types.
- Verify that `release_year` is numeric.
- Verify that `rating`, `budget`, and `gross_million` are numeric where applicable.

### Final Dataset Validation

- Confirm the final row count.
- Confirm that duplicate records have been removed.
- Confirm that the cleaned dataset is ready to load into MySQL.
