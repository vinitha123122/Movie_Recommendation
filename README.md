IMDb Movie Recommendation Script

Overview

This project is a Python-based script that scrapes IMDb to recommend movies based on a user's chosen emotion or genre. It fetches movie titles from IMDb's genre-specific pages using requests and BeautifulSoup for web scraping.

Features

Fetch movie titles for the following genres:

->Drama

->Action

->Comedy

->Horror

->Crime

Returns a list of top movies based on the chosen genre.

Prerequisites

To run this script, ensure you have the following installed:

Python 3.6 or later

Required Python libraries:

->requests

->beautifulsoup4

Installation

1.Clone the repository:

->git clone https://github.com/your-username/imdb-movie-recommendation.git

2.Navigate to the project directory:

->cd imdb-movie-recommendation

3.Install the required Python libraries:

->pip install -r requirements.txt

Usage

1.Run the script:

->python imdb_scraper.py

2.Enter an emotion (genre) when prompted. For example:

->Enter the emotion: Drama

3.The script will fetch and display a list of movie titles matching the selected genre.

Code Explanation

1.Emotion Mapping: The script includes a dictionary to map emotions to related genres and their IMDb URLs.

2.Web Scraping: It utilizes requests to fetch the page content and BeautifulSoup to parse and extract movie titles.

3.Dynamic Input Handling: The script intelligently handles user inputs, suggesting the closest genre if an exact match is not found.

4.Error Handling: Handles invalid inputs and HTTP errors gracefully, ensuring user-friendly behavior.

Example Output

Enter the emotion: Comedy ok https://www.imdb.com/search/title/?title_type=feature&genres=comedy The Hangover Superbad Step Brothers ... (more titles)

File Structure

1.imdb_scraper.py: The main script.

2.requirements.txt: List of required Python libraries.

Contributing

Contributions are welcome! If you'd like to add more features or improve the script, feel free to submit a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for more information.

Notes

IMDb updates its website structure periodically, which may break the scraping functionality. Please ensure the href pattern in the script is up to date.

Use this script responsibly and adhere to IMDb's terms of service
