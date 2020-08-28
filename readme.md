# Cengage Webscraper 

[![LICENSE](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/dennisfarmer/cengage-webscraper/master/LICENSE)

Mr. Iyengar waits to share links to Mosley's calculus lecture videos via a week by week basis, so I have taken it upon myself to download every lecture video directly from Cengage Webassign to give me enough time to cover the class material. This can probably be edited slightly to allow for use with other course lectures on Cengage. 

I have also included a PDF copy of `Calculus: Early Trancendental Functions 7e` (68.6 MiB) as well as chapter powerpoints (118.3 MiB) for convenience. If you only want the webscraper script, feel free to just use `wget` as shown below.

### Requirements:
_Python:_
`BeautifulSoup, wget, requests, moviepy`
_Shell_:
`wget ffmpeg`

### Installation on Linux / Windows Subsystem for Linux:
```zsh
pip install beautifulsoup4 requests moviepy wget
apt-get install wget ffmpeg

wget https://raw.githubusercontent.com/dennisfarmer/cengage-webscraper/master/scraper.py
wget https://raw.githubusercontent.com/dennisfarmer/cengage-webscraper/master/unit_names.txt
```

### Usage:
```zsh
python scraper.py unit_names.txt
```

_It is recommended that you run this program overnight, as the below process is automatically repeated for every individual lecture video. Using a dedicated GPU will vastly improve rendering speeds._

*Shown at 25x Speed:*

![](preview.gif)
