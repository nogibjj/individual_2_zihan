# Rust CLI Binary with SQLite
[![Rust CLI Binary](https://github.com/nogibjj/individual_2_zihan/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/individual_2_zihan/actions/workflows/cicd.yml)
## Overview

This project is a Rust command-line application that performs various operations on a SQLite database using data from a CSV file. The project demonstrates the use of Rust for handling data extraction, transformation, and CRUD (Create, Read, Update, Delete) operations on a SQLite database.

## Project Structure

- `.devcontainer/`: Contains configuration files for developing in a containerized environment.
  - `Dockerfile`: Defines the container image.
  - `devcontainer.json`: Configuration for the development container.

- `.github/workflows/`: Contains GitHub Actions workflows.
  - `cicd.yml`: Workflow for continuous integration and continuous deployment.

- `rust-cli-binary/`: Contains the main Rust application.
  - `src/`: Source code directory.
    - `main.rs`: Entry point of the CLI application.
    - `lib.rs`: Library containing functions for data operations.
  - `tests/`: Directory containing test files.
    - `test.rs`: Tests for the CLI application.
  - `Cargo.toml`: Cargo configuration file.
  - `flights.csv`: Example CSV file containing sample flight data.
  - `test_flights.csv`: CSV file used for testing.

- `Makefile`: Makefile for managing project commands.

## Requirements

- Rust (https://www.rust-lang.org/tools/install)
- Docker (for development container, optional)

## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-repo-url/rust-cli-binary.git
   cd rust-cli-binary
   ```

2. **Install dependencies:**
   ```sh
   make install
   ```

3. **Build the project:**
   ```sh
   make release
   ```

4. **Run the application:**
   ```sh
   make run
   ```

5. **Format the code:**
   ```sh
   make format
   ```

6. **Lint the code:**
   ```sh
   make lint
   ```

7. **Run tests:**
   ```sh
   make test
   ```

## Usage

The CLI application performs the following operations:
- Extract data from a URL and save it to a CSV file.
- Transform the CSV data into a SQLite database.
- Perform CRUD operations on the SQLite database.

## GitHub Actions

The project includes a CI/CD pipeline using GitHub Actions:
- **build**: Checks out the code, installs dependencies, builds the project, formats the code, runs lint checks, and executes tests.
- **upload-artifact**: Archives the optimized Rust binary.

## Using GitHub Copilot

GitHub Copilot was utilized throughout this project to assist in writing Rust code. It provided suggestions and code snippets that helped streamline the development process.

## SQLite Database Schema

The database schema used in this project consists of a single table:
- `data`: Contains columns for `year`, `month`, and `passengers`.

## Video Demonstration

For a detailed walkthrough and demonstration of this CLI application, please check out this [YouTube video](https://youtu.be/your-video-link).

## Acknowledgments

Special thanks to GPT for enhancing the coding experience and productivity throughout the development of this project.
