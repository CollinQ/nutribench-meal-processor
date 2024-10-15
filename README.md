# NutriBench Meal Processor

## Description

NutriBench Meal Processor is a data analysis and processing project focused on nutritional data from various datasets, particularly those from Kenya. The project aims to combine, clean, and analyze food consumption data, create unit conversions, and add word embeddings to food descriptions for better analysis and potential machine learning applications.

## Project Structure

The project consists of several Jupyter notebooks and datasets:

1. `combine_datasets.ipynb`: Combines and cleans multiple datasets.
2. `Portion Weight Conversion/portion_weight_conversion.ipynb`: Creates a food unit conversion table.
3. `Portion Weight Conversion/add_word_embeddings.ipynb`: Adds word embeddings to food descriptions.

## Installation

To run this project, you need Python 3.12.5 or later. Install the required packages using:

```bash
pip install -r requirements.txt
```


## Usage

1. Data Combination and Cleaning:
   Run the `combine_datasets.ipynb` notebook to combine and clean the datasets.

2. Food Unit Conversion:
   Execute the `portion_weight_conversion.ipynb` notebook to create a food unit conversion table.

3. Word Embeddings:
   Use the `add_word_embeddings.ipynb` notebook to add word embeddings to food descriptions.

## Key Features

- Data cleaning and combination from multiple sources
- Creation of a food unit conversion table
- Addition of word embeddings to food descriptions using OpenAI's API
- Visualization of null value percentages across datasets

## Data Sources

The project uses several datasets from Kenya, provided by Bioversity International. These datasets include:

- KEN_00035
- KEN_00469
- KEN_00470
- KEN_00471
- KEN_00472
- KEN_00475

For more information on the data sources, refer to the `FAO-WHO Data acknowledgment.txt` files in the respective dataset folders.

## Environment Variables

To use the OpenAI API for word embeddings, you need to set up an `.env` file with your API key:

```bash
OPENAI_API_KEY=<your_openai_api_key>
```

## Output Files

The project generates several output files:

- `combined_consumption_user.csv`: Combined dataset from all sources
- `combined_consumption_user_with_days.csv`: Combined dataset with days information
- `combined_consumption_user_with_days_and_food_name.csv`: Final combined dataset with food names
- `food_unit_conversion.csv`: Food unit conversion table
- `food_unit_conversion_with_embeddings.json`: Food unit conversion table with word embeddings

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

Data provided by Bioversity International, Nutrition and Marketing Diversity Programme, Italy – CGIAR Global Research Centre. When using this data, please provide the following acknowledgment:

"Improving nutrition through increased utilisation of local agricultural biodiversity in Kenya – the INULA initiative – Baseline data 2012"

Or shortly: "Kenya, Bioversity International, 2012"

## Contributing

Contributions to this project are welcome. Please ensure that you update tests as appropriate and adhere to the existing coding style.