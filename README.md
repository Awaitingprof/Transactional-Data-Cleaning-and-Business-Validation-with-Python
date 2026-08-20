# Transactional-Data-Cleaning-and-Business-Validation-with-Python
An end-to-end data cleaning, transformation, validation, and quality assurance project using Python and Pandas. This project transforms a complex, pivot-style retail sales report into a clean, structured, and analysis-ready dataset.

## Project Overview
The raw dataset contained embedded headers, structural missing values, Excel serial dates, multiple Ship Mode × Segment sales columns, and a Grand Total row.
The objective was to reconstruct the underlying transactional data while preserving the original business information and validating the transformation against the source totals.

<img width="967" height="478" alt="image" src="https://github.com/user-attachments/assets/76aa2e84-09e2-4088-8c96-3c7c316ff334" />

## Final Dataset
The cleaned dataset contains:
- 822 transactions
- 5 analytical fields
- 0 missing values
- 0 duplicate records
- 0 zero/negative sales
- 70 statistically identified but valid outliers
  
<img width="491" height="488" alt="Image" src="https://github.com/user-attachments/assets/32489fcb-a8c3-45c5-a9a1-248c4e9504b4" />

## Cleaning Process
- Raw Data Inspection:  Examined dimensions, columns, data types, headers, and missing-value patterns.
- Structural Analysis: Identified the embedded Order ID, Order Date, four Ship Modes, and three customer Segments.
- Header & Total Removal: Isolated the 822 genuine transaction records while excluding embedded headers and the Grand Total row.
- Wide-to-Long Transformation: Converted the 12 Ship Mode × Segment sales fields into a tidy transactional structure.
- Structural Missing-Value Handling: Removed empty combinations rather than incorrectly imputing them as zero.
- Date Transformation: Converted Excel serial dates into proper calendar dates.
- Data Type Standardisation: Converted Order Date to datetime and Sales to numeric.
- Data Quality Validation: Checked missing values, duplicates, categorical consistency, and invalid sales values.
- Outlier Analysis: Applied the IQR method and identified 70 high-value transactions. These were retained because they represented valid sales observations rather than demonstrated errors.
- Business Reconciliation: Compared the transformed Sales totals across all 12 Ship Mode × Segment combinations with the original Grand Total values. All totals reconciled exactly.
  
  <img width="491" height="488" alt="Image" src="https://github.com/user-attachments/assets/32489fcb-a8c3-45c5-a9a1-248c4e9504b4" />
  
## Tools and Technologies
- Python
- Pandas
- NumPy

### Skills Demonstrated
-  Data Cleaning
-  Data Transformation
-  Data Quality Assurance
-  Missing-Value Analysis
-  Excel Date Conversion
-  Outlier Detection
-   Business-Rule Validation
-   Data Reconciliation
-   Pandas
-   NumPy
-   Analytical Problem Solving

## Project Outcome
The project successfully converted a presentation-oriented retail report into a reliable analytical dataset without compromising the underlying sales information.

Effective data cleaning is not simply about removing missing values. It is about understanding the structure and business meaning of the data, transforming it appropriately, and proving that the resulting dataset still represents the original information.

This project demonstrates that approach through structured transformation, statistical validation, business reconciliation, and data-quality assurance.
