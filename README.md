README

Overview:
This repository contains a set of Python functions for scraping song lyrics from lyrics.com for a specified artist. The main goal is to extract song titles, URLs, and lyrics, and save them in a structured CSV format. Additionally, it provides basic data processing and visualization tools to generate insights from the lyrics.

Features:
Scrape song information: Fetch song titles and URLs for up to 100 songs by a specified artist.
Extract lyrics: Download lyrics for each song and save them in a CSV file.
Data processing: Count the number of words in each song and organize data into a CSV with the following columns:
Artist
Album
Song Title
URL of Song Lyrics
Song Lyrics
Number of Words in the Song
Visualization: Generate a word cloud from the collected lyrics to highlight frequently used words.
Dependencies
Make sure to install the required Python packages before running the script:

bash
Copy
Edit
pip install requests beautifulsoup4 wordcloud matplotlib
Usage
Specify the artist: Update the artist variable with the name of the artist you want to scrape.
Run the script: Execute the script to fetch song information and lyrics.
Generate CSV: The script saves the data to a CSV file named <artist>_songs.csv.
Create a word cloud: View a word cloud of the most common words in the lyrics.
Example
python
Copy
Edit
artist = 'The Beatles'
songs = get_artist_songs(artist)
print(songs)
This will output a list of songs with titles and links, and create a CSV file with detailed information.

Limitations
The script only fetches up to 100 songs for demonstration purposes due to time and resource constraints.
The structure of lyrics.com may change, causing the script to break. It may need adjustments if the HTML layout is updated.
License
This project is open-source and available under the MIT License.

Feel free to contribute by submitting issues or pull requests!
