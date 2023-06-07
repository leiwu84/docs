# docs
Write documentation/notes


# Way of work
Create an virtual environment of Python on local drive, but write actual docs/notes on cloud drive. 
This way, the cloud drive does not need to sync a large amount of files from the virtual environment.


## Create a folder on local drive.

```
$mkdir docs_server
$cd docs_server
$virtualenv venv
$source venv/bin/activate
$pip install -r requirements.txt
```

## Create a dedicated folder for docs/notes on cloud drive. 

1. Create a root folder, e.g. `notes`.
2. Copy everything from the root folder, except the `README.md` file, of this repo to the root folder `notes`.


## Run the server
```$mkdocs server
