# Indexing Your Website with Redis and Python

## Introduction
* [X] About me
* [X] About RediSearch
* [X] Who I am, why I’m here
* [X] What we’re working on
    Search API
    Search frontend
        https://docs.redislabs.com
* [X] Redis and RediSearch
* [X] The redis-sitesearch project
* [X] The redis-sitesearch-frontend project
* [X] Requirements for the day
    Git
    Python >= 3.8
    Node.js >= 15
    Docker >= 20

### Hands-On: You Try

* [X] Clone https://github.com/redislabs-training/redis-sitesearch
* [X] Run `docker-compose up`


## Indexing https://andrewbrookins.com

### Creating a SiteConfiguration

* [X] Create a new SiteConfiguration for https://andrewbrookins.com
* [X] Use the same schema as an existing SiteConfiguration
* [X] Copy scorers, synonyms, validators, allow, deny, etc.

### Running the Index Job

* [X] Normally, indexing happens on a schedule every hour
* [X] Here’s how to start the index job manually from the CLI: `docker-compose exec worker index https://andrewbrookins.com`

### Hands-On: You Try

* [X] Add a SiteConfiguration for andrewbrookins.com
* [X] Run the index job: `docker-compose exec worker index https://andrewbrookins.com`

## BREAK!

* [X] 10 minute break

## Testing the Search API

### Curl and jq

* [X] Use curl to test some queries
* [X] Check the response objects

### Hands-On: You Try

* [X] Query via curl from the CLI
* [X] Or query from the browser: http://localhost:8000/search?q=*

## Setting Up the Frontend

### Cloning the Repository

* [X] Clone https://github.com/redislabs-training/redis-sitesearch-frontend
* [X] Run `npm run build`
* [X] Run `npm run demo`
* [X] Open the file demo/search.js and change line 3 to `const SEARCH_SITE = 'https://andrewbrookins.com'`

### Hands-On: You Try

* [X] Try running the demo

## Q&A
