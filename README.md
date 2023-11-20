# youporn

A bash script for archiving youporn videos, channels and pornstars metadata in json.

## Requirements

 - [hgrep](https://github.com/TUVIMEN/hgrep)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 youporn /usr/bin

## Json format

Here's example of a [video](video-example.json), [pornstar](pornstar-example.json) and [channel](channel-example.json).

## Usage

Results will be saved in files named by their sha256 hash of urls and placed in DIR.

Download metadata of videos in DIR

    youporn -v DIR

Download metadata of pornstar in DIR

    youporn -p DIR

Download metadata of channel in DIR

    youporn -c DIR
