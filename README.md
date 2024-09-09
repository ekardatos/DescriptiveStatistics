# QuantitativeAnalysisOfLinguisticData

This project involves processing a large text file, splitting it into smaller files, and performing various statistical analyses on the text data. The project utilizes Python libraries such as `numpy`, `pandas`, `matplotlib`, and `seaborn` to manipulate and visualize the data.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data Preprocessing](#data-preprocessing)
- [Statistical Analysis](#statistical-analysis)
- [Visualizations](#visualizations)
- [License](#license)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/text-processing-project.git
    cd text-processing-project
    ```

2. Install the required Python packages:

    ```bash
    pip install numpy pandas matplotlib seaborn
    ```

## Usage

1. **Text Processing**: The main script reads a text file, removes punctuation, converts it to lowercase, and splits the text into words. It then creates multiple smaller text files based on a predefined word limit.

2. **Data Analysis**: The script reads a CSV file containing text data and performs various analyses, such as removing duplicates, calculating statistical measures (mean, median, standard deviation), and finding outliers.

3. **Visualizations**: The script generates boxplots and histograms for different text metrics to visualize the data distribution.

## Features

- **Text Splitting**: Splits a large text file into multiple smaller files.
- **Data Loading**: Loads and preprocesses data from a CSV file.
- **Statistical Analysis**: Computes mean, median, standard deviation, and identifies outliers.
- **Visualization**: Creates visual representations (boxplots, histograms) of various metrics.

## Data Preprocessing

1. **Text File Processing**: 
   - Reads the text from a specified file path.
   - Removes punctuation and converts text to lowercase.
   - Splits text into individual words and saves them into multiple smaller files.

2. **CSV Data Processing**:
   - Loads the CSV file using `pandas`.
   - Removes duplicate columns and unnecessary columns like frequencies.
   - Calculates descriptive statistics for different metrics.

## Statistical Analysis

- The script calculates various statistical measures:
  - Mean
  - Median
  - Standard Deviation
- Identifies and removes outliers based on certain conditions.

## Visualizations

- The script generates the following visualizations:
  - Boxplots for different metrics (e.g., TTR, h-Point, Entropy)
  - Histograms with KDE plots for each metric to visualize the distribution.
  - Calculates and displays skewness for various metrics.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
