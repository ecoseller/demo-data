# Demo Data Repository 

This repository contains a PostgreSQL database dump with demo data extracted from the MFF UK Movie Store dataset. The dataset consists of over 1000 movies, 2000+ variants, several orders, reviews, and product images. The movies can be purchased in different languages (Czech, English) and resolutions (720p, 1080p).

The primary purpose of this repository is to provide a sample dataset that can be used for testing, development, or educational purposes related to working with [ecosller](https://github.com/ecoseller/ecoseller) platform.

## Usage in EcoSeller Demo Instance

This demo data repository serves as the source of data for the **ecoseller** demo instance. The **ecoseller** demo instance is a simulation of the **ecoseller** platform. The demo instance utilizes this repository's data to showcase the functionality of the **ecoseller** platform.

## Integration with **ecosller** Backend Service

The demo data from this repository is integrated into the EcoSeller backend service using the following steps:

1. The [EcoSeller backend service](https://github.com/ecoseller/ecoseller) is set up using the [docker-compose.demo.yaml](https://github.com/ecoseller/ecoseller/blob/master/src/docker-compose.demo.yaml) configuration file.

2. Upon startup, the backend service executes the [demo_data_loader.sh](https://github.com/ecoseller/ecoseller/blob/master/src/backend/core/demo_data_loader.sh) script. This script pulls the data from this repository and loads it into the local PostgreSQL database used by the backend service.

## Dataset Overview

The dataset includes the following components:

- **Movies**: Over 1000 movie records, each containing details like title, description, release year, and genre.
- **Variants**: 2000+ variant records associated with movies. These variants represent different language and resolution options for each movie.
- **Orders**: Sample order records to demonstrate the relationship between customers and purchased products.
- **Reviews**: Sample review records associated with products, including ratings and comments.
- **Product Images**: Images of movie covers and promotional materials.


# Acknowledgments

The demo data in this repository is based on the MFF UK Movie Store dataset. We would like to express our gratitude to MFF UK for providing this dataset for educational and demonstration purposes.

# License

This demo data repository is provided under the MIT License.