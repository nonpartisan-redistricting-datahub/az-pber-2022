# Election Results Dataset

## Overview
This dataset contains election results for various offices across different precincts in a specific county. Each row represents the results of a candidate in a particular precinct for a given office.

## Column Descriptions

- **county**: The name of the county where the precinct is located.
  - Example: `Pinal`

- **precinct**: The specific precinct within the county where the votes were cast.
  - Example: `01 Kearny`

- **office**: The office for which the candidate is running. The office names have been standardized and mapped to abbreviations in the final processed dataset.
  - Example: `U.S. Senate` (abbreviated as `USS`)

- **district**: The district number for the election, applicable for offices that have multiple districts. This column may be `NaN` if the office does not have district-specific elections.
  - Example: `2`

- **candidate**: The full name of the candidate.
  - Example: `Mark Kelly`

- **party**: The political party of the candidate. The values have been standardized to their uppercase forms.
  - Example: `D` (Democratic Party)

- **votes**: The total number of votes received by the candidate in the precinct.
  - Example: `382`

- **ColumnName**: A generated column that combines several pieces of information to create a unique identifier for each candidate in a standardized format. The format includes:
  - `G`(General Election) followed by:
    - The office abbreviation.
    - The district number (if available) placed after the office abbreviation.
    - The first letter of the party.
    - The first three letters of the candidate's last name.

  - Examples:
    - For a candidate running in a district-specific office: `GUSH2DDOH` (U.S. House, District 2, Democratic Party, Last name starts with "Doh")
    - For a candidate without a district-specific office: `G22ATTDMAY` (Attorney General, Democratic Party, Last name starts with "May")

## Notes
- The dataset is cleaned and standardized to ensure consistency in the representation of office names, party affiliations, and candidate names.
- The `ColumnName` field is particularly useful for quickly identifying candidates and their respective offices and districts in the pivoted dataset format.
