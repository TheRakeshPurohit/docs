---
description: >-
  Explore the powerful validation options available for columns within our data
  import application
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🔰 Validators

Validators play a crucial role in ensuring the accuracy, consistency, and reliability of the data being imported via spreadsheets.

Each validator is designed to enforce specific rules on the column values, contributing to a seamless data import experience.

## Overview of the available validators, along with their functionalities:

1. **String Validator**: This validator ensures that the column value is a string. It also allows numbers, offering flexibility in handling diverse data types within the same column.
2. **Number Validator**: The Number validator verifies that the column value is a valid numeric entry. It enforces data integrity by permitting only numerical values.
3. **Email Validator**: With the Email validator, you can ensure that the column value conforms to a valid email format. This is particularly useful when dealing with email-related data.
4. **Regex Validator**: The Regex validator enables you to define a custom regular expression pattern that the column value must match. This versatile validator accommodates complex validation scenarios.
5. **Select Validator**: Use the Select validator to restrict column values to a predefined set of options. For instance, you can use it to ensure that a "Gender" column contains only values like "Male" or "Female."
6. **Any Validator**: The Any validator offers maximum flexibility by allowing any value in the column. This is handy when you don't need specific validation constraints.

### Validator Enhancements

* **isRequired**: When enabled, the isRequired checkbox mandates that a value must exist in each row of the column. This guarantees that essential data is not missing.
* **isUnique**: Enabling the isUnique checkbox ensures that the values in the column are unique throughout the entire spreadsheet. This prevents duplicate entries and promotes data accuracy.

Developers have the freedom to add each column individually and can directly modify the column JSON, tailoring the validation rules to their specific data import requirements.

Impler's validation system empowers developers and data engineers to create reliable data import workflows while maintaining data quality and integrity.

With Impler's rich array of validation options, you can confidently import data from spreadsheets, knowing that each column's content adheres to your predefined criteria.

Take advantage of these validators to build robust and error-free data pipelines that suit your unique needs.
