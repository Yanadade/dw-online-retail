# dw-online-retail 📝

* docker-airflow
* Google Cloud Platform (GCP): Google Cloud Storage (GCS) / Google Bigquery
* data build tool (dbt) 
* Looker studio


# Data Pipeline 🚀

<br>
<p align="center">
<img src="https://github.com/Yanadade/dw-online-retail/blob/main/image/Architecture.jpg" width="100%"></img> 
</p>

# Data Model 📃

<br>
<p align="center">
<img src="https://github.com/Yanadade/dw-online-retail/blob/main/image/datamodeling.png" width="100%"></img> 
</p>

# Visualization 📊

<br>
<p align="center">
<img src="https://github.com/Yanadade/dw-online-retail/blob/main/image/dashboard%201.jpg" width="100%"></img> 
<p align="center">
<img src="https://github.com/Yanadade/dw-online-retail/blob/main/image/dashboard%202.jpg" width="100%"></img> 
</p>

### Get Start on Codespaces


```sh
cd online-retail/
```

```sh
python -m venv ENV
```

```sh
source ENV/bin/activate
```

Running docker-airflow (port: 8080)
```sh
docker compose up
```

Download library dbt-core dbt-bigquery for able to use dbt tools and dbt connect to bigquery.
```sh
pip install dbt-core dbt-bigquery
```

create project profile dbt used to google bigqeury 
```sh
dbt init
```

create profiles.yml file in dbt_modeling folder and copy code to profiles.yml file 
```sh
code /home/codespace/.dbt/profiles.yml
```

change Directory to dbt_modeling for working with profiles.yml
```sh
cd dbt_modeling
```

check connection DBT with Google Bigquery
```sh
dbt debug
```

create tables/views follow with .sql files and according with schema.yml
```sh
dbt run
```

check conditions tables/views matching conditions 
```sh
dbt test
```

### Close webserver

To shutdown, press Ctrl+C and run: 
```sh
docker compose down
```

### Connect Bigquery with Looker studio
