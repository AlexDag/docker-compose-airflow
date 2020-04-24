# docker-compose-airflow
Docker Compose Apache Airflow (Official Docker Images) with CeleryExecutor, InitDB and InitUser

Ideal for local development or small scale personal deployments.

### How to deploy:

**Step 1:** Clone this Repo and open terminal

**Step 2:** Go through .env file, init_airflow_setup.sh, docker-compose.yml file to change settings according to your preference. Or you can just keep them as it is for local development.

**Step 3:** Run `docker-compose up -d`

**Step 4:** Run `sh init_airflow_setup.sh` (Only run this for initial deployment)

**Step 5:** Go to http://localhost:8080 and login with user: _airflow_test_user_ and password: _airflow_test_password_ as specified in init_airflow_setup.sh script

**Step 6:** Run few dags and monitor Celery workers at http://localhost:5555