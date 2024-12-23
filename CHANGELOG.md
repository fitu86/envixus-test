# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]



### Added
- Added error handling and validation for CSV columns in `load_data.py`.
- Added preprocessing step to handle missing columns in `load_data.py`.
- Added default source data insertion in `load_data.py`.
- Added `preprocess_csv` function to `load_data.py` to ensure all required columns are present.
- Added `validate_csv` function to `load_data.py` to validate CSV columns against the database schema.
- Added `insert_vehicle_if_not_exists` function to `load_data.py` to prevent duplicate vehicle entries.
- Added `add_default_sources` function to `load_data.py` to insert default source data.
- Added `clean_and_reformat_data` function to `clean_data.py` to clean and reformat the input CSV data.
- Added `etl_pipeline` function to `ETLpipeline.py` to handle the ETL process for vehicle data.
- Added `transform_data` function to `ETLpipeline.py` to transform raw data to match the database schema.
- Added `.gitignore` and `.env_example` for managing environment variables.

### Changed
- Updated `scripts/clean_data.py` to handle cases where `engine` column has unexpected formats.
- Ensured all values are converted to strings before processing in `scripts/clean_data.py`.
- Updated `db_config.py` to handle environment variable-based configurations.
- Corrected input/output paths in `scripts/clean_data.py`.
- Updated `README.md` to fix errors and clarify usage instructions.

### Fixed
- Fixed "list index out of range" error in `scripts/clean_data.py`.
- Fixed "argument of type 'float' is not iterable" error in `scripts/clean_data.py`.
- Fixed path issues in `scripts/load_data.py` for compatibility with the new project structure.
- Added required packages (`python-dotenv`, `SQLAlchemy`, `psycopg2-binary`) to `requirements.txt`.

## [Initial Release]
- Initial setup of the repository.
