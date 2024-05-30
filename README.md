# youporn-scraper

A bash script for scraping youporn videos, channels and pornstars metadata in json.

## Requirements

 - [reliq](https://github.com/TUVIMEN/reliq)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 youporn-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [pornstar](pornstar-example.json) and [channel](channel-example.json).

## Usage

Results will be saved in files named by sha256 hash of their urls.

Download metadata of videos in DIR

    youporn-scraper -v DIR

Download metadata of videos to DIR

    youporn-scraper -d DIR -v URL -v URL -v URL
    youporn-scraper -d DIR URL URL URL

Download metadata of pornstars using 8 threads

    youporn-scraper -t 8 -p URL -p URL -p URL
    youporn-scraper -t 8 URL URL URL

Download metadata of channels into DIR using 8 threads

    youporn-scraper -t 8 -d DIR -c URL -c URL -c URL
    youporn-scraper -t 8 -d DIR URL URL URL

Download metadata of all pornstars from sitemap

    youporn-scraper -P

Download metadata of all videos from sitemap

    youporn-scraper -V

Download metadata of all channels from sitemap

    youporn-scraper -C

Get some help

    youporn-scraper -h
