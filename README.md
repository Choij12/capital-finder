# capital-finder

## Overview

Deploy a serverless function to the cloud.

## Feature Tasks and Requirements

- Sign up with [Vercel]
- Create a repository on Github and link it to Vercel account.
- Use [requests](https://docs.python-requests.org/en/latest/){:target="_blank"} library to interact with [REST Countries API](https://restcountries.com/#rest-countries){:target="_blank"}
- Create a serverless function following Vercel's get-started directions that handles two kinds of queries:
  - The serverless function should handle a `GET` http request with a given country name that responds with a string with the form `The capital of X is Y`
    - E.g.`/capital-finder?country=Chile` should generate an http response of `The capital of Chile is Santiago.`
    - The serverless function should handle a `GET` http request with a given capital that responds with a string with the form `The capital of X is Y`
      - E.g.`/capital-finder?capital=Santiago` should generate an http response of `Santiago is the capital of Chile.`
