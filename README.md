# THIS IS NOT AN ORIGINAL Hydra-Launcher Prepository I JUST MADE THIS FOR THE DOWNLAOD SOURCES
# Original Link: https://github.com/hydralauncher/hydra



- Go to settings
- Download Sources
- Import
- And Copy paste every link individually

		https://hydralinks.cloud/sources/xatab.json
		https://hydralinks.cloud/sources/tinyrepacks.json
		https://hydralinks.cloud/sources/onlinefix.json
		https://hydralinks.cloud/sources/kaoskrew.json
		https://hydralinks.cloud/sources/gog.json
		https://hydralinks.cloud/sources/fitgirl.json
 		https://hydralinks.cloud/sources/empress.json
		https://hydralinks.cloud/sources/dodi.json
		https://hydralinks.cloud/sources/steamrip.json
		https://hydralinks.cloud/sources/atop-games.json
		https://hydralinks.cloud/sources/repack-games.json

# OR
- Go To this link
- https://hydralinks.cloud/
- And press install on hydra whichever Download Source You feel is safe
<br>

<div align="center">

[<img src="./resources/icon.png" width="144"/>](https://help.hydralauncher.gg)

  <h1 align="center">Hydra Launcher</h1>

  <p align="center">
    <strong>Hydra is a game launcher with its own embedded bittorrent client.</strong>
  </p>

[![build](https://img.shields.io/github/actions/workflow/status/hydralauncher/hydra/build.yml)](https://github.com/hydralauncher/hydra/actions)
[![release](https://img.shields.io/github/package-json/v/hydralauncher/hydra)](https://github.com/hydralauncher/hydra/releases)

</div>
**Hydra** is a **Game Launcher** with its own embedded **BitTorrent Client**.
<br>
The launcher is written in TypeScript (Electron) and Python, which handles the torrenting system by using libtorrent.

## Features

- Own embedded bittorrent client
- How Long To Beat (HLTB) integration on game page
- Downloads path customization
- Windows and Linux support
- Constantly updated
- And more ...

## Installation

Follow the steps below to install:

1. Download the latest version of Hydra from the [Releases](https://github.com/enmafps/hydra-launcher-guide/releases/latest) page.
   - Download only .exe if you want to install Hydra on Windows.
   - Download .deb or .rpm or .zip if you want to install Hydra on Linux. (depends on your Linux distro)
2. Run the downloaded file.
3. Enjoy Hydra!
## Build from source

### Install Node.js

Ensure you have Node.js installed on your machine. If not, download and install it from [nodejs.org](https://nodejs.org/).

### Install Yarn

Yarn is a package manager for Node.js. If you haven't installed Yarn yet, you can do so by following the instructions on [yarnpkg.com](https://classic.yarnpkg.com/lang/en/docs/install/).

### Install Node Dependencies

Navigate to the project directory and install the Node dependencies using Yarn:

```bash
cd hydra
yarn
```

### Install OpenSSL 1.1

[OpenSSL 1.1](https://slproweb.com/download/Win64OpenSSL-1_1_1w.exe) is required by libtorrent in Windows environments.

### Install Python 3.9

Ensure you have Python 3.9 installed on your machine. You can download and install it from [python.org](https://www.python.org/downloads/release/python-3913/).

### Install Python Dependencies

Install the required Python dependencies using pip:

```bash
pip install -r requirements.txt
```

## Environment variables

You'll need an SteamGridDB API Key in order to fetch the game icons on installation.

Once you have it, you can copy or rename the `.env.example` file to `.env` and put it on`STEAMGRIDDB_API_KEY`.

## Running

Once you've got all things set up, you can run the following command to start both the Electron process and the bittorrent client:

```bash
yarn dev
```

## Build

### Build the bittorrent client

Build the bittorrent client by using this command:

```bash
python torrent-client/setup.py build
```

### Build the Electron application

Build the Electron application by using this command:

On Windows:

```bash
yarn build:win
```

On Linux:

```bash
yarn build:linux
```

## License

Hydra is licensed under the [MIT License](LICENSE).
