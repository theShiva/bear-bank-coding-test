# Bank of the West Coding Test

# Requirements

Create a simple REST-ful API to perform some basic operations (see #2) on a list of Bank Locations, that are stored in a .CSV file.

1. The `bank-locations.csv` data file in the `\Data` folder is your data source of Bank locations. Import that into either a local SQL database or store it in-memory (ex HTTP Cache). The current user can be used to populate the `CreatedBy` field in the json (see #2).

<img src="/Docs/Media/bank-locations-screenshot.png" alt="free bank locations csv file"/>

2. Design and develop a REST API with various endpoints that expose the locations collection for the following operations. 
    - Get all locations
    - Get a single location
    - Delete a location
    - Create and Save a new location
    
3. Sample output of a GET operation on a `/api/locations/` endpoint, for example, should return the data as shown below (only 2 locations shown for illustration purposes)

````
[
  {
    "id": 1,
    "locationId": "L0004",
    "status": "A",
    "name": "Anaheim Hills",
    "addressLine1": "4501 E La Palma",
    "addressLine2": "",
    "city": "Anaheim",
    "state": "CA",
    "zipCode": 92807,
    "latitude": 37.33386,
    "longitude": -121.88932,
    "createdOn": "2016-04-13T15:15:56",
    "modifiedOn": "2016-12-07T16:20:09",    
    "createdBy": "lenny",
  },
  {
    "id": 2,
    "locationId": "L0005",
    "status": "A",
    "name": "Arcadia",
    "addressLine1": "1155 W Huntington Drive",
    "addressLine2": "",
    "city": "Arcadia",
    "state": "CA",
    "zipCode": 91006,
    "latitude": 37.33386,
    "longitude": -121.88932,
    "createdOn": "2017-10-13T15:15:56",
    "modifiedOn": "2017-04-07T16:20:09",    
    "createdBy": "teddy",
  }
]

````


4. Create your solution using ASP.Net Web API and upload your solution to a public github repository and send the recruiter the link to it so we can review your solution.

## Notes:
1. Not all the rows in `bank-locations.csv` are valid locations. You should only import and expose those rows / records that have an address, city, state and zipcode.
2. Design the various API endpoint keeping REST design priciples in mind. Ex: A DELETE on a location would use the DELETE Http VERB
3. You can create the API using either 

## Bonus:

The following is completely optional, and you can do some, all or none of these.

1. Create API documentation using Swagger
2. Populate `latitude` and `longitude` after the data import, using a geocoding api like Google Maps API.
3. Document the main classes using XML code comments
4. Write inline code comments to briefly describe the design patterns you are using.


