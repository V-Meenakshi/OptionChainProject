

# Option Chain Data Analysis Project

## Project Overview

This project is designed to analyze option chain data for stock market instruments, focusing on retrieving and visualizing the highest Last Traded Prices (LTP) for Call (CE) and Put (PE) options across various strike prices. The project aims to identify market trends through expiry date filtering, data preprocessing, and effective visualization. Due to limited API access, data was sourced in CSV format, and mock data was generated to simulate API responses, providing a realistic experience with API-like data.

## Key Features

1. **Data Retrieval and Preprocessing**: 
   - Reads options data from a CSV file, cleans and preprocesses it, then filters by expiry date and option type (Call or Put).
   - Retrieves the highest LTP for each strike price, allowing for analysis of peak trading prices.

2. **Mock Data Generation**:
   - Simulates API responses by generating mock data, providing hands-on experience in handling real-time data structures without API access.

3. **Data Visualization**:
   - Uses grouped bar charts to display the highest LTP values for Calls (CE) and Puts (PE) by strike price, simplifying trend identification and price distribution analysis.

## Code Structure

### `get_option_chain_data` Function

- **Purpose**: Processes CSV data to retrieve the highest LTP for Calls and Puts by strike price, ready for visualization and analysis.
- **Steps**:
  - Loads and cleans the data using `pandas`, ensuring consistent column formatting.
  - Filters data based on the specified expiry date.
  - Separates Call and Put data, then extracts the highest LTP for each strike price using `groupby` and `max`.
  - Combines the processed data into a single, well-structured DataFrame for further analysis.

### `plot_option_chain` Function

- **Purpose**: Visualizes the option chain data through grouped bar charts, enhancing interpretability and simplifying data comparison across strike prices.
- **Steps**:
  - Prepares the data by converting columns to numeric types and handling any missing values.
  - Filters for the top N strike prices (optional) for focused analysis.
  - Sets up a pivoted data structure for easier plotting.
  - Uses Matplotlib and Seaborn to generate color-coded bar charts for Calls and Puts, adding value labels and formatting for readability.

## ChatGPT Assistance in Development

ChatGPT was instrumental in developing this project, particularly in error handling, code optimization, and API simulation strategies. Some specific areas where ChatGPT assisted include:

- **Syntax Corrections and Debugging**: ChatGPT helped resolve syntax errors encountered during data processing and visualization setup.
- **Error Handling**: AI provided error-handling strategies for data type conversions and missing values, helping create a robust codebase.
- **Mock Data Simulation Guidance**: Since API access was limited, ChatGPT suggested ways to simulate API responses with mock data, providing an effective workaround.

To illustrate ChatGPT’s assistance in the project, a Colab notebook is available that includes rough code versions with common errors and ChatGPT’s recommendations for resolving them. This notebook documents the evolution of the code, showcasing how AI suggestions led to the final, error-free version.

[Colab Notebook - ChatGPT-Assisted Code Development](https://colab.research.google.com/drive/1qgTbLoPgs_MhJPo9mNaskECCL1GX-JLr?usp=drive_link)  

## Insights and Unique Approaches

- **API Simulation with Mock Data**: By creating mock data that mimics API responses, the project provides a practical approach to real-time data handling without live API access.
- **Visualization**: The use of grouped bar charts helps in analyzing the distribution of LTP values for Calls and Puts, simplifying complex market data into actionable insights.

## Conclusion

This project helped build key skills in data preprocessing, error handling, and visualization. The collaboration with ChatGPT allowed for a smooth workflow, troubleshooting errors, and refining the logic for optimal results. This experience has strengthened my abilities in data-driven decision-making and prepared me for handling real-world API integrations in future projects.

Thank you for reviewing this project. I’m excited about the opportunity to apply these skills in a professional setting.

---

