# Weather Application

This project is a weather application designed to fetch and display weather-related information. It is built using R and utilizes environment-specific configurations to manage API keys and other sensitive data.

## Project Structure

- `weather.r`: The main R script responsible for handling weather-related operations.
- `.env`: Contains environment variables such as API keys (not included in the repository).
- `.env.example`: A template for the environment variables required for the project.
- `renv.lock`: A lock file used to manage R package dependencies with renv.
- `renv`: A directory used to isolate the R package environment.
- `README.md`: Project documentation (this file).

## Getting Started

### Prerequisites

- R (version >= 4.0.0)
- `renv` for package management in R. You can install it using the following command in R:

```r
install.packages("renv")
```

### Setting up the Environment

1. Copy the `.env.example` file to `.env`:

```bash
cp .env.example .env
```

2. Open `.env` and configure the required environment variables, such as your API key for the weather service.

### Installing Dependencies

To install the required R packages, use the `renv` package to restore the environment:

```r
renv::restore()
```

This will install all necessary dependencies based on the `renv.lock` file.

### Running the Application

Once the environment is set up, you can run the application by executing the `weather.r` script in R:

```r
source("weather.r")
```

This will fetch weather information based on the API configurations and display the results.

## Environment Variables

The following environment variables are required:

- `API_KEY`: The API key for accessing the weather service.

Make sure to set these variables in your `.env` file before running the application.
