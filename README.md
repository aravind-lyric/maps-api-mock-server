# Maps Data API

## Required runtime

[Node.js](https://nodejs.org/en/) is required to run the project. Please have the latest version installed before using this project.

## Installation

- Clone this repository and `cd` into the root directory of this repository.
- Run `npm i`.
- Run `npm start` to run the server on port 3000 (To change port, set the desired PORT value in `package.json > scripts > start`).

## Routes

- GET `http://localhost:<port>/datasets` to get the list of all datasets (currently only two datasets are available: Network data and Routes data).
- GET `http://localhost:<port>/dataset/<dataset-name>` to get data for that particular dataset.
- PATCH `http://localhost:<port>/app-data/<id>` with any JSON payload in the body of the request to store the config needed to render the "View" of the map.
- GET `http://localhost:<port>/app-data` to get the list of all app config data stored for the datasets.

Note: For PATCH call, use the IDs of the individual datasets.

## Postman collection

There is a Postman collection JSON at the root of this repository named `postman-collection.json`. It can be imported into Insomnia app too.
