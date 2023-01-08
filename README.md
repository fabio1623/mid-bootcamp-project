# Top 100 Spotify Podcasts in Germany Data Analysis Project (mid-bootcamp-project)

## Introduction

This project aims to provide insights into the most popular podcasts on Spotify in Germany in December 2022.
(100 Podcasts & 17k Episodes)

## Data Sources

We have scraped data from the following sources:

- https://podcastcharts.byspotify.com/
- https://www.buzzsprout.com/global_stats

The scraped data can be found in the `scraped_data` folder.

## Data Folder

In the `data` folder, we have a `json` folder which contains cached HTTP responses and a `csv` folder which contains cleaned podcasts (shows) and their episodes data.

## Image Folder

The `image` folder contains images used for the Tableau presentation. (https://public.tableau.com/shared/742R67JT9?:display_count=n&:origin=viz_share_link)

## Spotify Data Aggregator Notebook

The `spotify-data-aggregator` notebook performs the following tasks:

1. It cleans the `spotify_top_100_germany.csv` file.
2. It retrieves podcast and episodes data from the Podcast IDs found in the `spotify_top_100_germany.csv` file using the Spotify REST API (https://developer.spotify.com/documentation/web-api/reference/) and the `spotipy` library.
3. It enriches the data using OpenAI and cleans the podcast and episodes data again.
4. It saves the podcast and episodes data in a MySQL database.

## Conclusion

We hope that this project helps you to better understand the most popular podcasts on Spotify in Germany in December 2022.