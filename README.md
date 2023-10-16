# WorldDemographicsAPI

**World Demographics API** is an open-source API that provides comprehensive demographic data for countries and continents worldwide. Our API allows easy access to information on population statistics, including total population and population over specific years. It's designed for developers looking to integrate demographic data into their applications and analyses. Explore global demographic trends with WorldDemographicsAPI!

## Table of Contents

- [Features](#features)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Features

- Access population data for countries and continents.
- Generate bar charts for specific countries.
- Generate pie charts for specific continents.

## Usage

To use the API, make GET requests to the following endpoints:

- `/data`: Get the full dataset.
- `/continent/{continent_name}`: Get data for a specific continent.
- `/country/{country_name}`: Get data for a specific country.
- `/population/{year}/{population}`: Get data for countries with a population greater than a certain threshold.
- `/visualize`: Visualize the dataset.
- `/generate_bar_chart/{country_name}`: Generate a bar chart for a specific country.
- `/generate_pie_chart/{continent_name}`: Generate a pie chart for a specific continent.

For detailed documentation, please see [API Documentation](#api-documentation).

## API Documentation

For detailed information on available routes and endpoints, refer to the [API Documentation](API_DOCUMENTATION.md).

## Getting Started

1. Clone this repository: `git clone https://github.com/yourusername/WorldDemographicsAPI.git`
2. Install environment: `python3 -m venv env`
3. Activate environment: `source env/bin/activate`
4. Install the required dependencies by running: `pip install -r requirements.txt`
5. Run the application: `uvicorn main:app --reload`
6. Access the API at `http://localhost:8000`

## Contributing

Contributions are welcome! Please feel free to open issues and pull requests. For major changes, please discuss them in advance.

## License

This project is licensed under the [MIT License](LICENSE).