# Novamind Flow - Airflow Project

This repository contains an Apache Airflow setup for orchestrating data workflows.

## Project Structure

```
.
├── airflow.cfg           # Main Airflow configuration file
├── webserver_config.py   # Airflow webserver configuration
├── airflow.db           # SQLite database for Airflow metadata
└── logs/                # Directory containing Airflow logs
```

## Setup Instructions

1. Make sure you have Python 3.7+ installed
2. Install Apache Airflow:
   ```bash
   pip install apache-airflow
   ```

3. Initialize the Airflow database:
   ```bash
   airflow db init
   ```

4. Start the Airflow webserver:
   ```bash
   airflow webserver --port 8080
   ```

5. In a new terminal, start the Airflow scheduler:
   ```bash
   airflow scheduler
   ```

6. Access the Airflow UI at `http://localhost:8080`

## Configuration

The main configuration file is `airflow.cfg`. Key configurations can be modified here, including:
- Database settings
- Executor settings
- Webserver configurations
- Security settings

## Development

To add new DAGs:
1. Create a new Python file in the `dags/` directory
2. Define your DAG using the Airflow DAG API
3. The DAG will automatically be picked up by the scheduler

## Security Note

- The `standalone_admin_password.txt` contains the admin password for standalone mode
- Make sure to secure your credentials and never commit sensitive information to version control

## Additional Resources

- [Apache Airflow Documentation](https://airflow.apache.org/docs/apache-airflow/stable/index.html)
- [Best Practices](https://airflow.apache.org/docs/apache-airflow/stable/best-practices.html) 