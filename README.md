# Scraping Football Data from FBref



## Table of Contents
- [About](#about)
- [Usage](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

# About
This Python script allows users to scrape football (soccer) data from FBref for various leagues including the English Premier League (EPL), Bundesliga, La Liga, Serie A, and Ligue 1. The user can select the desired league, and the script will fetch and save the corresponding data as a CSV file.

## How to use
Select League: Run the script and choose the league you want to scrape data for.

Scraping Process: The script fetches the HTML content of the selected league's page on FBref using the requests library and parses it using BeautifulSoup.

Data Extraction: It extracts various statistics including team standings, possession, standard stats, shooting, passing, goal shot creation, and defensive stats from the HTML content.

Data Processing: The extracted data is processed, and column names are updated for clarity.

Data Merging: Different statistics are merged into a single DataFrame for comprehensive analysis.

Data Cleaning: Unnecessary columns are dropped to streamline the DataFrame.

Saving Data: The cleaned and merged DataFrame is saved as a CSV file with the league's name and the season appended to the filename.

## Code Explanation
The script defines functions to fetch HTML content (fetch_data), extract table data (get_table_data), and update column names (update_column_names).

The user is prompted to select a league from a list of available options (EPL, Bundesliga, La Liga, Serie A, Ligue 1).

After the user selects a league, the script dynamically constructs the URL for the selected league and fetches data from FBref.

The div_id for the team standings table (team_table) is dynamically generated based on the league URL to ensure correct data extraction.

The script then extracts various statistics tables such as possession, shooting, passing, etc., from the HTML content.

It updates the column names of the extracted tables for clarity and merges them into a single DataFrame.

Unnecessary columns are dropped from the DataFrame to keep only relevant information.

Finally, the cleaned DataFrame is saved as a CSV file named after the selected league and season.

## Dependencies
Python 3.x

pandas: For data manipulation

requests: For making HTTP requests

BeautifulSoup: For HTML parsing



After running the script, follow the on-screen prompts to select the desired league. The script will then scrape the data, process it, and save it as a CSV file.

## Note
Ensure that you have a stable internet connection while running the script as it fetches data from the web.


## Contributing
Contributions to this project are welcome! If you find any bugs or have suggestions for improvements, please feel free to open an issue or submit a pull request.

Before contributing, please ensure that you have read the [Contributing Guidelines](CONTRIBUTING.md).


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


### Running the Python Script

You can run the Python script directly from GitHub using either Binder or Google Colab:

#### Using Binder

1. Navigate to [Binder](https://mybinder.org/).
2. Paste the GitHub URL of the repository containing your Python file into the "GitHub repository name or URL" field.
3. Click the "launch" button.

#### Using Google Colab

1. Go to [Google Colab](https://colab.research.google.com/).
2. Click on "File" -> "Open notebook".
3. Select the "GitHub" tab.
4. Paste the GitHub URL of the repository containing your Python file [Football-Stats_Scraper](https://github.com/ezrarichard/Football-Stats-Scraper.git). 
5. Select the Python file you want to open.


## Support
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Donate-yellow.svg)](https://www.buymeacoffee.com/ezrarichard)
