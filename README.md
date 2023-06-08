# docs-server
Mkdocs Material server to write documentation/notes


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
2. Copy everything in the `docs` folder and `mkdocs.yml` file from this repo to the root folder `notes`.
3. Change `site_name` and `copyright` in the `mkdocs.yml` file.


## Usage

1. `cd` to the folder of `docs_server`.
2. Activiate the `venv`.
    ```
    source venv/bin/activate
    ```
3. `cd` to the folder of documentation root folder like `notes`.
4. Run commmand
    ```
    $mkdocs serve
    ```