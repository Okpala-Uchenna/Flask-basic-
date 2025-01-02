# Flask Basic Application

This is a simple Flask application that returns a JSON message when accessed at the root endpoint (`/`).

## Features
- A minimal Flask app.
- Returns a JSON response: `{"message": "hey there python"}`.

---

## Code Overview

### Application Code
The application is defined as follows:

```python
from flask import Flask

helloworld = Flask(__name__)

@helloworld.route("/")
def run():
    return "{\"message\":\"hey there python\"}"

if __name__ == "__main__":
    helloworld.run(host="0.0.0.0", port=int("3000"), debug=True
