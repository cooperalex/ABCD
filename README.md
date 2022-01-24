# ABCD
Open Hackathon

Basically we need to come up with a JSON interface to input data, something like:

`
{imageid=””, image_truth=true/false, algorithm=”” algorithm_version=””,location=lon,lat or WKT, id=””, radius_of_confidence=radius in meters, chip=Uuencoded (optional)}
`
..and anything else I missed

## Project Goals

1. Provide a simple json interface to accept observations from humans, algorithms or models
2. The json will return a UUID for the record
3. Provide a simple open layer map (OSM?) to display results and allow filtering based on algorithm or model.

## Backend

- Django 2.2.10
- PostGIS

## Frontend

- OSM
- Openlayers

## Setup

After checkout:

`$ cd ABCD`

`$ python3 -m venv env`

`$ source env/bin/activate`

`$ pip install -r requirements.txt`

`$ cd abcd`

`$ python manage.py runserver 0.0.0.0:8080`