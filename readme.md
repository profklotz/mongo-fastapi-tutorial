# MongoDB and FastAPI Tutorial

This repository contains the Python code for the MongoDB and FastAPI tutorial which has been executed as part of the
*Big Data Management and Analytics* course at Hochschule der Medien Stuttgart.  

**Credits**: The code follows this great tutorial from MongoDB:
https://www.mongodb.com/languages/python/pymongo-tutorial

## Installation
This code was tested on Python version 3.10, running in an Anaconda environment.

The following packages have been installed:
- `fastapi` (from channel `conda-forge`)
- `uvicorn`
- `pymongo`
- `dnspython`
- `python-dotenv`

An [export of the Anaconda environment](req.txt) has been added to the repository. It can be used to create a new
environment with all the packages using the following statement: 

```$ conda create --name <env> --file req.txt```

## MongoDB Information

You need to manually create a file named `.env` in the project directory which contains the following contents:

```
ATLAS_URI=mongodb+srv://<user>:<pass>@<host>/?retryWrites=true&w=majority
DB_NAME=<db-name>
```