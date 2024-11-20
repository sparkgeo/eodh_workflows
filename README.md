# EODH Workflows

See [Workflow JSON](workflows.json) for the list of workflows and what inputs are required, both ones to allow the user to select and not.

Below are examples of the json that you would need to send to the ADES workflow for each one.

## Land Surface Temperature (LST) Day

Call to workflow "lst-filter" with the following JSON:

```json
{
    "inputs": {
        "workspace": "sparkgeouser",
        "assets": "sparkgeouser/uk_points.geojson",
        "stac_catalog": "https://test.eodatahub.org.uk/api/catalogue/stac/catalogs/user-datasets/sparkgeouser/processing-results/cat_f99e920a-a58e-11ef-aab0-7a33b70d8782",
        "start_date": "2024-03-01",
        "end_date": "2024-03-03",
        "stac_collection": "col_f99e920a-a58e-11ef-aab0-7a33b70d8782",
        "stac_query": "{'day_night': 'DAY'}",
        "token": <token>
    }
}
```

## Land Surface Temperature (LST) Night

Call to workflow "lst-filter" with the following JSON:

```json
{
    "inputs": {
        "workspace": "sparkgeouser",
        "assets": "sparkgeouser/uk_points.geojson",
        "stac_catalog": "https://test.eodatahub.org.uk/api/catalogue/stac/catalogs/user-datasets/sparkgeouser/processing-results/cat_f99e920a-a58e-11ef-aab0-7a33b70d8782",
        "start_date": "2024-03-01",
        "end_date": "2024-03-03",
        "stac_collection": "col_f99e920a-a58e-11ef-aab0-7a33b70d8782",
        "stac_query": "{'day_night': 'NIGHT'}",
        "token": <token>
    }
}
```

## OS Climate Physical Risk

Call to workflow "physrisk-filter" with the following JSON:

```json
{
        "inputs": {
                "workspace": "sparkgeouser",
                "assets": "sparkgeouser/realestate_assets.geojson"
        }
}
```
