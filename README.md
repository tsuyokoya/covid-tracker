# Covid-19 Tracker

<img src='./screenshots/covid-cards' alt='covid tracker main' height='350' width='500'>

## 🧐 Project Description

This is a Covid-19 tracker that displays the number of infected, recovered, and deaths due to Covid-19.
The "Global" selection displays the Covid data in a line graph on a daily basis.
Selection of individual countries shows the data for that country in a bar chart.
Please note that the API no longer updates the daily number of cases (there is data up to 2021-02-03) or the number of recovered individuals.

Technologies used: React.js, Material UI, Axios, Chart.js
API: https://covid19.mathdro.id/api

## 💭 Structure

### Components

Aside from the App component, there are three components:

- Cards
  - Displays the cards that show the number of infected, recovered, and deaths.
- Chart
  - Displays the line chart, if the selection is "Global", or the bar chart, if a specific country is selected.
- CountryPicker
  - Dynamically creates the select field to display all countries supported by the API as options.

### API

The "api" directory contains an index.js file that fetches (via axios) the daily data and data by country.

## Line chart for daily Covid-19 cases

<img src='./screenshots/covid-daily' alt='covid tracker main' height='350' width='500'>

## Bar chart for a specific country's Covid-19 cases

<img src='./screenshots/covid-country' alt='covid tracker main' height='350' width='500'>
