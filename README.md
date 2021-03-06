# dh-books-discovery
DailyHunt Books' plugin module for 360fy's humane-discovery.

## How to Setup

1. Ensure prerequisites of [humane-discovery](https://github.com/360fy/humane-discovery).
2. Install humane-discovery v1.1.5 as global module: `npm install -g humane-discovery@v1.1.5`
3. Install dh-books-discovery as global module: `npm install -g https://private-npm-releases.s3.amazonaws.com/dh-books-discovery-1.1.3.tgz`
4. Install dh-transliterate as global module: `npm install -g https://private-npm-releases.s3.amazonaws.com/dh-transliterate-1.0.0.tgz`
5. To run server: `humane-server -d dh-books-discovery --transliterator dh-transliterate`
6. To run cli: `humane-cli -d dh-books-discovery`
7. You can optionally export environment variables for plugin and transliterator and run commands without any arguments.
    - Export Plugin: `export HUMANE_PLUGIN_DISCOVERY=dh-books-discovery`
    - Export Transliterator: `export HUMANE_PLUGIN_TRANSLITERATOR=dh-transliterate`
    - Run Server: `humane-server`
    - Run Cli: `humane-cli`
8. Setup watcher for book stats from profile feed: 
    - If Plugin is exported: `humane-cli importBookStats -w -i <stats-directory>`
    - Otherwise: `humane-cli -d dh-books-discovery importBookStats -w -i <stats-directory>`    

## API Documentation
- [Indexer APIs](https://github.com/360fy/humane-indexer)
- [Search APIs](https://github.com/360fy/humane-searcher)

## Search Types
- book
- category_entity
- author_entity
- publisher_entity

## Autocomplete Types
- *
- searchQueryAutocomplete
- authorAutocomplete
- categoryAutocomplete
- publisherAutocomplete
- bookAutocomplete


Working set :

# dh-books-discovery
DailyHunt Books' plugin module for 360fy's humane-discovery.

## How to Setup

1. Ensure prerequisites of [humane-discovery](https://github.com/360fy/humane-discovery).
2. Install humane-discovery as global module: `install npm install -g humane-discovery@v1.1.8-fix.1`
3. Install dh-books-discovery as global module: `npm install -g https://private-npm-releases.s3.amazonaws.com/dh-books-discovery-1.1.6-fix.0.tgz`
4. Install dh-transliterate as global module: `npm install -g https://private-npm-releases.s3.amazonaws.com/dh-transliterate-1.0.0.tgz`
5. To run server: `humane-server -d dh-books-discovery --transliterator dh-transliterate`
6. To run cli: `humane-cli -d dh-books-discovery`
7. You can optionally export environment variables for plugin and transliterator and run commands without any arguments.
- Export Plugin: `export HUMANE_PLUGIN_DISCOVERY=dh-books-discovery`
- Export Transliterator: `export HUMANE_PLUGIN_TRANSLITERATOR=dh-transliterate`
- Run Server: `humane-server`
- Run Cli: `humane-cli`
8. Setup watcher for book stats from profile feed: 
- If Plugin is exported: `humane-cli importBookStats -w -i <stats-directory>`
- Otherwise: `humane-cli -d dh-books-discovery importBookStats -w -i <stats-directory>` 

## API Documentation
- [Indexer APIs](https://github.com/360fy/humane-indexer)
- [Search APIs](https://github.com/360fy/humane-searcher)

## Search Types
- book
- category_entity
- author_entity
- publisher_entity

## Autocomplete Types
- *
- searchQueryAutocomplete
- authorAutocomplete
- categoryAutocomplete
- publisherAutocomplete
- bookAutocomplete

CHAT:

you can put the configurations in some folder
and define production.yml for production env.
staging.yml for staging
default.yml for dev
for env. you need to export NODE_ENV=production, for example.
you can see defined properties in source code I sent you for dh-books
they are under envConfig folder
production properties are defined as per your prod env. but commented
I picked those values from earlier shared code
default it picks from that location as you mentioned
but way to override is put in some outside folder and use it with -c or --config argument
point to folder, not property file.


