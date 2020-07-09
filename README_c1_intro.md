Chapter 1: Introduction

Install Python
Install Poetry
Poetry shell
Install Flask

mkdir microblog
cd microblog
mkdir app

touch app/__init__.py
<!-- from flask import Flask

app = Flask(__name__)

from app import routes -->

touch app/routes.py
<!-- from app import app

@app.route('/')
@app.route('/index')
def index():
    return "Hello, World!" -->

touch microblog/microblog.py (main)
<!-- from app import app -->

export FLASK_APP=microblog.py
flask run
<!-- * Serving Flask app "microblog"
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit) -->

pip install python-dotenv

touch microblog/.flaskenv
<!-- FLASK_APP=microblog.py -->
