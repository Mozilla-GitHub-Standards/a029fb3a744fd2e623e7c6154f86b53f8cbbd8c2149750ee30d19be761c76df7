# switchboard-experiments-kinto

This project let you manage the configuration files for managing [switchboard-experiments](https://github.com/mozilla-services/switchboard-experiments) data using [Kinto](http://kinto-storage.org/).

## Setup the collection

Enter the kinto-bootstrap folder, then you can setup the collection on a kinto server by running the following command:

    make migrate SERVER_URL=https://localhost:8888/v1 AUTH=token:switchboard BUCKET=switchboard COLLECTION=features

- The switchboard data will be editable on to the [kinto-admin](http://kinto.github.io/kinto-admin/).
- Published JSON data will then be available here: https://localhost:8888/v1/buckets/switchboard/collections/features/records

## License

Apache-2.0
