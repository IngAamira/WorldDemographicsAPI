# WorldDemographicsAPI - API Documentation

**WorldDemographicsAPI** is an API that provides global demographic data for countries and continents. The database contains data in English, so please use English names for countries and continents in your GET requests. Compound names should be separated by underscores ("_"), for example, "south_america".

## List of Available Routes

- **GET /data**: Get the full dataset
- **GET /continent/{continent_name}**: Get data for a specific continent
  - Parameters:
    - `continent_name` (string): The name of the continent
  - Example: `/continent/south_america`

- **GET /country/{country_name}**: Get data for a specific country
  - Parameters:
    - `country_name` (string): The name of the country
  - Example: `/country/brazil`

- **GET /population/{year}/{population}**: Get data for countries with a population greater than a certain threshold
  - Parameters:
    - `year` (int): The target year for population data
    - `population` (int): The minimum population threshold
  - Example: `/population/2022/50000000`

- **GET /visualize**: Visualize the dataset
  - Example: `/visualize`

- **GET /generate_bar_chart/{country_name}**: Generate a bar chart for a specific country
  - Parameters:
    - `country_name` (string): The name of the country
  - Example: `/generate_bar_chart/canada`

- **GET /generate_pie_chart/{continent_name}**: Generate a pie chart for a specific continent
  - Parameters:
    - `continent_name` (string): The name of the continent
  - Example: `/generate_pie_chart/north_america`

## Route Details

### GET /

Get information about the API.

### GET /data

Get the full dataset.

### GET /continent/{continent_name}

Get data for a specific continent.

- **Parameters:**
  - `continent_name` (string): The name of the continent

- **Example:**
  - `/continent/south_america`

### GET /country/{country_name}

Get data for a specific country.

- **Parameters:**
  - `country_name` (string): The name of the country

- **Example:**
  - `/country/brazil`

### GET /population/{year}/{population}

Get data for countries with a population greater than a certain threshold.

- **Parameters:**
  - `year` (int): The target year for population data
  - `population` (int): The minimum population threshold

- **Example:**
  - `/population/2022/50000000`

### GET /visualize

Visualize the dataset.

### GET /generate_bar_chart/{country_name}

Generate a bar chart for a specific country.

- **Parameters:**
  - `country_name` (string): The name of the country

- **Example:**
  - `/generate_bar_chart/canada`

### GET /generate_pie_chart/{continent_name}

Generate a pie chart for a specific continent.

- **Parameters:**
  - `continent_name` (string): The name of the continent

- **Example:**
  - `/generate_pie_chart/north_america`
