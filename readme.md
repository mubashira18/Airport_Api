# Airport API

This project is a Node.js-based API for retrieving information about airports, cities, and countries. The API provides endpoints to query data related to airports, including associated city and country information.

### Folders and Files

- **controllers/**: Contains the controller files that handle the logic for each endpoint.

  - `airportController.js`: Contains the logic for handling airport-related requests.
  - `cityController.js`: Contains the logic for handling city-related requests.
  - `countryController.js`: Contains the logic for handling country-related requests.

- **models/**: Contains the data models that define the structure of the database tables.

  - `Airport.js`: Defines the Airport model.
  - `City.js`: Defines the City model.
  - `Country.js`: Defines the Country model.

- **routes/**: Contains the route definitions for the API endpoints.

  - `airport.js`: Defines the routes for airport-related endpoints.
  - `city.js`: Defines the routes for city-related endpoints.
  - `country.js`: Defines the routes for country-related endpoints.

- **index.js**: The main entry point of the application.

- **package-lock.json**: Automatically generated file that describes the exact tree that was generated, such as versions of the dependencies.

- **package.json**: Contains the metadata for the project, including dependencies, scripts, and other configuration.

## Prerequisites

- Node.js (version 14.x or higher)
- MySQL (Ensure it is installed and running)

## Setup Instructions

1. **Clone the repository:**

   ```sh
   git clone https://github.com/mubashira18/Airport_Api.git
   cd airport-api
   Get Airport by IATA Code
   Endpoint: /airport?iata_code=XYZ
   eg link:: https://airport-9rlu.onrender.com/api/airport?iata_code=AGR
   ```

Method: GET

Response:

json

{
  "airport": {
    "id": 145,
    "icao_code": "VIAG",
    "iata_code": "AGR",
    "name": "Agra Airport / Agra Air Force Station",
    "type": "medium_airport",
    "latitude_deg": 27.157683,
    "longitude_deg": 77.960942,
    "elevation_ft": 551,
    "address": {
      "city": {
        "id": 436,
        "name": "Agra",
        "country_id": 76,
        "is_active": true,
        "lat": 27.18,
        "long": 78.02
      },
      "country": {
        "id": 76,
        "name": "India",
        "country_code_two": "IN",
        "country_code_three": "IND",
        "mobile_code": 91,
        "continent_id": 1
      }
    }
  }
}
deployed link --  https://airport-9rlu.onrender.com/api/airport
