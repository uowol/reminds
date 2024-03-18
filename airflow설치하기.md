### install
```sh
pip install 'apache-airflow==2.6.3 \
--constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.6.3constraints-3.11.txt"
```

### db init -> cfg, db 생성
```sh
airflow db init
```

### add admin account
```sh
export AIRFLOW_HOME=`pwd`
echo $AIRFLOW_HOME 
airflow users create \
--username admin \
--password '!boostcamp-aitech!' \
--firstname kim \
--lastname chanwoo \
--role Admin \
--email alllhvhla@gmail.com
```

### start webserver
```sh
export AIRFLOW_HOME=`pwd`
echo $AIRFLOW_HOME 
airflow webserver ­--port 8080
```

### start scheduler
```sh
export AIRFLOW_HOME=`pwd`
echo $AIRFLOW_HOME 
airflow scheduler
```

