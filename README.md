# Simple Sensor Logging
This project was created as a guide and an example of a machine sensor logging format that is easily consumed by Sight Machine. This is just one of many schemas. Additionally this should be used as an example for creating production systems and is not recommended to use this as a stand along log.

## Tag structure
This database schema describes a tag. A tag consists of the following information:

* **Timestamp** of when the sensor reading was taken
* **Name** of the sensor being read. Preferably this is a human readable name.
* **Value** of the sensor that was read

There are also optional fields:

* **Location** of the sensor. This can be different in many cases:
 * Indicate Machine
 * Indicate zone, section, or workarea
* **Data Type**: what is the data type of the sensor value:
 * There is currently no predefined list of valid data types
 * Best practice would be to indicate string, int, float, etc.

This schema can be extended as needed

## Supporting tools

This was completed with the following:

* Postgres Docker Container (this is configured in the docker-compose.yml file)
* JupyterLab
* 3rd party libraries installed via pip (documented in the notebook)

## Quick start

Assuming that you are using ubuntu, run the commands in [this setup script](https://gist.github.com/jplsightm/523cfee0f7f058d327f5309bcf0dbcc8). This is doing the following:

* Installing [Docker](https://www.docker.com/)
* Installing [docker-compose](https://docs.docker.com/compose/overview/)

If you do not have an account with [Docker Hub](https://docs.docker.com/docker-hub/)

```
docker login
```

Login with the username and password you created.

Checkout the needed repos and 
