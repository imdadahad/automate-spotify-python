# Automate Spotify with Python

Pulls music videos from your YouTube playlists and adds them to Spotify

## Getting Started

For this project, you will need Python installed on your system.

### Prerequisites

1. YouTube Data API credentials (named as `client_secret.json`). These must be placed in the creds/ directory.
2. Spotify Web API OAuth Token. Must be sourced in your environment as `SPOTIFY_AUTH_TOKEN`

### Installing

```
pip install -r requirements.txt
```

## Running the app

```
python run.py
```

## Common issues

Song and artist fields sometimes come back as None in json response. This can be resolved by setting the youtube_dl User-Agent to Facebook's web crawler:
```
youtube_dl.utils.std_headers['User-Agent'] = "facebookexternalhit/1.1 (+http://www.facebook.com/externalhit_uatext.php)"
```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## YouTube Video Tutorial


![Image description](https://i.imgur.com/9PhXtCd.jpg)

Link: https://youtu.be/R3XgZ__jQxw
