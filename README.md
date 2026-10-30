# Flask website (GitHub + Render)

## Run locally
1. Install Python 3.10 or newer.
2. Open a terminal in this folder.
3. Run `pip install -r requirements.txt`
4. Run `python app.py`
5. Open `http://127.0.0.1:5000`

## Deploy on Render
1. Upload all files in this folder to a GitHub repository.
2. In Render, choose **New +** → **Blueprint**.
3. Connect the GitHub repository.
4. Render reads `render.yaml`; approve deployment.
5. Open the generated `onrender.com` URL.

You can also choose **New +** → **Web Service**, select the repository, set:
- Runtime: Python
- Build command: `pip install -r requirements.txt`
- Start command: `gunicorn app:app`

## Customize
Edit `templates/index.html` for page text/content and `static/css/style.css` for design.
The supplied HTML's JavaScript is obfuscated, so this is a deploy-ready Flask starter, not an exact recovery of the original site's hidden features.
