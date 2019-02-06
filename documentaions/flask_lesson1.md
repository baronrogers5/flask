# Flask

> Flask is an easy to use framework for serving html pages and web content. <br>
It comes with a barebones instalalation and is very easy to set up and get started with, giving the developer the freedom of choosing the database, login and form handling and all the nitty-gritty stuff.

## Running a Flask app

To run a basic flask app like the below hello world example, we need to export some variables in the terminal:

```shell 
export FLASK_APP=<name_of_app.py>
$ flask run
```
> Sample hello world flask code
```python
from flask import Flask
app = Flask(__name__)


@app.route('/')
def hello():
    # shows embedded html tag in return statement
    return '<h2>hello world!</h2>'

```
This will run the app and we can copy the link and view the results in a web-browser.<br>
But, everytime a change is required we need to restart the running flask server, to remove such hinderances, we can run flask in debug mode, by:
```shell
export FLASK_DEBUG=1
$ flask run
```
Doing so allows us to make changes on the fly and refresh the browser window to observe the changes.
