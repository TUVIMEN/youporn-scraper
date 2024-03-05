# youporn-scraper

A bash script for scraping youporn videos, channels and pornstars metadata in json.

## Requirements

 - [hgrep](https://github.com/TUVIMEN/hgrep)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 youporn-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [pornstar](pornstar-example.json) and [channel](channel-example.json).

## Usage

Results will be saved in files named by their sha256 hash of urls and placed in DIR.

Download metadata of videos in DIR

    youporn-scraper -v DIR

Download metadata of pornstar in DIR

    youporn-scraper -p DIR

Download metadata of channel in DIR

    youporn-scraper -c DIR
