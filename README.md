# Sample Flask App

A small Flask application that renders a home page.

## Run locally

1. Create and activate a virtual environment:

   ```sh
   python3 -m venv .venv
   source .venv/bin/activate
   ```

2. Install the dependencies:

   ```sh
   pip install -r requirements.txt
   ```

3. Start the development server:

   ```sh
   flask --app app run
   ```

Open the local URL printed by Flask in your browser.

## Production server

The included `Procfile` starts the app with Gunicorn. To run that command locally:

```sh
gunicorn --worker-tmp-dir /dev/shm --config gunicorn_config.py app:app
```
