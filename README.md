# YouTube Automatic Playlist Uploader
This is a Python script that creates a new public YouTube playlist from a user's .csv/playlist.

## Setup
Before using this script, please make sure you have the following:
- A Google account with access to the YouTube Data API v3 [(click here for more details](https://developers.google.com/youtube/v3/getting-started))
- Python 3 installed
- Client secrets file downloaded from the Google Cloud Console and saved to your local machine

## Usage
1. Clone this repository to your local machine.
2. Open the script in a code editor of your choice and make sure to update the following:
   - CLIENT_SECRETS_FILE: the path to your client secrets file
   - title_playlist: the name of the playlist you want to convert to a YouTube playlist
   - description: the description you want for your new YouTube playlist
   - query: the search query used to find the video on YouTube
   - title and artist: the columns in your playlist CSV containing the track and artist names
3. Run the script.

## Dependencies
This script uses the following Python modules:
- google_auth_oauthlib
- googleapiclient
- pandas

## Note
- This script assumes that your music playlist has been exported as a CSV file using the [Spotisave](https://github.com/joosefupas/spotisave) code, but it's not limited to such format hence feel free to modify the names of your 'track artist' and 'track name' columns accordingly.
