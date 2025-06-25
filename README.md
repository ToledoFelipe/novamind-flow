# Novamind Flow - Data Ecossystem for testing and learning

This repository contains an Apache Airflow setup for orchestrating data workflows.

## Setup Instructions

1. Install docker
2. Build docker-compose
3. Run docker-compose
4. (Optional) Set Ubuntu Keyboard Layout to Portuguese
```bash
setxkbmap -model abnt2 -layout br
```

# To DO
- Design Airflow infrastructure
    - Principal commponents
        - webserver
            - How Flask works with Airflow
        - triggerer
        - scheduler
        - standalone

- Create a crawler based at python operator and run locally, retrieve the information as json reading though https://www.tabnews.com.br/ 
- Add a pre commit and after commit with a github actions to apply security checks 
- Add black for identation and flake8 for better quality code
- Add a library with other stuff such quality, dag structure and quality

---

# Fonts

- [Apache Airflow Documentation](https://airflow.apache.org/docs/apache-airflow/stable/index.html)
- [Best Practices](https://airflow.apache.org/docs/apache-airflow/stable/best-practices.html) 