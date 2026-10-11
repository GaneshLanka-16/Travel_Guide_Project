# Travel Guide

A Flask app that serves the travel guide frontend and generates narrated destination guides using Gemini and Murf.

## Run locally

1. Create `Backend/.env` with your API keys. Use `Backend/.env.example` as the template.
2. Install the Python dependencies with `pip install -r Backend/requirements.txt`.
3. Start the app with `python Backend/app.py`.
4. Open <http://127.0.0.1:5000>.

## Deploy on Render

This repository includes `render.yaml` for a single web service. Create a new Blueprint in Render from the GitHub repository, then set `GEMINI_API_KEY` and `MURF_API_KEY` in the service environment settings. Render installs the dependencies and starts the Flask app with Gunicorn. The `.env` file is excluded from Git; never commit API keys.
