# TiDB Python Connector Examples

This repository contains example code demonstrating how to use TiDB with Python, specifically designed for [TiDB Labs](https://labs.tidb.io). These examples showcase various ways to interact with TiDB using the MySQL Connector/Python.

## Prerequisites

- Python 3.11 or later
- Poetry (Python package manager)
- Access to a TiDB database instance

## Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/tidb-lab-python.git
   cd tidb-lab-python
   ```

2. Install dependencies using Poetry:

   ```bash
   poetry install
   ```

3. Create a `.env` file in the root directory with your TiDB connection details:

   ```properties
   TIDB_HOST=your_tidb_host
   TIDB_PORT=4000
   TIDB_USER=your_username
   TIDB_PASSWORD=your_password
   TIDB_DB_NAME=your_database
   ```

## Examples

This repository includes several examples demonstrating different aspects of working with TiDB:

### Basic Connection

- `demo_connection.py`: Shows how to establish a basic connection to TiDB with SSL verification

### Query Examples

- `query_fetch_all.py`: Demonstrates how to fetch all rows from a query result
- `query_fetch_one.py`: Shows how to fetch a single row from a query result
- `positional_placeholders.py`: Examples of using positional placeholders in queries
- `named_placeholders.py`: Examples of using named placeholders in queries

### Data Manipulation

- `batch_insert.py`: Shows how to perform efficient batch insertions
- `prepared_statement.py`: Demonstrates the use of prepared statements

## Usage

Each example can be run directly using Python. For example:

```bash
python demo_connection.py
```

## Project Structure

```bash
.
├── README.md
├── pyproject.toml          # Poetry project configuration
├── poetry.lock            # Poetry dependency lock file
├── .env                   # Environment variables (create this)
├── demo_connection.py     # Basic connection example
├── query_fetch_all.py     # Fetch all rows example
├── query_fetch_one.py     # Fetch single row example
├── positional_placeholders.py  # Positional parameters example
├── named_placeholders.py  # Named parameters example
├── batch_insert.py        # Batch insertion example
└── prepared_statement.py  # Prepared statements example
```

## Dependencies

- `mysql-connector-python`: Official MySQL driver for Python
- `python-dotenv`: For loading environment variables from .env file
