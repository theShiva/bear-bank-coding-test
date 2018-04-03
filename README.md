# Bank of the West Coding Test

# Requirements

Create a simple REST-ful API to perform CRUD operations on a list of Bank Locations, that are stored in a .CSV file.
1. The `bank-locations.csv` data file in the `\Data` folder is your data source of Bank locations. Import that into either a local SQL database or store it in-memory (ex HTTP Cache)
2. Design a REST API with various endpoints that expose the locations for CRUD operations. 
3. Sample output of a GET operation on a `/api/locations/` endpoint, for example, should return the following data

## Notes:
1. Not all the rows in `bank-locations.csv` are valid locations. You should only import and expose those rows / records that have an address, city, state and zipcode.
2. Design the various API endpoint keeping REST design priciples in mind. Ex: A DELETE on a location would use the DELETE Http VERB

## Bonus:

The following is completely optional, and you can do some, all or none of these.

1. Create API documentation using Swagger
2. Populate `latitude` and `longitude` after the data import, using a geocoding api like Google Maps API.
3 Document the main classes using XML code comments
4 Write inline code comments to briefly describe the design patterns you are using.

## Media

### Source data - bank-locations.csv

<img src="/Docs/Media/bank-locations-screenshot.png" alt="free bank locations csv file"/>

### Sample API JSON output for `/api/locations/` endpoint

<img src="/Docs/Media/bank-locations-json.jpg" alt="free bank locations json file"/>
