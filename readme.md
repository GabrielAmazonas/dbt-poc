### Step 0: Install Docker and docker-compose
[Install Docker Here](https://docs.docker.com/get-docker/)

Clone this repository, change the terminal directory to it's main folder and run:

```
docker-compose up
```

- This will spin up a container running a Postgres database @ localhost:5432

### Step 1: Create and activate a virtualenv:

Create a new virtual environment for the project in its root directory:

```
python3 -m venv .venv
```

Activate it:

```
source .venv/bin/activate
```

Run from the root directory the pip install to get boto3.

```
pip3 install -r requirements.txt
```

Change the directory to `.dbt`  and copy the profiles.yml file to ~/.dbt

```
cd .dbt

cp profiles.yml ~/.dbt
```

Change the directory to `dbtpoc` 

```
cd dbtpoc
```

Run  `dbt debug`