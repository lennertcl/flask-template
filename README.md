# flask-template

Based on: https://github.com/CoreyMSchafer/code_snippets/tree/master/Python/Flask_Blog/13-Deployment-Linode

## Quickstart

### Install requirements

Create virtual environment and activate it.

Linux/mac:
```
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Windows:
```
python -m venv venv
call venv/Scripts/activate.bat
pip install -r requirements.txt
```

### Set the necessary config variables

Copy the `website/.env.example` file to `website/.env`.
Enter the correct information for your system:

```
SECRET_KEY=<your secret key>
SECURITY_PASSWORD_SALT=<your password salt>
SQLALCHEMY_DATABASE_URI=<location of the database>
EMAIL_USER=<app gmail account>
EMAIL_PASS=<app gmail password>
```

### Initialize the database

```python
python create_db.py
```

### Run the application

```
python run.py
```
