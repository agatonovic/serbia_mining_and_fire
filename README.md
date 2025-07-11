# Serbian Geology & Fire Reporting App

An interactive web application for visualizing mining research locations and fire reports in Serbia. Combines geological data (Geo Srbija) and NASA FIRMS fire data on a modern, bilingual map with user fire reporting and voting.

## Features
- Interactive map with geology and fire layers
- User fire reporting (right-click on map)
- Date/radius filtering, media upload, voting
- Bilingual UI (Serbian/English)
- Professional info bar with Buy Me a Coffee
- Responsive, mobile-friendly design

## Demo (GitHub Pages)
The static frontend is available at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO/
```

## Local Development
### 1. Frontend (Static Map)
You can test the static HTML/JS frontend locally:
```sh
python -m http.server 8000
# Then open http://localhost:8000/geology_template.html
```

### 2. Backend (API/Streamlit)
If you want to run the backend (for fire reporting, database, etc):
```sh
pip install -r requirements.txt
python simple_api_server.py
# or
streamlit run main.py
```

## Deployment to GitHub Pages
1. Push all static files (HTML, JS, CSS, images, JSON) to the repo root.
2. Rename your main HTML file to `index.html` or add a redirect `index.html`:
```html
<meta http-equiv="refresh" content="0; url=geology_template.html">
```
3. Enable GitHub Pages in repo settings (branch: main, folder: /root).
4. Visit your published site at the URL above.

## Data Sources
- [Geo Srbija](https://geosrbija.rs/)
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/)

## License
MIT