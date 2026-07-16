Spotify ISRC Fetcher

Find ISRCs of the 20 most recent releases from any specific artist on Spotify.

Features

- Fetches artist data from a Spotify artist link
- Lists the 30 most recent releases (albums + singles)
- Extracts the ISRC of every track from each release
- Generates an organized output.txt file

Requirements

- Python 3.8+
- A Spotify for Developers account with an app created (to get a Client ID and Client Secret)

Installation

git clone https://github.com/robertojrss/Spotify-ISRC-Fetcher.git
cd Spotify-ISRC-Fetcher
pip install requests

Configuration

Set your Spotify credentials as environment variables before running (avoid hardcoding them):

Linux / macOS:
export SPOTIFY_CLIENT_ID="your_client_id"
export SPOTIFY_CLIENT_SECRET="your_client_secret"

Windows (PowerShell):
$env:SPOTIFY_CLIENT_ID="your_client_id"
$env:SPOTIFY_CLIENT_SECRET="your_client_secret"

Usage

python main.py

Paste the artist's Spotify link when prompted, for example:
https://open.spotify.com/artist/1234567890abcdef

The script will generate an output.txt file with all releases and ISRCs found.

Example output

ARTIST NAME
======================================================================

ALBUM: Album Name
Release date: 2026-05-10
----------------------------------------------------------------------
01. Track Name
    ISRC: US1234567890

02. Another Track
    ISRC: US1234567891

======================================================================

Built with

- Python
- Spotify Web API
- requests

License

This project is licensed under the MIT License. See the LICENSE file for details.
