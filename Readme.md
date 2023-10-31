## Information

![image](https://github.com/dogukannulu/csv_extract_airflow_docker/assets/91257958/d0c01724-d2c6-4646-8f22-dac0ea3b5931)


```bash
pip install -r requirements.txt

```

## Steps

`write_csv_to_postgres.py`-> gets a csv file from a URL. Saves it into the local working directory as [churn_modelling.csv](https://raw.githubusercontent.com/dogukannulu/datasets/master/Churn_Modelling.csv). After reading the csv file, it writes it to a local PostgreSQL table

`create_df_and_modify.py` -> reads the same Postgres table and creates a pandas dataframe out of it, modifies it. Then, creates 3 separate dataframes.

`write_df_to_postgres.py` -> writes these 3 dataframes to 3 separate tables located in Postgres server. 





## PostgreSQL

I am using a local Postgres Server and installed `PgAdmin` to control the tables instead of using `psql`.
