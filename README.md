# Topsis-Garima-102203385
It performs TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) analysis on a given dataset.

## Installation
```pip install Topsis-Garima-102203385```

## How to use it?
Open the terminal and type the following command:\
\
```topsis <input_file> <weights> <impacts> <output_file>```

\
**`<input_file>`:** Path to the input CSV file.\
**`<weights>`:** Comma-separated weights for each criterion (e.g., 1,2,3).\
**`<impacts>`:** Comma-separated impacts for each criterion (e.g., +,+,-).\
**`<output_file>`:** Path to save the result CSV file.

\
**Example:**\
\
```topsis data.csv "1,2,3" "+,+,-" result.csv```

\
**Input File Format:**\
\
The input file must have at least three columns:
- The first column contains object names.
- The remaining columns contain numeric criteria values.

\
**Example input file (data.csv):**
|Object|Criteria1|Criteria2|Criteria3|
|------|---------|---------|---------|
|   A  |    250  |   16    |    12   |
|   B  |    200  |   20    |    15   |
|   C  |    300  |   14    |    18   |

\
**Output File Format:**\
\
The output file will include:
- Topsis Score: Calculated for each object.
- Rank: Objects ranked based on their Topsis scores.

\
**Example output file (result.csv):**
|Object|Criteria1|Criteria2|Criteria3|Topsis_Score|Rank|
|------|---------|---------|---------|------------|----|
|   A  |    250  |   16    |    12   |    0.78    |  1 |
|   B  |    200  |   20    |    15   |    0.52    |  3 |
|   C  |    300  |   14    |    18   |    0.68    |  2 |

## License
© 2025 Garima Ahuja

This repository is licensed under the MIT license. See LICENSE for details.
